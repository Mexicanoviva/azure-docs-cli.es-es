---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/23/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 65e34ab6014c47ae92a6d4bae8cdc30d4a1413dc
ms.sourcegitcommit: aec89531c938781b4724f43b5bb4b878e106a26a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/23/2018
ms.locfileid: "49952492"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="091e2-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="091e2-103">Azure CLI release notes</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="091e2-104">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-104">October 23, 2018</span></span>

<span data-ttu-id="091e2-105">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="091e2-105">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="091e2-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-106">Core</span></span>
* <span data-ttu-id="091e2-107">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="091e2-107">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="091e2-108">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="091e2-108">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-109">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-109">ACR</span></span>
* <span data-ttu-id="091e2-110">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="091e2-110">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="091e2-111">CDN</span><span class="sxs-lookup"><span data-stu-id="091e2-111">CDN</span></span>
* <span data-ttu-id="091e2-112">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="091e2-112">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="091e2-113">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="091e2-113">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="091e2-114">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-114">Container</span></span>
* <span data-ttu-id="091e2-115">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="091e2-115">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="091e2-116">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-116">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="091e2-117">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="091e2-117">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="091e2-118">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-118">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="091e2-119">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="091e2-119">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="091e2-120">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="091e2-120">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="091e2-121">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="091e2-121">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="091e2-122">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="091e2-122">CosmosDB</span></span>
* <span data-ttu-id="091e2-123">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="091e2-123">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-124">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-124">Interactive</span></span>
* <span data-ttu-id="091e2-125">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="091e2-125">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="091e2-126">IoT Central</span><span class="sxs-lookup"><span data-stu-id="091e2-126">IoT Central</span></span>
* <span data-ttu-id="091e2-127">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="091e2-127">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="091e2-128">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="091e2-128">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-129">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-129">Monitor</span></span>
* <span data-ttu-id="091e2-130">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="091e2-130">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="091e2-131">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="091e2-131">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="091e2-132">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="091e2-132">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="091e2-133">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="091e2-133">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="091e2-134">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="091e2-134">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="091e2-135">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="091e2-135">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="091e2-136">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="091e2-136">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="091e2-137">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="091e2-137">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="091e2-138">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="091e2-138">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="091e2-139">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="091e2-139">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="091e2-140">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-140">Network</span></span>
* <span data-ttu-id="091e2-141">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="091e2-141">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="091e2-142">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="091e2-142">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="091e2-143">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="091e2-143">ServiceBus</span></span>
* <span data-ttu-id="091e2-144">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="091e2-144">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-145">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-145">SQL</span></span>
* <span data-ttu-id="091e2-146">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="091e2-146">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-147">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-147">Storage</span></span>
* <span data-ttu-id="091e2-148">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="091e2-148">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="091e2-149">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="091e2-149">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-150">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-150">VM</span></span>
* <span data-ttu-id="091e2-151">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="091e2-151">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="091e2-152">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="091e2-152">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="091e2-153">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="091e2-153">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="091e2-154">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-154">October 16, 2018</span></span>

<span data-ttu-id="091e2-155">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="091e2-155">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-156">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-156">VM</span></span>
* <span data-ttu-id="091e2-157">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="091e2-157">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="091e2-158">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-158">October 9, 2018</span></span>

<span data-ttu-id="091e2-159">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="091e2-159">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="091e2-160">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-160">Core</span></span>
* <span data-ttu-id="091e2-161">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="091e2-161">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-162">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-162">ACR</span></span>
* <span data-ttu-id="091e2-163">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="091e2-163">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-164">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-164">ACS</span></span>
* <span data-ttu-id="091e2-165">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="091e2-165">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="091e2-166">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="091e2-166">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="091e2-167">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="091e2-167">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="091e2-168">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="091e2-168">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="091e2-169">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-169">Container</span></span>
* <span data-ttu-id="091e2-170">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="091e2-170">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="091e2-171">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="091e2-171">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="091e2-172">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="091e2-172">Event Hub</span></span>
* <span data-ttu-id="091e2-173">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="091e2-173">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="091e2-174">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="091e2-174">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="091e2-175">Extensiones</span><span class="sxs-lookup"><span data-stu-id="091e2-175">Extensions</span></span>
* <span data-ttu-id="091e2-176">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="091e2-176">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="091e2-177">HDInsight</span><span class="sxs-lookup"><span data-stu-id="091e2-177">HDInsight</span></span>
* <span data-ttu-id="091e2-178">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="091e2-178">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-179">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-179">IoT</span></span>
* <span data-ttu-id="091e2-180">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="091e2-180">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-181">KeyVault</span><span class="sxs-lookup"><span data-stu-id="091e2-181">KeyVault</span></span>
* <span data-ttu-id="091e2-182">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="091e2-182">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="091e2-183">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-183">Network</span></span>
* <span data-ttu-id="091e2-184">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="091e2-184">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="091e2-185">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="091e2-185">See #6052</span></span>
* <span data-ttu-id="091e2-186">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="091e2-186">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="091e2-187">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="091e2-187">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="091e2-188">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="091e2-188">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="091e2-189">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="091e2-189">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="091e2-190">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="091e2-190">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="091e2-191">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="091e2-191">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="091e2-192">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-192">Role</span></span>
* <span data-ttu-id="091e2-193">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="091e2-193">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="091e2-194">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="091e2-194">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="091e2-195">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="091e2-195">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="091e2-196">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="091e2-196">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="091e2-197">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="091e2-197">Service Bus</span></span>
* <span data-ttu-id="091e2-198">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="091e2-198">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-199">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-199">VM</span></span>
* <span data-ttu-id="091e2-200">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="091e2-200">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="091e2-201">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="091e2-201">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="091e2-202">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="091e2-202">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="091e2-203">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="091e2-203">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="091e2-204">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="091e2-204">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="091e2-205">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="091e2-205">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="091e2-206">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-206">September 21, 2018</span></span>

<span data-ttu-id="091e2-207">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="091e2-207">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-208">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-208">ACR</span></span>
* <span data-ttu-id="091e2-209">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-209">Added ACR Task commands</span></span>
* <span data-ttu-id="091e2-210">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="091e2-210">Added quick run command</span></span>
* <span data-ttu-id="091e2-211">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="091e2-211">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="091e2-212">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-212">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="091e2-213">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="091e2-213">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="091e2-214">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="091e2-214">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-215">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-215">ACS</span></span>
* <span data-ttu-id="091e2-216">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="091e2-216">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="091e2-217">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="091e2-217">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-218">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-218">AppService</span></span>

* <span data-ttu-id="091e2-219">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="091e2-219">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="091e2-220">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="091e2-220">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="091e2-221">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="091e2-221">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="091e2-222">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="091e2-222">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-223">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-223">Batch</span></span>
* <span data-ttu-id="091e2-224">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="091e2-224">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="091e2-225">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="091e2-225">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="091e2-226">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="091e2-226">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="091e2-227">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="091e2-227">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="091e2-228">Batch AI</span><span class="sxs-lookup"><span data-stu-id="091e2-228">Batch AI</span></span> 
* <span data-ttu-id="091e2-229">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="091e2-229">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="091e2-230">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="091e2-230">Cognitive Services</span></span>
* <span data-ttu-id="091e2-231">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="091e2-231">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="091e2-232">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="091e2-232">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="091e2-233">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="091e2-233">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="091e2-234">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="091e2-234">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="091e2-235">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-235">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="091e2-236">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="091e2-236">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="091e2-237">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-237">Container</span></span>
* <span data-ttu-id="091e2-238">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="091e2-238">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="091e2-239">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="091e2-239">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="091e2-240">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-240">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="091e2-241">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-241">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="091e2-242">DataLake</span><span class="sxs-lookup"><span data-stu-id="091e2-242">Datalake</span></span>
* <span data-ttu-id="091e2-243">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-243">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="091e2-244">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="091e2-244">Interactive Shell</span></span>
* <span data-ttu-id="091e2-245">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="091e2-245">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="091e2-246">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="091e2-246">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-247">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-247">IoT</span></span>
* <span data-ttu-id="091e2-248">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-248">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="091e2-249">Key Vault</span><span class="sxs-lookup"><span data-stu-id="091e2-249">Key Vault</span></span>
* <span data-ttu-id="091e2-250">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="091e2-250">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="091e2-251">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-251">Network</span></span>
* <span data-ttu-id="091e2-252">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="091e2-252">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="091e2-253">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="091e2-253">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="091e2-254">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="091e2-254">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="091e2-255">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="091e2-255">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="091e2-256">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="091e2-256">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="091e2-257">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="091e2-257">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="091e2-258">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="091e2-258">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="091e2-259">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="091e2-259">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="091e2-260">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="091e2-260">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="091e2-261">`network express-route create/update`: se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="091e2-261">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="091e2-262">`network vnet subnet create/update`: se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="091e2-262">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="091e2-263">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="091e2-263">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="091e2-264">`network traffic-manager profile create/update`: se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` a Monitor Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="091e2-264">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="091e2-265">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="091e2-265">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="091e2-266">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="091e2-266">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="091e2-267">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="091e2-267">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="091e2-268">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="091e2-268">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="091e2-269">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="091e2-269">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="091e2-270">RDBMS</span><span class="sxs-lookup"><span data-stu-id="091e2-270">RDBMS</span></span>
* <span data-ttu-id="091e2-271">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="091e2-271">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="091e2-272">Reserva</span><span class="sxs-lookup"><span data-stu-id="091e2-272">Reservation</span></span>
* <span data-ttu-id="091e2-273">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="091e2-273">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="091e2-274">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="091e2-274">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="091e2-275">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="091e2-275">Manage App</span></span>
* <span data-ttu-id="091e2-276">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="091e2-276">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="091e2-277">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="091e2-277">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="091e2-278">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-278">Role</span></span>
* <span data-ttu-id="091e2-279">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="091e2-279">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="091e2-280">SignalR</span><span class="sxs-lookup"><span data-stu-id="091e2-280">SignalR</span></span>
* <span data-ttu-id="091e2-281">Primera versión</span><span class="sxs-lookup"><span data-stu-id="091e2-281">First release</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-282">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-282">Storage</span></span>
* <span data-ttu-id="091e2-283">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="091e2-283">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="091e2-284">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="091e2-284">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-285">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-285">VM</span></span>
* <span data-ttu-id="091e2-286">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="091e2-286">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="091e2-287">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="091e2-287">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="091e2-288">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-288">August 28, 2018</span></span>

<span data-ttu-id="091e2-289">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="091e2-289">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="091e2-290">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-290">Core</span></span>

* <span data-ttu-id="091e2-291">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="091e2-291">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="091e2-292">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="091e2-292">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-293">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-293">ACR</span></span>

* <span data-ttu-id="091e2-294">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="091e2-294">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="091e2-295">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="091e2-295">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-296">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-296">ACS</span></span>

* <span data-ttu-id="091e2-297">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="091e2-297">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="091e2-298">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="091e2-298">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-299">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-299">AppService</span></span>

* <span data-ttu-id="091e2-300">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="091e2-300">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="091e2-301">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-301">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="091e2-302">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-302">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="091e2-303">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="091e2-303">Backup</span></span>

* <span data-ttu-id="091e2-304">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-304">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="091e2-305">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="091e2-305">Bot Service</span></span>

* <span data-ttu-id="091e2-306">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="091e2-306">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="091e2-307">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="091e2-307">Cognitive Services</span></span>

* <span data-ttu-id="091e2-308">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="091e2-308">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-309">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-309">IoT</span></span>

* <span data-ttu-id="091e2-310">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="091e2-310">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-311">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-311">Monitor</span></span>

* <span data-ttu-id="091e2-312">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="091e2-312">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="091e2-313">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="091e2-313">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="091e2-314">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-314">Network</span></span>

* <span data-ttu-id="091e2-315">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-315">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-316">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-316">Resource</span></span>

* <span data-ttu-id="091e2-317">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-317">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-318">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-318">Storage</span></span>

* <span data-ttu-id="091e2-319">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-319">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-320">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-320">VM</span></span>

* <span data-ttu-id="091e2-321">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-321">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="091e2-322">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="091e2-322">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="091e2-323">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-323">Auguest 14, 2018</span></span>

<span data-ttu-id="091e2-324">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="091e2-324">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="091e2-325">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-325">Core</span></span>

* <span data-ttu-id="091e2-326">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="091e2-326">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="091e2-327">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="091e2-327">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="091e2-328">Telemetría</span><span class="sxs-lookup"><span data-stu-id="091e2-328">Telemetry</span></span>

* <span data-ttu-id="091e2-329">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="091e2-329">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-330">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-330">ACR</span></span>

* <span data-ttu-id="091e2-331">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="091e2-331">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="091e2-332">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="091e2-332">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-333">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-333">ACS</span></span>

* <span data-ttu-id="091e2-334">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="091e2-334">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="091e2-335">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="091e2-335">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="091e2-336">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="091e2-336">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="091e2-337">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="091e2-337">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="091e2-338">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="091e2-338">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="091e2-339">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-339">AppService</span></span>

* <span data-ttu-id="091e2-340">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="091e2-340">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="091e2-341">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="091e2-341">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="091e2-342">BatchAI</span><span class="sxs-lookup"><span data-stu-id="091e2-342">BatchAI</span></span>

* <span data-ttu-id="091e2-343">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="091e2-343">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="091e2-344">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-344">Container</span></span>

* <span data-ttu-id="091e2-345">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-345">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="091e2-346">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-346">IoT</span></span>

* <span data-ttu-id="091e2-347">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="091e2-347">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="091e2-348">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="091e2-348">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="091e2-349">Iot Central</span><span class="sxs-lookup"><span data-stu-id="091e2-349">Iot Central</span></span>

* <span data-ttu-id="091e2-350">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="091e2-350">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-351">KeyVault</span><span class="sxs-lookup"><span data-stu-id="091e2-351">KeyVault</span></span>


* <span data-ttu-id="091e2-352">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="091e2-352">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="091e2-353">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="091e2-353">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="091e2-354">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="091e2-354">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="091e2-355">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="091e2-355">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="091e2-356">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="091e2-356">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="091e2-357">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="091e2-357">Relay</span></span>

* <span data-ttu-id="091e2-358">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="091e2-358">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-359">Sql</span><span class="sxs-lookup"><span data-stu-id="091e2-359">Sql</span></span>

* <span data-ttu-id="091e2-360">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="091e2-360">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-361">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-361">Storage</span></span>

* <span data-ttu-id="091e2-362">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="091e2-362">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="091e2-363">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="091e2-363">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="091e2-364">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="091e2-364">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="091e2-365">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="091e2-365">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="091e2-366">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-366">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-367">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-367">VM</span></span>

* <span data-ttu-id="091e2-368">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="091e2-368">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="091e2-369">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-369">July 31, 2018</span></span>

<span data-ttu-id="091e2-370">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="091e2-370">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-371">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-371">ACR</span></span>

* <span data-ttu-id="091e2-372">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-372">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="091e2-373">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="091e2-373">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-374">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-374">ACS</span></span>

* <span data-ttu-id="091e2-375">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="091e2-375">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-376">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-376">Batch</span></span>

* <span data-ttu-id="091e2-377">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="091e2-377">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="091e2-378">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-378">Container</span></span>

* <span data-ttu-id="091e2-379">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="091e2-379">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="091e2-380">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-380">Network</span></span>

* <span data-ttu-id="091e2-381">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="091e2-381">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="091e2-382">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-382">Resource</span></span>

* <span data-ttu-id="091e2-383">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="091e2-383">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="091e2-384">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="091e2-384">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="091e2-385">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-385">Role</span></span>

* <span data-ttu-id="091e2-386">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="091e2-386">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="091e2-387">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="091e2-387">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="091e2-388">Search</span><span class="sxs-lookup"><span data-stu-id="091e2-388">Search</span></span>

* <span data-ttu-id="091e2-389">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="091e2-389">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="091e2-390">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="091e2-390">Service Bus</span></span>

* <span data-ttu-id="091e2-391">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="091e2-391">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="091e2-392">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="091e2-392">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="091e2-393">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="091e2-393">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="091e2-394">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="091e2-394">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-395">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-395">Storage</span></span>

* <span data-ttu-id="091e2-396">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="091e2-396">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="091e2-397">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="091e2-397">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-398">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-398">VM</span></span>

* <span data-ttu-id="091e2-399">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="091e2-399">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="091e2-400">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="091e2-400">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="091e2-401">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="091e2-401">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="091e2-402">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="091e2-402">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="091e2-403">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-403">July 18, 2018</span></span>

<span data-ttu-id="091e2-404">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="091e2-404">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="091e2-405">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-405">Core</span></span>

* <span data-ttu-id="091e2-406">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="091e2-406">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="091e2-407">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="091e2-407">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="091e2-408">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-408">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-409">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-409">ACR</span></span>

* <span data-ttu-id="091e2-410">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="091e2-410">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="091e2-411">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="091e2-411">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="091e2-412">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="091e2-412">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="091e2-413">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="091e2-413">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-414">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-414">ACS</span></span>

* <span data-ttu-id="091e2-415">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="091e2-415">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-416">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-416">AppService</span></span>

* <span data-ttu-id="091e2-417">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="091e2-417">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-418">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-418">Batch</span></span>

* <span data-ttu-id="091e2-419">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="091e2-419">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="091e2-420">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="091e2-420">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="091e2-421">Batch AI</span><span class="sxs-lookup"><span data-stu-id="091e2-421">Batch AI</span></span>

* <span data-ttu-id="091e2-422">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="091e2-422">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="091e2-423">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-423">Container</span></span>

* <span data-ttu-id="091e2-424">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="091e2-424">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="091e2-425">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="091e2-425">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="091e2-426">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-426">Network</span></span>

* <span data-ttu-id="091e2-427">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="091e2-427">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="091e2-428">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="091e2-428">Added `network nic wait`</span></span>
* <span data-ttu-id="091e2-429">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="091e2-429">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="091e2-430">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="091e2-430">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="091e2-431">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-431">Resource</span></span>

* <span data-ttu-id="091e2-432">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="091e2-432">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="091e2-433">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="091e2-433">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="091e2-434">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="091e2-434">Added `deployment wait` command</span></span>
* <span data-ttu-id="091e2-435">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="091e2-435">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-436">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-436">SQL</span></span>

* <span data-ttu-id="091e2-437">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="091e2-437">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="091e2-438">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="091e2-438">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="091e2-439">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="091e2-439">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-440">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-440">Storage</span></span>

* <span data-ttu-id="091e2-441">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="091e2-441">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-442">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-442">VM</span></span>

* <span data-ttu-id="091e2-443">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="091e2-443">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="091e2-444">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="091e2-444">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="091e2-445">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="091e2-445">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="091e2-446">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-446">July 3, 2018</span></span>

<span data-ttu-id="091e2-447">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="091e2-447">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="091e2-448">AKS</span><span class="sxs-lookup"><span data-stu-id="091e2-448">AKS</span></span>

* <span data-ttu-id="091e2-449">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="091e2-449">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="091e2-450">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-450">July 3, 2018</span></span>

<span data-ttu-id="091e2-451">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="091e2-451">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="091e2-452">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-452">Core</span></span>

* <span data-ttu-id="091e2-453">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="091e2-453">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-454">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-454">ACR</span></span>

* <span data-ttu-id="091e2-455">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="091e2-455">Added polling build status</span></span>
* <span data-ttu-id="091e2-456">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="091e2-456">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="091e2-457">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="091e2-457">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-458">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-458">ACS</span></span>

* <span data-ttu-id="091e2-459">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="091e2-459">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="091e2-460">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="091e2-460">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="091e2-461">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="091e2-461">Updated options for `aks browse` command.</span></span> <span data-ttu-id="091e2-462">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="091e2-462">Added `--listen-port` support</span></span>
* <span data-ttu-id="091e2-463">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="091e2-463">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="091e2-464">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="091e2-464">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="091e2-465">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="091e2-465">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-466">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-466">AppService</span></span>

* <span data-ttu-id="091e2-467">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="091e2-467">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="091e2-468">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="091e2-468">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="091e2-469">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="091e2-469">Backup</span></span>

* <span data-ttu-id="091e2-470">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="091e2-470">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="091e2-471">BatchAI</span><span class="sxs-lookup"><span data-stu-id="091e2-471">BatchAI</span></span>

* <span data-ttu-id="091e2-472">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="091e2-472">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="091e2-473">Nube</span><span class="sxs-lookup"><span data-stu-id="091e2-473">Cloud</span></span>

* <span data-ttu-id="091e2-474">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="091e2-474">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="091e2-475">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-475">Container</span></span>

* <span data-ttu-id="091e2-476">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="091e2-476">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="091e2-477">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="091e2-477">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="091e2-478">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="091e2-478">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-479">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-479">Extension</span></span>

* <span data-ttu-id="091e2-480">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="091e2-480">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="091e2-481">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-481">Network</span></span>

* <span data-ttu-id="091e2-482">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="091e2-482">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="091e2-483">Rdbms</span><span class="sxs-lookup"><span data-stu-id="091e2-483">Rdbms</span></span>

* <span data-ttu-id="091e2-484">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="091e2-484">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-485">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-485">Resource</span></span>

* <span data-ttu-id="091e2-486">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="091e2-486">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-487">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-487">VM</span></span>

* <span data-ttu-id="091e2-488">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="091e2-488">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="091e2-489">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-489">June 25, 2018</span></span>

<span data-ttu-id="091e2-490">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="091e2-490">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="091e2-491">CLI</span><span class="sxs-lookup"><span data-stu-id="091e2-491">CLI</span></span>

* <span data-ttu-id="091e2-492">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-492">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="091e2-493">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-493">June 19, 2018</span></span>

<span data-ttu-id="091e2-494">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="091e2-494">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="091e2-495">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-495">Core</span></span>

* <span data-ttu-id="091e2-496">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-496">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-497">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-497">ACR</span></span>

* <span data-ttu-id="091e2-498">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="091e2-498">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="091e2-499">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="091e2-499">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-500">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-500">ACS</span></span>

* <span data-ttu-id="091e2-501">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="091e2-501">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="091e2-502">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="091e2-502">Added `--update` support</span></span>
* <span data-ttu-id="091e2-503">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="091e2-503">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="091e2-504">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="091e2-504">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="091e2-505">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="091e2-505">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="091e2-506">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="091e2-506">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="091e2-507">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="091e2-507">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="091e2-508">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="091e2-508">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-509">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-509">AppService</span></span>

* <span data-ttu-id="091e2-510">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="091e2-510">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="091e2-511">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="091e2-511">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-512">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-512">Batch</span></span>

* <span data-ttu-id="091e2-513">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="091e2-513">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="091e2-514">Batch AI</span><span class="sxs-lookup"><span data-stu-id="091e2-514">Batch AI</span></span>

* <span data-ttu-id="091e2-515">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="091e2-515">Added support for workspaces.</span></span> <span data-ttu-id="091e2-516">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="091e2-516">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="091e2-517">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="091e2-517">Added support for experiments.</span></span> <span data-ttu-id="091e2-518">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="091e2-518">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="091e2-519">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="091e2-519">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="091e2-520">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="091e2-520">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="091e2-521">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="091e2-521">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="091e2-522">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="091e2-522">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="091e2-523">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="091e2-523">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="091e2-524">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="091e2-524">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="091e2-525">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-525">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="091e2-526">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="091e2-526">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="091e2-527">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-527">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="091e2-528">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="091e2-528">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="091e2-529">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="091e2-529">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="091e2-530">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="091e2-530">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="091e2-531">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-531">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="091e2-532">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="091e2-532">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="091e2-533">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="091e2-533">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="091e2-534">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="091e2-534">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="091e2-535">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="091e2-535">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="091e2-536">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="091e2-536">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="091e2-537">Mapas</span><span class="sxs-lookup"><span data-stu-id="091e2-537">Maps</span></span>

* <span data-ttu-id="091e2-538">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="091e2-538">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="091e2-539">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-539">Network</span></span>

* <span data-ttu-id="091e2-540">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="091e2-540">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="091e2-541">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="091e2-541">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="091e2-542">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="091e2-542">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="091e2-543">Reservations</span><span class="sxs-lookup"><span data-stu-id="091e2-543">Reservations</span></span>

* <span data-ttu-id="091e2-544">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-544">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="091e2-545">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-545">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="091e2-546">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="091e2-546">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="091e2-547">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="091e2-547">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="091e2-548">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="091e2-548">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="091e2-549">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-549">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="091e2-550">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-550">Role</span></span>

* <span data-ttu-id="091e2-551">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="091e2-551">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-552">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-552">SQL</span></span>

* <span data-ttu-id="091e2-553">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="091e2-553">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-554">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-554">Storage</span></span>

* <span data-ttu-id="091e2-555">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="091e2-555">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-556">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-556">VM</span></span>

* <span data-ttu-id="091e2-557">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="091e2-557">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="091e2-558">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="091e2-558">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="091e2-559">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="091e2-559">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="091e2-560">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-560">June 13, 2018</span></span>

<span data-ttu-id="091e2-561">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="091e2-561">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="091e2-562">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-562">Core</span></span>

* <span data-ttu-id="091e2-563">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="091e2-563">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="091e2-564">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-564">June 13, 2018</span></span>

<span data-ttu-id="091e2-565">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="091e2-565">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="091e2-566">AKS</span><span class="sxs-lookup"><span data-stu-id="091e2-566">AKS</span></span>

* <span data-ttu-id="091e2-567">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="091e2-567">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="091e2-568">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="091e2-568">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="091e2-569">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="091e2-569">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="091e2-570">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="091e2-570">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="091e2-571">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="091e2-571">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-572">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-572">AppService</span></span>

* <span data-ttu-id="091e2-573">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="091e2-573">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="091e2-574">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-574">June 5, 2018</span></span>

<span data-ttu-id="091e2-575">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="091e2-575">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-576">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-576">Interactive</span></span>

* <span data-ttu-id="091e2-577">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="091e2-577">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="091e2-578">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-578">June 5, 2018</span></span>

<span data-ttu-id="091e2-579">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="091e2-579">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="091e2-580">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-580">Core</span></span>

* <span data-ttu-id="091e2-581">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="091e2-581">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="091e2-582">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="091e2-582">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-583">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-583">ACR</span></span>

* <span data-ttu-id="091e2-584">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="091e2-584">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="091e2-585">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="091e2-585">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="091e2-586">AKS</span><span class="sxs-lookup"><span data-stu-id="091e2-586">AKS</span></span>

* <span data-ttu-id="091e2-587">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="091e2-587">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-588">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-588">Batch</span></span>

* <span data-ttu-id="091e2-589">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="091e2-589">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-590">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-590">IOT</span></span>

* <span data-ttu-id="091e2-591">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="091e2-591">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="091e2-592">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-592">Network</span></span>

* <span data-ttu-id="091e2-593">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="091e2-593">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="091e2-594">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="091e2-594">Policy Insights</span></span>

* <span data-ttu-id="091e2-595">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="091e2-595">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="091e2-596">ARM</span><span class="sxs-lookup"><span data-stu-id="091e2-596">ARM</span></span>

* <span data-ttu-id="091e2-597">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="091e2-597">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-598">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-598">SQL</span></span>

* <span data-ttu-id="091e2-599">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="091e2-599">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="091e2-600">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="091e2-600">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="091e2-601">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-601">Storage</span></span>

* <span data-ttu-id="091e2-602">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="091e2-602">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-603">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-603">VM</span></span>

* <span data-ttu-id="091e2-604">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="091e2-604">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="091e2-605">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="091e2-605">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="091e2-606">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="091e2-606">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="091e2-607">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-607">May 22, 2018</span></span>

<span data-ttu-id="091e2-608">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="091e2-608">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="091e2-609">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-609">Core</span></span>

* <span data-ttu-id="091e2-610">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="091e2-610">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-611">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-611">ACS</span></span>

* <span data-ttu-id="091e2-612">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="091e2-612">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="091e2-613">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="091e2-613">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-614">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-614">AppService</span></span>

* <span data-ttu-id="091e2-615">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="091e2-615">Improved generic update commands</span></span>
* <span data-ttu-id="091e2-616">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="091e2-616">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="091e2-617">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-617">Container</span></span>

* <span data-ttu-id="091e2-618">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="091e2-618">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="091e2-619">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-619">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-620">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-620">Extension</span></span>

* <span data-ttu-id="091e2-621">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="091e2-621">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-622">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-622">Interactive</span></span>

* <span data-ttu-id="091e2-623">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="091e2-623">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="091e2-624">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="091e2-624">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-625">KeyVault</span><span class="sxs-lookup"><span data-stu-id="091e2-625">KeyVault</span></span>

* <span data-ttu-id="091e2-626">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="091e2-626">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="091e2-627">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-627">Network</span></span>

* <span data-ttu-id="091e2-628">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="091e2-628">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="091e2-629">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="091e2-629">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-630">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-630">SQL</span></span>

* <span data-ttu-id="091e2-631">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="091e2-631">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="091e2-632">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="091e2-632">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="091e2-633">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="091e2-633">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="091e2-634">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="091e2-634">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="091e2-635">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="091e2-635">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="091e2-636">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="091e2-636">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="091e2-637">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="091e2-637">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="091e2-638">`edition`.</span><span class="sxs-lookup"><span data-stu-id="091e2-638">`edition`.</span></span> <span data-ttu-id="091e2-639">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="091e2-639">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="091e2-640">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="091e2-640">`elasticPoolName`.</span></span> <span data-ttu-id="091e2-641">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="091e2-641">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="091e2-642">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="091e2-642">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="091e2-643">`edition`.</span><span class="sxs-lookup"><span data-stu-id="091e2-643">`edition`.</span></span> <span data-ttu-id="091e2-644">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="091e2-644">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="091e2-645">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="091e2-645">`dtu`.</span></span> <span data-ttu-id="091e2-646">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="091e2-646">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="091e2-647">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="091e2-647">`databaseDtuMin`.</span></span> <span data-ttu-id="091e2-648">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="091e2-648">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="091e2-649">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="091e2-649">`databaseDtuMax`.</span></span> <span data-ttu-id="091e2-650">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="091e2-650">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="091e2-651">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="091e2-651">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="091e2-652">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="091e2-652">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-653">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-653">Storage</span></span>

* <span data-ttu-id="091e2-654">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="091e2-654">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="091e2-655">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="091e2-655">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-656">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-656">VM</span></span>

* <span data-ttu-id="091e2-657">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-657">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="091e2-658">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="091e2-658">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="091e2-659">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="091e2-659">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="091e2-660">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="091e2-660">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="091e2-661">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="091e2-661">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="091e2-662">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-662">May 7, 2018</span></span>

<span data-ttu-id="091e2-663">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="091e2-663">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="091e2-664">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-664">Core</span></span>

* <span data-ttu-id="091e2-665">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="091e2-665">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="091e2-666">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="091e2-666">Added limited support for positional arguments</span></span>
* <span data-ttu-id="091e2-667">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="091e2-667">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="091e2-668">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="091e2-668">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="091e2-669">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="091e2-669">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="091e2-670">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="091e2-670">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="091e2-671">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-671">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="091e2-672">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="091e2-672">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="091e2-673">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-673">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-674">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-674">ACR</span></span>

* <span data-ttu-id="091e2-675">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="091e2-675">Added ACR Build commands</span></span>
* <span data-ttu-id="091e2-676">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="091e2-676">Improved resource not found error messages</span></span>
* <span data-ttu-id="091e2-677">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="091e2-677">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="091e2-678">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="091e2-678">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="091e2-679">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="091e2-679">Improved repository commands error messages</span></span>
* <span data-ttu-id="091e2-680">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="091e2-680">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-681">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-681">ACS</span></span>

* <span data-ttu-id="091e2-682">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="091e2-682">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="091e2-683">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="091e2-683">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="091e2-684">AMS</span><span class="sxs-lookup"><span data-stu-id="091e2-684">AMS</span></span>

* <span data-ttu-id="091e2-685">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="091e2-685">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-686">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-686">Appservice</span></span>

* <span data-ttu-id="091e2-687">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="091e2-687">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="091e2-688">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="091e2-688">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="091e2-689">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="091e2-689">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="091e2-690">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-690">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="091e2-691">Batch AI</span><span class="sxs-lookup"><span data-stu-id="091e2-691">Batch AI</span></span>

* <span data-ttu-id="091e2-692">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="091e2-692">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="091e2-693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="091e2-693">Cognitive Services</span></span>

* <span data-ttu-id="091e2-694">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="091e2-694">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="091e2-695">Consumo</span><span class="sxs-lookup"><span data-stu-id="091e2-695">Consumption</span></span>

* <span data-ttu-id="091e2-696">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="091e2-696">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="091e2-697">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-697">Container</span></span>

* <span data-ttu-id="091e2-698">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="091e2-698">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="091e2-699">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="091e2-699">Cosmos DB</span></span>

* <span data-ttu-id="091e2-700">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="091e2-700">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="091e2-701">DMS</span><span class="sxs-lookup"><span data-stu-id="091e2-701">DMS</span></span>

* <span data-ttu-id="091e2-702">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-702">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-703">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-703">Extension</span></span>

* <span data-ttu-id="091e2-704">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="091e2-704">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-705">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-705">Interactive</span></span>

* <span data-ttu-id="091e2-706">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="091e2-706">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="091e2-707">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="091e2-707">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="091e2-708">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="091e2-708">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="091e2-709">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-709">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="091e2-710">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-710">Lab</span></span>

* <span data-ttu-id="091e2-711">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="091e2-711">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="091e2-712">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-712">Network</span></span>

* <span data-ttu-id="091e2-713">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="091e2-713">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="091e2-714">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-714">Profile</span></span>

* <span data-ttu-id="091e2-715">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="091e2-715">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="091e2-716">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="091e2-716">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="091e2-717">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="091e2-717">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="091e2-718">Redis</span><span class="sxs-lookup"><span data-stu-id="091e2-718">Redis</span></span>

* <span data-ttu-id="091e2-719">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="091e2-719">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="091e2-720">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="091e2-720">Deprecated `redis list-all`.</span></span> <span data-ttu-id="091e2-721">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="091e2-721">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="091e2-722">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="091e2-722">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="091e2-723">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-723">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="091e2-724">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-724">Role</span></span>

* <span data-ttu-id="091e2-725">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="091e2-725">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-726">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-726">Storage</span></span>

* <span data-ttu-id="091e2-727">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="091e2-727">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="091e2-728">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="091e2-728">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="091e2-729">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="091e2-729">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="091e2-730">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="091e2-730">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="091e2-731">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="091e2-731">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-732">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-732">VM</span></span>

* <span data-ttu-id="091e2-733">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="091e2-733">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="091e2-734">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="091e2-734">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="091e2-735">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="091e2-735">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="091e2-736">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="091e2-736">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="091e2-737">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="091e2-737">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="091e2-738">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="091e2-738">Added write accelerator support</span></span>
* <span data-ttu-id="091e2-739">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="091e2-739">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="091e2-740">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="091e2-740">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="091e2-741">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="091e2-741">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="091e2-742">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-742">April 10, 2018</span></span>

<span data-ttu-id="091e2-743">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="091e2-743">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-744">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-744">ACR</span></span>

* <span data-ttu-id="091e2-745">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="091e2-745">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-746">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-746">ACS</span></span>

* <span data-ttu-id="091e2-747">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="091e2-747">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-748">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-748">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="091e2-750">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="091e2-750">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="091e2-751">BatchAI</span><span class="sxs-lookup"><span data-stu-id="091e2-751">BatchAI</span></span>

* <span data-ttu-id="091e2-752">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="091e2-752">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="091e2-753">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="091e2-753">Job level mounting</span></span>
  - <span data-ttu-id="091e2-754">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="091e2-754">Environment variables with secret values</span></span>
  - <span data-ttu-id="091e2-755">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="091e2-755">Performance counters settings</span></span>
  - <span data-ttu-id="091e2-756">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="091e2-756">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="091e2-757">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="091e2-757">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="091e2-758">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="091e2-758">Usage and limits reporting</span></span>
  - <span data-ttu-id="091e2-759">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="091e2-759">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="091e2-760">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="091e2-760">Support for custom images</span></span>
  - <span data-ttu-id="091e2-761">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="091e2-761">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="091e2-762">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="091e2-762">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="091e2-763">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="091e2-763">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="091e2-764">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="091e2-764">National clouds are supported</span></span>
* <span data-ttu-id="091e2-765">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="091e2-765">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="091e2-766">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="091e2-766">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="091e2-767">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="091e2-767">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="091e2-768">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="091e2-768">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="091e2-769">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="091e2-769">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="091e2-770">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="091e2-770">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="091e2-771">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-771">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="091e2-772">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="091e2-772">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="091e2-773">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="091e2-773">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="091e2-774">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="091e2-774">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="091e2-775">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-775">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="091e2-776">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="091e2-776">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="091e2-777">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="091e2-777">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="091e2-778">Facturación</span><span class="sxs-lookup"><span data-stu-id="091e2-778">Billing</span></span>

* <span data-ttu-id="091e2-779">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="091e2-779">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="091e2-780">Consumo</span><span class="sxs-lookup"><span data-stu-id="091e2-780">Consumption</span></span>

* <span data-ttu-id="091e2-781">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="091e2-781">Added `marketplace` commands</span></span>
* <span data-ttu-id="091e2-782">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="091e2-782">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="091e2-783">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="091e2-783">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="091e2-784">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="091e2-784">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="091e2-785">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="091e2-785">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="091e2-786">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="091e2-786">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="091e2-787">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-787">Container</span></span>

* <span data-ttu-id="091e2-788">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="091e2-788">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="091e2-789">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="091e2-789">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-790">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-790">Extension</span></span>

* <span data-ttu-id="091e2-791">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="091e2-791">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-792">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-792">Interactive</span></span>

* <span data-ttu-id="091e2-793">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="091e2-793">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="091e2-794">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-794">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="091e2-795">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="091e2-795">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="091e2-796">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-796">Network</span></span>

* <span data-ttu-id="091e2-797">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="091e2-797">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="091e2-798">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="091e2-798">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="091e2-799">4910</span><span class="sxs-lookup"><span data-stu-id="091e2-799">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="091e2-800">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="091e2-800">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="091e2-801">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="091e2-801">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="091e2-802">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-802">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="091e2-803">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-803">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="091e2-804">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="091e2-804">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-805">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-805">Profile</span></span>

* <span data-ttu-id="091e2-806">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="091e2-806">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="091e2-807">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="091e2-807">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="091e2-808">RDBMS</span><span class="sxs-lookup"><span data-stu-id="091e2-808">RDBMS</span></span>

* <span data-ttu-id="091e2-809">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="091e2-809">Added `georestore` command</span></span>
* <span data-ttu-id="091e2-810">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="091e2-810">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-811">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-811">Resource</span></span>

* <span data-ttu-id="091e2-812">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-812">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="091e2-813">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="091e2-813">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-814">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-814">SQL</span></span>

* <span data-ttu-id="091e2-815">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="091e2-815">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-816">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-816">Storage</span></span>

* <span data-ttu-id="091e2-817">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="091e2-817">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-818">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-818">VM</span></span>

* <span data-ttu-id="091e2-819">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="091e2-819">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="091e2-820">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="091e2-820">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="091e2-822">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="091e2-822">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="091e2-823">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="091e2-823">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="091e2-824">5718</span><span class="sxs-lookup"><span data-stu-id="091e2-824">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="091e2-825">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="091e2-825">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="091e2-826">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-826">March 27, 2018</span></span>

<span data-ttu-id="091e2-827">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="091e2-827">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="091e2-828">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-828">Core</span></span>

* <span data-ttu-id="091e2-829">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="091e2-829">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-830">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-830">ACS</span></span>

* <span data-ttu-id="091e2-831">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="091e2-831">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-832">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-832">Appservice</span></span>

* <span data-ttu-id="091e2-833">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="091e2-833">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="091e2-834">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="091e2-834">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="091e2-835">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="091e2-835">Backup</span></span>

* <span data-ttu-id="091e2-836">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="091e2-836">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="091e2-837">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-837">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="091e2-838">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="091e2-838">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="091e2-839">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="091e2-839">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="091e2-840">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-840">Container</span></span>

* <span data-ttu-id="091e2-841">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="091e2-841">Added `container exec` command.</span></span> <span data-ttu-id="091e2-842">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="091e2-842">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="091e2-843">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-843">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-844">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-844">Extension</span></span>

* <span data-ttu-id="091e2-845">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="091e2-845">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="091e2-846">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="091e2-846">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="091e2-847">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="091e2-847">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-848">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-848">Interactive</span></span>

* <span data-ttu-id="091e2-849">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-849">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="091e2-850">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="091e2-850">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="091e2-851">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-851">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="091e2-852">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="091e2-852">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="091e2-853">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-853">Lab</span></span>

* <span data-ttu-id="091e2-854">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="091e2-854">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-855">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-855">Monitor</span></span>

* <span data-ttu-id="091e2-856">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="091e2-856">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="091e2-857">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="091e2-857">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="091e2-858">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="091e2-858">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="091e2-859">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-859">Network</span></span>

* <span data-ttu-id="091e2-860">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="091e2-860">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-861">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-861">Profile</span></span>

* <span data-ttu-id="091e2-862">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="091e2-862">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="091e2-863">RDBMS</span><span class="sxs-lookup"><span data-stu-id="091e2-863">RDBMS</span></span>

* <span data-ttu-id="091e2-864">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="091e2-864">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-865">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-865">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="091e2-867">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-867">Role</span></span>

* <span data-ttu-id="091e2-868">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="091e2-868">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="091e2-869">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="091e2-869">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="091e2-870">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="091e2-870">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="091e2-871">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="091e2-871">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="091e2-872">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="091e2-872">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-873">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-873">Storage</span></span>

* <span data-ttu-id="091e2-874">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="091e2-874">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="091e2-875">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="091e2-875">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-876">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-876">VM</span></span>

* <span data-ttu-id="091e2-877">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="091e2-877">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="091e2-878">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="091e2-878">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="091e2-879">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="091e2-879">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="091e2-880">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="091e2-880">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="091e2-881">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-881">March 13, 2018</span></span>

<span data-ttu-id="091e2-882">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="091e2-882">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-883">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-883">ACR</span></span>

* <span data-ttu-id="091e2-884">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="091e2-884">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="091e2-885">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-885">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="091e2-886">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="091e2-886">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-887">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-887">ACS</span></span>

* <span data-ttu-id="091e2-888">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="091e2-888">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="091e2-889">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="091e2-889">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="091e2-890">Advisor</span><span class="sxs-lookup"><span data-stu-id="091e2-890">Advisor</span></span>

* <span data-ttu-id="091e2-891">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="091e2-891">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="091e2-892">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="091e2-892">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="091e2-893">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="091e2-893">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="091e2-894">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="091e2-894">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="091e2-895">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-895">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-896">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-896">Appservice</span></span>

* <span data-ttu-id="091e2-897">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-897">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="091e2-898">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="091e2-898">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="091e2-899">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="091e2-899">Eventhubs</span></span>

* <span data-ttu-id="091e2-900">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="091e2-900">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-901">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-901">Extension</span></span>

* <span data-ttu-id="091e2-902">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="091e2-902">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-903">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-903">Interactive</span></span>

* <span data-ttu-id="091e2-904">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="091e2-904">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="091e2-905">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="091e2-905">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="091e2-906">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="091e2-906">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="091e2-907">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="091e2-907">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-908">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-908">Monitor</span></span>

* <span data-ttu-id="091e2-909">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-909">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="091e2-910">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="091e2-910">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="091e2-911">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="091e2-911">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="091e2-912">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="091e2-912">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="091e2-913">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-913">Network</span></span>

* <span data-ttu-id="091e2-914">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="091e2-914">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="091e2-915">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="091e2-915">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="091e2-916">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="091e2-916">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="091e2-917">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="091e2-917">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-918">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-918">Profile</span></span>

* <span data-ttu-id="091e2-919">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-919">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="091e2-920">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="091e2-920">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="091e2-921">RDBMS</span><span class="sxs-lookup"><span data-stu-id="091e2-921">RDBMS</span></span>

* <span data-ttu-id="091e2-922">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="091e2-922">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="091e2-923">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="091e2-923">Service Bus</span></span>

* <span data-ttu-id="091e2-924">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="091e2-924">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-925">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-925">Storage</span></span>

* <span data-ttu-id="091e2-926">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="091e2-926">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="091e2-927">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="091e2-927">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-928">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-928">VM</span></span>

* <span data-ttu-id="091e2-929">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="091e2-929">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="091e2-930">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-930">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="091e2-931">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-931">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="091e2-932">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="091e2-932">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="091e2-933">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-933">February 27, 2018</span></span>

<span data-ttu-id="091e2-934">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="091e2-934">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="091e2-935">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-935">Core</span></span>

* <span data-ttu-id="091e2-936">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="091e2-936">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="091e2-937">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="091e2-937">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="091e2-938">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="091e2-938">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-939">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-939">ACS</span></span>

* <span data-ttu-id="091e2-940">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="091e2-940">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="091e2-941">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="091e2-941">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="091e2-942">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="091e2-942">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="091e2-943">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="091e2-943">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-944">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-944">Appservice</span></span>

* <span data-ttu-id="091e2-945">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="091e2-945">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="091e2-946">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="091e2-946">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="091e2-947">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="091e2-947">Cognitive Services</span></span>

* <span data-ttu-id="091e2-948">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="091e2-948">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="091e2-949">Consumo</span><span class="sxs-lookup"><span data-stu-id="091e2-949">Consumption</span></span>

* <span data-ttu-id="091e2-950">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="091e2-950">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="091e2-951">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="091e2-951">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="091e2-952">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-952">Container</span></span>

* <span data-ttu-id="091e2-953">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="091e2-953">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="091e2-954">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-954">Network</span></span>

* <span data-ttu-id="091e2-955">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="091e2-955">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-956">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-956">Resource</span></span>

* <span data-ttu-id="091e2-957">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="091e2-957">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="091e2-958">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-958">Role</span></span>

* <span data-ttu-id="091e2-959">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="091e2-959">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-960">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-960">SQL</span></span>

* <span data-ttu-id="091e2-961">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="091e2-961">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-962">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-962">Storage</span></span>

* <span data-ttu-id="091e2-963">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="091e2-963">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-964">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-964">VM</span></span>

* <span data-ttu-id="091e2-965">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="091e2-965">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="091e2-966">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-966">February 13, 2018</span></span>

<span data-ttu-id="091e2-967">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="091e2-967">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="091e2-968">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-968">Core</span></span>

* <span data-ttu-id="091e2-969">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="091e2-969">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-970">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-970">ACS</span></span>

* <span data-ttu-id="091e2-971">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="091e2-971">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="091e2-972">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="091e2-972">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="091e2-973">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="091e2-973">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="091e2-974">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="091e2-974">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="091e2-975">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="091e2-975">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="091e2-976">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="091e2-976">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="091e2-977">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="091e2-977">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="091e2-978">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="091e2-978">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-979">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-979">Appservice</span></span>

* <span data-ttu-id="091e2-980">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="091e2-980">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="091e2-981">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="091e2-981">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="091e2-982">CDN</span><span class="sxs-lookup"><span data-stu-id="091e2-982">CDN</span></span>

* <span data-ttu-id="091e2-983">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="091e2-983">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="091e2-984">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-984">Container</span></span>

* <span data-ttu-id="091e2-985">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="091e2-985">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="091e2-986">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-986">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="091e2-987">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="091e2-987">CosmosDB</span></span>

* <span data-ttu-id="091e2-988">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="091e2-988">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-989">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-989">Extension</span></span>

* <span data-ttu-id="091e2-990">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-990">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="091e2-991">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-991">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="091e2-992">Comentarios</span><span class="sxs-lookup"><span data-stu-id="091e2-992">Feedback</span></span>

* <span data-ttu-id="091e2-993">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="091e2-993">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-994">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-994">Interactive</span></span>

* <span data-ttu-id="091e2-995">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="091e2-995">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="091e2-996">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="091e2-996">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-997">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-997">IoT</span></span>

* <span data-ttu-id="091e2-998">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="091e2-998">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="091e2-999">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="091e2-999">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="091e2-1000">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1000">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="091e2-1001">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="091e2-1001">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-1002">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-1002">Monitor</span></span>

* <span data-ttu-id="091e2-1003">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1003">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1004">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1004">Network</span></span>

* <span data-ttu-id="091e2-1005">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="091e2-1005">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="091e2-1006">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-1006">Profile</span></span>

* <span data-ttu-id="091e2-1007">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="091e2-1007">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1008">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1008">Resource</span></span>

* <span data-ttu-id="091e2-1009">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="091e2-1009">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="091e2-1010">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-1010">Role</span></span>

* <span data-ttu-id="091e2-1011">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1011">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1012">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-1012">SQL</span></span>

* <span data-ttu-id="091e2-1013">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1013">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="091e2-1014">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1014">Added `sql db rename`</span></span>
* <span data-ttu-id="091e2-1015">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="091e2-1015">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1016">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1016">Storage</span></span>

* <span data-ttu-id="091e2-1017">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="091e2-1017">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1018">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1018">VM</span></span>

* <span data-ttu-id="091e2-1019">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="091e2-1019">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="091e2-1020">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="091e2-1020">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="091e2-1021">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="091e2-1021">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="091e2-1022">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-1022">January 31, 2018</span></span>

<span data-ttu-id="091e2-1023">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="091e2-1023">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="091e2-1024">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1024">Core</span></span>

* <span data-ttu-id="091e2-1025">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="091e2-1025">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="091e2-1026">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="091e2-1026">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="091e2-1027">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="091e2-1027">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="091e2-1028">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="091e2-1028">Use `--verbose` to see</span></span>
* <span data-ttu-id="091e2-1029">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="091e2-1029">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1030">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1030">ACS</span></span>

* <span data-ttu-id="091e2-1031">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="091e2-1031">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="091e2-1032">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="091e2-1032">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1033">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1033">Appservice</span></span>

* <span data-ttu-id="091e2-1034">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="091e2-1034">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="091e2-1035">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="091e2-1035">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="091e2-1036">CDN</span><span class="sxs-lookup"><span data-stu-id="091e2-1036">CDN</span></span>

* <span data-ttu-id="091e2-1037">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1037">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="091e2-1038">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="091e2-1038">CosmosDB</span></span>

* <span data-ttu-id="091e2-1039">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="091e2-1039">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-1040">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-1040">Interactive</span></span>

* <span data-ttu-id="091e2-1041">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="091e2-1041">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1042">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1042">Network</span></span>

* <span data-ttu-id="091e2-1043">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1043">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="091e2-1044">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="091e2-1044">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="091e2-1045">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1045">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="091e2-1046">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1046">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="091e2-1047">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="091e2-1047">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="091e2-1048">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="091e2-1048">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="091e2-1049">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="091e2-1049">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="091e2-1050">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="091e2-1050">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="091e2-1051">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="091e2-1051">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="091e2-1052">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="091e2-1052">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-1053">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-1053">Profile</span></span>

* <span data-ttu-id="091e2-1054">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="091e2-1054">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1055">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1055">Resource</span></span>

* <span data-ttu-id="091e2-1056">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="091e2-1056">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1057">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1057">Storage</span></span>

* <span data-ttu-id="091e2-1058">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="091e2-1058">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="091e2-1059">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="091e2-1059">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="091e2-1060">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="091e2-1060">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="091e2-1061">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1061">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="091e2-1062">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="091e2-1062">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1063">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1063">VM</span></span>

* <span data-ttu-id="091e2-1064">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="091e2-1064">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="091e2-1065">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="091e2-1065">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="091e2-1066">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="091e2-1066">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="091e2-1067">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1067">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="091e2-1068">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="091e2-1068">January 17, 2018</span></span>

<span data-ttu-id="091e2-1069">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="091e2-1069">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-1070">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-1070">ACR</span></span>

* <span data-ttu-id="091e2-1071">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="091e2-1071">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="091e2-1072">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="091e2-1072">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1073">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1073">ACS</span></span>

* <span data-ttu-id="091e2-1074">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="091e2-1074">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="091e2-1075">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="091e2-1075">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1076">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1076">Appservice</span></span>

* <span data-ttu-id="091e2-1077">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="091e2-1077">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="091e2-1078">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="091e2-1078">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="091e2-1079">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="091e2-1079">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="091e2-1080">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="091e2-1080">Backup</span></span>

* <span data-ttu-id="091e2-1081">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="091e2-1081">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="091e2-1082">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="091e2-1082">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="091e2-1083">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="091e2-1083">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="091e2-1084">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="091e2-1084">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="091e2-1085">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="091e2-1085">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-1086">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-1086">Batch</span></span>

* <span data-ttu-id="091e2-1087">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="091e2-1087">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="091e2-1088">Nube</span><span class="sxs-lookup"><span data-stu-id="091e2-1088">Cloud</span></span>

* <span data-ttu-id="091e2-1089">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="091e2-1089">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="091e2-1090">Consumo</span><span class="sxs-lookup"><span data-stu-id="091e2-1090">Consumption</span></span>

* <span data-ttu-id="091e2-1091">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="091e2-1091">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="091e2-1092">Event Grid</span><span class="sxs-lookup"><span data-stu-id="091e2-1092">Event Grid</span></span>

* <span data-ttu-id="091e2-1093">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="091e2-1093">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="091e2-1094">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="091e2-1094">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="091e2-1095">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1095">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="091e2-1096">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="091e2-1096">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="091e2-1097">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1097">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="091e2-1098">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1098">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="091e2-1099">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="091e2-1099">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="091e2-1100">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="091e2-1100">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-1101">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-1101">Interactive</span></span>

* <span data-ttu-id="091e2-1102">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="091e2-1102">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="091e2-1103">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="091e2-1103">Fixed errors on startup</span></span>
* <span data-ttu-id="091e2-1104">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="091e2-1104">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-1105">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-1105">IoT</span></span>

* <span data-ttu-id="091e2-1106">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="091e2-1106">Added support for device provisioning service</span></span>
* <span data-ttu-id="091e2-1107">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-1107">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="091e2-1108">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-1108">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-1109">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-1109">Monitor</span></span>

* <span data-ttu-id="091e2-1110">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="091e2-1110">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="091e2-1111">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1111">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="091e2-1112">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="091e2-1112">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1113">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1113">Network</span></span>

* <span data-ttu-id="091e2-1114">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1114">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="091e2-1115">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1115">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-1116">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-1116">Profile</span></span>

* <span data-ttu-id="091e2-1117">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="091e2-1117">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="091e2-1118">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-1118">Role</span></span>

* <span data-ttu-id="091e2-1119">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="091e2-1119">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="091e2-1120">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="091e2-1120">Service Fabric</span></span>

* <span data-ttu-id="091e2-1121">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="091e2-1121">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="091e2-1122">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="091e2-1122">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1123">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1123">VM</span></span>

* <span data-ttu-id="091e2-1124">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="091e2-1124">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="091e2-1125">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="091e2-1125">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="091e2-1126">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="091e2-1126">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="091e2-1127">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="091e2-1127">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="091e2-1128">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="091e2-1128">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="091e2-1129">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1129">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="091e2-1130">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1130">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="091e2-1131">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="091e2-1131">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="091e2-1132">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1132">December 19, 2017</span></span>

<span data-ttu-id="091e2-1133">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="091e2-1133">Version 2.0.23</span></span>

* <span data-ttu-id="091e2-1134">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="091e2-1134">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="091e2-1135">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-1135">Container</span></span>

* <span data-ttu-id="091e2-1136">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-1136">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1137">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1137">Network</span></span>

* <span data-ttu-id="091e2-1138">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1138">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="091e2-1139">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1139">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1140">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1140">Storage</span></span>

* <span data-ttu-id="091e2-1141">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="091e2-1141">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1142">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1142">VM</span></span>

* <span data-ttu-id="091e2-1143">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="091e2-1143">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="091e2-1144">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1144">December 5, 2017</span></span>

<span data-ttu-id="091e2-1145">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="091e2-1145">Version 2.0.22</span></span>

* <span data-ttu-id="091e2-1146">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1146">Removed `az component` commands.</span></span> <span data-ttu-id="091e2-1147">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="091e2-1147">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="091e2-1148">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1148">Core</span></span>
* <span data-ttu-id="091e2-1149">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="091e2-1149">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="091e2-1150">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="091e2-1150">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1151">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1151">ACS</span></span>

* <span data-ttu-id="091e2-1152">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="091e2-1152">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="091e2-1153">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1153">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="091e2-1154">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="091e2-1154">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="091e2-1155">Advisor</span><span class="sxs-lookup"><span data-stu-id="091e2-1155">Advisor</span></span>

* <span data-ttu-id="091e2-1156">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="091e2-1156">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1157">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1157">Appservice</span></span>

* <span data-ttu-id="091e2-1158">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="091e2-1158">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="091e2-1159">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="091e2-1159">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="091e2-1160">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="091e2-1160">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="091e2-1161">Consumo</span><span class="sxs-lookup"><span data-stu-id="091e2-1161">Consumption</span></span>

* <span data-ttu-id="091e2-1162">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="091e2-1162">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="091e2-1163">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-1163">Container</span></span>

* <span data-ttu-id="091e2-1164">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="091e2-1164">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-1165">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-1165">Monitor</span></span>

* <span data-ttu-id="091e2-1166">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="091e2-1166">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1167">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1167">Resource</span></span>

* <span data-ttu-id="091e2-1168">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="091e2-1168">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="091e2-1169">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-1169">Role</span></span>

* <span data-ttu-id="091e2-1170">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="091e2-1170">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="091e2-1171">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="091e2-1171">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="091e2-1172">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="091e2-1172">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1173">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-1173">SQL</span></span>

* <span data-ttu-id="091e2-1174">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="091e2-1174">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="091e2-1175">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1175">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1176">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1176">VM</span></span>

* <span data-ttu-id="091e2-1177">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="091e2-1177">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="091e2-1178">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1178">November 14, 2017</span></span>

<span data-ttu-id="091e2-1179">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="091e2-1179">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-1180">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-1180">ACR</span></span>

* <span data-ttu-id="091e2-1181">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="091e2-1181">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="091e2-1182">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1182">ACS</span></span>

* <span data-ttu-id="091e2-1183">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="091e2-1183">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="091e2-1184">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1184">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="091e2-1185">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="091e2-1185">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="091e2-1186">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="091e2-1186">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="091e2-1187">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="091e2-1187">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1188">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1188">Appservice</span></span>

* <span data-ttu-id="091e2-1189">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="091e2-1189">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="091e2-1190">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="091e2-1190">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="091e2-1191">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="091e2-1191">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="091e2-1192">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="091e2-1192">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="091e2-1193">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="091e2-1193">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="091e2-1194">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="091e2-1194">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-1195">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-1195">Batch</span></span>

* <span data-ttu-id="091e2-1196">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="091e2-1196">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="091e2-1197">Batchai</span><span class="sxs-lookup"><span data-stu-id="091e2-1197">Batchai</span></span>

* <span data-ttu-id="091e2-1198">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1198">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="091e2-1199">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1199">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="091e2-1200">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="091e2-1200">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="091e2-1201">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1201">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="091e2-1202">Nube</span><span class="sxs-lookup"><span data-stu-id="091e2-1202">Cloud</span></span>

* <span data-ttu-id="091e2-1203">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="091e2-1203">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="091e2-1204">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-1204">Container</span></span>

* <span data-ttu-id="091e2-1205">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="091e2-1205">Added support to open multiple ports</span></span>
* <span data-ttu-id="091e2-1206">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="091e2-1206">Added container group restart policy</span></span>
* <span data-ttu-id="091e2-1207">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="091e2-1207">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="091e2-1208">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="091e2-1208">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="091e2-1209">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="091e2-1209">Data Lake Analytics</span></span>

* <span data-ttu-id="091e2-1210">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="091e2-1210">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="091e2-1211">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="091e2-1211">Data Lake Store</span></span>

* <span data-ttu-id="091e2-1212">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="091e2-1212">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-1213">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-1213">Extension</span></span>

* <span data-ttu-id="091e2-1214">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="091e2-1214">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="091e2-1215">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="091e2-1215">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-1216">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-1216">IoT</span></span>

* <span data-ttu-id="091e2-1217">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="091e2-1217">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-1218">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-1218">Monitor</span></span>

* <span data-ttu-id="091e2-1219">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1219">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1220">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1220">Network</span></span>

* <span data-ttu-id="091e2-1221">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="091e2-1221">Added support for CAA DNS records</span></span>
* <span data-ttu-id="091e2-1222">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1222">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="091e2-1223">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1223">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="091e2-1224">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="091e2-1224">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="091e2-1225">Reservations</span><span class="sxs-lookup"><span data-stu-id="091e2-1225">Reservations</span></span>

* <span data-ttu-id="091e2-1226">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="091e2-1226">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1227">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1227">Resource</span></span>

* <span data-ttu-id="091e2-1228">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1228">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-1229">SQL</span></span>

* <span data-ttu-id="091e2-1230">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1230">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1231">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1231">Storage</span></span>

* <span data-ttu-id="091e2-1232">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="091e2-1232">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="091e2-1233">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="091e2-1233">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="091e2-1234">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="091e2-1234">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="091e2-1235">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="091e2-1235">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="091e2-1236">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1236">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="091e2-1237">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="091e2-1237">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="091e2-1238">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="091e2-1238">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1239">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1239">VM</span></span>

* <span data-ttu-id="091e2-1240">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="091e2-1240">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="091e2-1241">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="091e2-1241">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="091e2-1242">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="091e2-1242">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="091e2-1243">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1243">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="091e2-1244">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="091e2-1244">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="091e2-1245">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1245">October 24, 2017</span></span>

<span data-ttu-id="091e2-1246">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="091e2-1246">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="091e2-1247">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1247">Core</span></span>

* <span data-ttu-id="091e2-1248">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="091e2-1248">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-1249">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-1249">ACR</span></span>

* <span data-ttu-id="091e2-1250">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="091e2-1250">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="091e2-1251">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="091e2-1251">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="091e2-1252">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="091e2-1252">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1253">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1253">ACS</span></span>

* <span data-ttu-id="091e2-1254">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="091e2-1254">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="091e2-1255">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="091e2-1255">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1256">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1256">Appservice</span></span>

* <span data-ttu-id="091e2-1257">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="091e2-1257">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="091e2-1258">Componente</span><span class="sxs-lookup"><span data-stu-id="091e2-1258">Component</span></span>

* <span data-ttu-id="091e2-1259">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="091e2-1259">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-1260">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-1260">Monitor</span></span>

* <span data-ttu-id="091e2-1261">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1261">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1262">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1262">Resource</span></span>

* <span data-ttu-id="091e2-1263">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="091e2-1263">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="091e2-1264">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="091e2-1264">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1265">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1265">VM</span></span>

* <span data-ttu-id="091e2-1266">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1266">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="091e2-1267">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1267">October 9, 2017</span></span>

<span data-ttu-id="091e2-1268">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="091e2-1268">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="091e2-1269">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1269">Core</span></span>

* <span data-ttu-id="091e2-1270">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="091e2-1270">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1271">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1271">Appservice</span></span>

* <span data-ttu-id="091e2-1272">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1272">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-1273">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-1273">Batch</span></span>

* <span data-ttu-id="091e2-1274">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="091e2-1274">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="091e2-1275">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="091e2-1275">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="091e2-1276">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-1276">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="091e2-1277">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="091e2-1277">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="091e2-1278">Batchai</span><span class="sxs-lookup"><span data-stu-id="091e2-1278">Batchai</span></span>

* <span data-ttu-id="091e2-1279">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-1279">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-1280">Keyvault</span><span class="sxs-lookup"><span data-stu-id="091e2-1280">Keyvault</span></span>

* <span data-ttu-id="091e2-1281">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="091e2-1281">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="091e2-1282">(#4448)</span><span class="sxs-lookup"><span data-stu-id="091e2-1282">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="091e2-1283">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1283">Network</span></span>

* <span data-ttu-id="091e2-1284">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="091e2-1284">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="091e2-1285">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="091e2-1285">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1286">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1286">Resource</span></span>

* <span data-ttu-id="091e2-1287">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1287">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="091e2-1288">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="091e2-1288">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="091e2-1289">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="091e2-1289">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="091e2-1290">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1290">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1291">Sql</span><span class="sxs-lookup"><span data-stu-id="091e2-1291">Sql</span></span>

* <span data-ttu-id="091e2-1292">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="091e2-1292">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="091e2-1293">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="091e2-1293">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="091e2-1294">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="091e2-1294">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1295">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1295">Storage</span></span>

* <span data-ttu-id="091e2-1296">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="091e2-1296">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1297">Vm</span><span class="sxs-lookup"><span data-stu-id="091e2-1297">Vm</span></span>

* <span data-ttu-id="091e2-1298">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="091e2-1298">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="091e2-1299">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1299">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="091e2-1300">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="091e2-1300">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="091e2-1301">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1301">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="091e2-1302">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1302">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="091e2-1303">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1303">September 22, 2017</span></span>

<span data-ttu-id="091e2-1304">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="091e2-1304">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1305">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1305">Resource</span></span>

* <span data-ttu-id="091e2-1306">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="091e2-1306">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="091e2-1307">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="091e2-1307">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="091e2-1308">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1308">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="091e2-1309">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="091e2-1309">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1310">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1310">Network</span></span>

* <span data-ttu-id="091e2-1311">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="091e2-1311">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="091e2-1312">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="091e2-1312">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="091e2-1313">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="091e2-1313">Added `asg` application security group commands</span></span>
* <span data-ttu-id="091e2-1314">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1314">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="091e2-1315">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1315">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="091e2-1316">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1316">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="091e2-1317">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1317">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1318">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1318">Storage</span></span>

* <span data-ttu-id="091e2-1319">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="091e2-1319">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="091e2-1320">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="091e2-1320">Eventgrid</span></span>

* <span data-ttu-id="091e2-1321">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="091e2-1321">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1322">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-1322">SQL</span></span>

* <span data-ttu-id="091e2-1323">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="091e2-1323">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="091e2-1324">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="091e2-1324">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="091e2-1325">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1325">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-1326">Keyvault</span><span class="sxs-lookup"><span data-stu-id="091e2-1326">Keyvault</span></span>

* <span data-ttu-id="091e2-1327">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="091e2-1327">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1328">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1328">VM</span></span>

* <span data-ttu-id="091e2-1329">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1329">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="091e2-1330">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="091e2-1330">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="091e2-1331">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1331">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="091e2-1332">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="091e2-1332">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="091e2-1333">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="091e2-1333">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="091e2-1334">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="091e2-1334">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1335">ACS</span></span>

* <span data-ttu-id="091e2-1336">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1336">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1337">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1337">Appservice</span></span>

* <span data-ttu-id="091e2-1338">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1338">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="091e2-1339">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="091e2-1339">Backup</span></span>

* <span data-ttu-id="091e2-1340">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="091e2-1340">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="091e2-1341">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1341">September 11, 2017</span></span>

<span data-ttu-id="091e2-1342">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="091e2-1342">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="091e2-1343">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1343">Core</span></span>

* <span data-ttu-id="091e2-1344">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="091e2-1344">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="091e2-1345">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="091e2-1345">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1346">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1346">Acs</span></span>

* <span data-ttu-id="091e2-1347">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1347">Added `acs list-locations` command</span></span>
* <span data-ttu-id="091e2-1348">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="091e2-1348">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1349">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1349">Appservice</span></span>

* <span data-ttu-id="091e2-1350">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="091e2-1350">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="091e2-1351">CDN</span><span class="sxs-lookup"><span data-stu-id="091e2-1351">CDN</span></span>

* <span data-ttu-id="091e2-1352">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1352">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="091e2-1353">Extensión</span><span class="sxs-lookup"><span data-stu-id="091e2-1353">Extension</span></span>

* <span data-ttu-id="091e2-1354">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="091e2-1354">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-1355">Keyvault</span><span class="sxs-lookup"><span data-stu-id="091e2-1355">Keyvault</span></span>

* <span data-ttu-id="091e2-1356">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="091e2-1356">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1357">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1357">Network</span></span>

* <span data-ttu-id="091e2-1358">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1358">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="091e2-1359">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1359">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="091e2-1360">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1360">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="091e2-1361">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1361">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="091e2-1362">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1362">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1363">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1363">Resource</span></span>

* <span data-ttu-id="091e2-1364">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1364">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="091e2-1365">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1365">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="091e2-1366">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="091e2-1366">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="091e2-1367">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="091e2-1367">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1368">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-1368">SQL</span></span>

* <span data-ttu-id="091e2-1369">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1369">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1370">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1370">VM</span></span>

* <span data-ttu-id="091e2-1371">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1371">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="091e2-1372">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="091e2-1372">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="091e2-1373">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1373">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="091e2-1374">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="091e2-1374">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="091e2-1375">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="091e2-1375">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="091e2-1376">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1376">August 31, 2017</span></span>

<span data-ttu-id="091e2-1377">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="091e2-1377">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-1378">Keyvault</span><span class="sxs-lookup"><span data-stu-id="091e2-1378">Keyvault</span></span>

* <span data-ttu-id="091e2-1379">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1379">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="091e2-1380">Sf</span><span class="sxs-lookup"><span data-stu-id="091e2-1380">Sf</span></span>

* <span data-ttu-id="091e2-1381">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="091e2-1381">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1382">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1382">Storage</span></span>

* <span data-ttu-id="091e2-1383">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="091e2-1383">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="091e2-1384">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="091e2-1384">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="091e2-1385">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1385">August 28, 2017</span></span>

<span data-ttu-id="091e2-1386">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="091e2-1386">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="091e2-1387">CLI</span><span class="sxs-lookup"><span data-stu-id="091e2-1387">CLI</span></span>

* <span data-ttu-id="091e2-1388">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="091e2-1388">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1389">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1389">ACS</span></span>

* <span data-ttu-id="091e2-1390">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="091e2-1390">Corrected preview regions</span></span>
* <span data-ttu-id="091e2-1391">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="091e2-1391">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="091e2-1392">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="091e2-1392">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1393">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1393">Appservice</span></span>

* <span data-ttu-id="091e2-1394">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1394">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="091e2-1395">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1395">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="091e2-1396">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1396">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="091e2-1397">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="091e2-1397">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="091e2-1398">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="091e2-1398">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-1399">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-1399">IoT</span></span>

* <span data-ttu-id="091e2-1400">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="091e2-1400">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1401">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1401">Network</span></span>

* <span data-ttu-id="091e2-1402">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="091e2-1402">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="091e2-1403">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="091e2-1403">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="091e2-1404">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1404">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="091e2-1405">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1405">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="091e2-1406">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1406">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-1407">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-1407">Profile</span></span>

* <span data-ttu-id="091e2-1408">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="091e2-1408">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="091e2-1409">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="091e2-1409">Service Fabric</span></span>

* <span data-ttu-id="091e2-1410">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="091e2-1410">Preview release</span></span>
* <span data-ttu-id="091e2-1411">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="091e2-1411">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="091e2-1412">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="091e2-1412">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="091e2-1413">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1413">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1414">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1414">Storage</span></span>

* <span data-ttu-id="091e2-1415">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="091e2-1415">Enabled setting blob tier</span></span>
* <span data-ttu-id="091e2-1416">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="091e2-1416">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="091e2-1417">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1417">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="091e2-1418">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="091e2-1418">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="091e2-1419">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="091e2-1419">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="091e2-1420">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="091e2-1420">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1421">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1421">VM</span></span>

* <span data-ttu-id="091e2-1422">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1422">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="091e2-1423">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1423">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="091e2-1424">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1424">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="091e2-1425">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="091e2-1425">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="091e2-1426">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="091e2-1426">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="091e2-1427">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1427">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="091e2-1428">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1428">August 15, 2017</span></span>

<span data-ttu-id="091e2-1429">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="091e2-1429">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1430">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1430">ACS</span></span>

* <span data-ttu-id="091e2-1431">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="091e2-1431">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1432">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1432">Appservice</span></span>

* <span data-ttu-id="091e2-1433">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="091e2-1433">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="091e2-1434">Event Grid</span><span class="sxs-lookup"><span data-stu-id="091e2-1434">Event Grid</span></span>

* <span data-ttu-id="091e2-1435">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="091e2-1435">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="091e2-1436">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1436">August 11, 2017</span></span>

<span data-ttu-id="091e2-1437">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="091e2-1437">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1438">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1438">ACS</span></span>

* <span data-ttu-id="091e2-1439">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="091e2-1439">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-1440">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-1440">Batch</span></span>

* <span data-ttu-id="091e2-1441">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="091e2-1441">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="091e2-1442">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="091e2-1442">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="091e2-1443">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="091e2-1443">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="091e2-1444">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="091e2-1444">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="091e2-1445">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="091e2-1445">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="091e2-1446">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="091e2-1446">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="091e2-1447">Componente</span><span class="sxs-lookup"><span data-stu-id="091e2-1447">Component</span></span>

* <span data-ttu-id="091e2-1448">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="091e2-1448">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="091e2-1449">Contenedor</span><span class="sxs-lookup"><span data-stu-id="091e2-1449">Container</span></span>

* <span data-ttu-id="091e2-1450">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="091e2-1450">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="091e2-1451">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="091e2-1451">Data Lake Store</span></span>

* <span data-ttu-id="091e2-1452">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="091e2-1452">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="091e2-1453">Event Grid</span><span class="sxs-lookup"><span data-stu-id="091e2-1453">Event Grid</span></span>

* <span data-ttu-id="091e2-1454">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="091e2-1454">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1455">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1455">Network</span></span>

* <span data-ttu-id="091e2-1456">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="091e2-1456">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="091e2-1457">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1457">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="091e2-1458">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="091e2-1458">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="091e2-1459">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1459">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-1460">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-1460">Profile</span></span>

* <span data-ttu-id="091e2-1461">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="091e2-1461">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1462">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1462">Storage</span></span>

* <span data-ttu-id="091e2-1463">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="091e2-1463">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1464">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1464">VM</span></span>

* <span data-ttu-id="091e2-1465">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="091e2-1465">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="091e2-1466">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1466">Exposed `list-skus` command</span></span>
* <span data-ttu-id="091e2-1467">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="091e2-1467">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="091e2-1468">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="091e2-1468">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="091e2-1469">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="091e2-1469">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="091e2-1470">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1470">July 28, 2017</span></span>

<span data-ttu-id="091e2-1471">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="091e2-1471">Version 2.0.12</span></span>

* <span data-ttu-id="091e2-1472">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="091e2-1472">Added container commands</span></span>
* <span data-ttu-id="091e2-1473">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="091e2-1473">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="091e2-1474">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1474">Core</span></span>

* <span data-ttu-id="091e2-1475">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="091e2-1475">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="091e2-1476">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="091e2-1476">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="091e2-1477">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="091e2-1477">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="091e2-1478">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="091e2-1478">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="091e2-1479">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="091e2-1479">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="091e2-1480">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="091e2-1480">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="091e2-1481">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="091e2-1481">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="091e2-1482">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="091e2-1482">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="091e2-1483">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="091e2-1483">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="091e2-1484">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="091e2-1484">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="091e2-1485">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="091e2-1485">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="091e2-1486">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="091e2-1486">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="091e2-1487">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="091e2-1487">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="091e2-1488">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="091e2-1488">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="091e2-1489">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="091e2-1489">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="091e2-1490">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="091e2-1490">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="091e2-1491">ACR</span><span class="sxs-lookup"><span data-stu-id="091e2-1491">ACR</span></span>

* <span data-ttu-id="091e2-1492">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="091e2-1492">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="091e2-1493">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="091e2-1493">Support SKU update for managed registries</span></span>
* <span data-ttu-id="091e2-1494">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="091e2-1494">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="091e2-1495">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="091e2-1495">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="091e2-1496">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="091e2-1496">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="091e2-1497">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="091e2-1497">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1498">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1498">ACS</span></span>

* <span data-ttu-id="091e2-1499">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="091e2-1499">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1500">Appservice</span><span class="sxs-lookup"><span data-stu-id="091e2-1500">Appservice</span></span>

* <span data-ttu-id="091e2-1501">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="091e2-1501">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="091e2-1502">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="091e2-1502">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="091e2-1503">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1503">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="091e2-1504">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="091e2-1504">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="091e2-1505">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="091e2-1505">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="091e2-1506">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="091e2-1506">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="091e2-1507">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="091e2-1507">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="091e2-1508">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="091e2-1508">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="091e2-1509">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="091e2-1509">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="091e2-1510">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="091e2-1510">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="091e2-1511">Batch</span><span class="sxs-lookup"><span data-stu-id="091e2-1511">Batch</span></span>

* <span data-ttu-id="091e2-1512">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="091e2-1512">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="091e2-1513">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1513">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="091e2-1514">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1514">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="091e2-1515">CDN</span><span class="sxs-lookup"><span data-stu-id="091e2-1515">CDN</span></span>

* <span data-ttu-id="091e2-1516">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="091e2-1516">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="091e2-1517">Nube</span><span class="sxs-lookup"><span data-stu-id="091e2-1517">Cloud</span></span>

* <span data-ttu-id="091e2-1518">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="091e2-1518">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="091e2-1519">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="091e2-1519">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="091e2-1520">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="091e2-1520">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="091e2-1521">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="091e2-1521">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="091e2-1522">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1522">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="091e2-1523">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="091e2-1523">CosmosDB</span></span>

* <span data-ttu-id="091e2-1524">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="091e2-1524">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="091e2-1525">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="091e2-1525">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="091e2-1526">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="091e2-1526">Data Lake Analytics</span></span>

* <span data-ttu-id="091e2-1527">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1527">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="091e2-1528">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1528">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="091e2-1529">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1529">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="091e2-1530">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="091e2-1530">Data Lake Store</span></span>

* <span data-ttu-id="091e2-1531">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1531">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="091e2-1532">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="091e2-1532">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="091e2-1533">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1533">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="091e2-1534">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="091e2-1534">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="091e2-1535">Interactive</span><span class="sxs-lookup"><span data-stu-id="091e2-1535">Interactive</span></span>

* <span data-ttu-id="091e2-1536">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="091e2-1536">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="091e2-1537">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="091e2-1537">Increased test coverage</span></span>
* <span data-ttu-id="091e2-1538">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="091e2-1538">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="091e2-1539">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="091e2-1539">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="091e2-1540">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="091e2-1540">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="091e2-1541">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="091e2-1541">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="091e2-1542">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="091e2-1542">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="091e2-1543">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1543">Added `--progress` flag</span></span>
* <span data-ttu-id="091e2-1544">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="091e2-1544">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="091e2-1545">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="091e2-1545">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="091e2-1546">IoT</span><span class="sxs-lookup"><span data-stu-id="091e2-1546">IoT</span></span>

* <span data-ttu-id="091e2-1547">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="091e2-1547">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="091e2-1548">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="091e2-1548">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="091e2-1549">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="091e2-1549">Key vault</span></span>

* <span data-ttu-id="091e2-1550">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="091e2-1550">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="091e2-1551">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="091e2-1551">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="091e2-1552">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="091e2-1552">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="091e2-1553">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="091e2-1553">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="091e2-1554">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="091e2-1554">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="091e2-1555">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="091e2-1555">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="091e2-1556">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="091e2-1556">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="091e2-1557">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="091e2-1557">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="091e2-1558">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-1558">Lab</span></span>

* <span data-ttu-id="091e2-1559">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1559">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="091e2-1560">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1560">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-1561">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-1561">Monitor</span></span>

* <span data-ttu-id="091e2-1562">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="091e2-1562">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="091e2-1563">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1563">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="091e2-1564">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1564">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="091e2-1565">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1565">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="091e2-1566">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1566">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="091e2-1567">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="091e2-1567">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="091e2-1568">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="091e2-1568">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="091e2-1569">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="091e2-1569">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="091e2-1570">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="091e2-1570">`location` no longer required</span></span>
  * <span data-ttu-id="091e2-1571">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="091e2-1571">Add name and ID support for target</span></span>
  * <span data-ttu-id="091e2-1572">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1572">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="091e2-1573">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="091e2-1573">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="091e2-1574">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="091e2-1574">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="091e2-1575">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="091e2-1575">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="091e2-1576">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1576">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="091e2-1577">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="091e2-1577">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1578">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1578">Network</span></span>

* <span data-ttu-id="091e2-1579">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1579">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="091e2-1580">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1580">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="091e2-1581">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="091e2-1581">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="091e2-1582">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="091e2-1582">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="091e2-1583">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1583">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="091e2-1584">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1584">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="091e2-1585">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="091e2-1585">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="091e2-1586">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="091e2-1586">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="091e2-1587">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="091e2-1587">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="091e2-1588">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="091e2-1588">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="091e2-1589">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1589">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="091e2-1590">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1590">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="091e2-1591">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="091e2-1591">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="091e2-1592">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1592">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="091e2-1593">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1593">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="091e2-1594">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1594">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="091e2-1595">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="091e2-1595">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="091e2-1596">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1596">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="091e2-1597">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1597">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="091e2-1598">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1598">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="091e2-1599">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1599">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="091e2-1600">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1600">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="091e2-1601">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1601">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="091e2-1602">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="091e2-1602">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="091e2-1603">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="091e2-1603">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="091e2-1604">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="091e2-1604">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="091e2-1605">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="091e2-1605">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-1606">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-1606">Profile</span></span>

* <span data-ttu-id="091e2-1607">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="091e2-1607">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="091e2-1608">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="091e2-1608">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="091e2-1609">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="091e2-1609">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="091e2-1610">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="091e2-1610">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="091e2-1611">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="091e2-1611">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="091e2-1612">RDBMS</span><span class="sxs-lookup"><span data-stu-id="091e2-1612">RDBMS</span></span>

* <span data-ttu-id="091e2-1613">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="091e2-1613">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="091e2-1614">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="091e2-1614">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="091e2-1615">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="091e2-1615">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="091e2-1616">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="091e2-1616">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1617">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1617">Resource</span></span>

* <span data-ttu-id="091e2-1618">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1618">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="091e2-1619">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1619">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="091e2-1620">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1620">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="091e2-1621">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1621">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="091e2-1622">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="091e2-1622">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="091e2-1623">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1623">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="091e2-1624">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="091e2-1624">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="091e2-1625">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1625">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="091e2-1626">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-1626">Role</span></span>

* <span data-ttu-id="091e2-1627">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="091e2-1627">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="091e2-1628">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="091e2-1628">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="091e2-1629">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1629">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="091e2-1630">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1630">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="091e2-1631">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1631">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="091e2-1632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="091e2-1632">Service Fabric</span></span>
* <span data-ttu-id="091e2-1633">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="091e2-1633">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="091e2-1634">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="091e2-1634">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="091e2-1635">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="091e2-1635">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1636">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-1636">SQL</span></span>

* <span data-ttu-id="091e2-1637">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="091e2-1637">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="091e2-1638">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1638">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="091e2-1639">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="091e2-1639">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1640">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1640">Storage</span></span>

* <span data-ttu-id="091e2-1641">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="091e2-1641">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="091e2-1642">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="091e2-1642">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="091e2-1643">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="091e2-1643">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="091e2-1644">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="091e2-1644">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="091e2-1645">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="091e2-1645">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="091e2-1646">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="091e2-1646">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1647">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1647">VM</span></span>

* <span data-ttu-id="091e2-1648">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="091e2-1648">Support configuring nsg</span></span>
* <span data-ttu-id="091e2-1649">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="091e2-1649">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="091e2-1650">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="091e2-1650">Support managed service identities</span></span>
* <span data-ttu-id="091e2-1651">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="091e2-1651">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="091e2-1652">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="091e2-1652">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="091e2-1653">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1653">May 10, 2017</span></span>

<span data-ttu-id="091e2-1654">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="091e2-1654">Version 2.0.6</span></span>

* <span data-ttu-id="091e2-1655">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="091e2-1655">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="091e2-1656">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="091e2-1656">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="091e2-1657">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="091e2-1657">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="091e2-1658">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="091e2-1658">Include Cognitive Services module</span></span>
* <span data-ttu-id="091e2-1659">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="091e2-1659">Include Service Fabric module</span></span>
* <span data-ttu-id="091e2-1660">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="091e2-1660">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="091e2-1661">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="091e2-1661">Add support for CDN commands</span></span>
* <span data-ttu-id="091e2-1662">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="091e2-1662">Remove Container module</span></span>
* <span data-ttu-id="091e2-1663">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="091e2-1663">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="091e2-1664">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="091e2-1664">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="091e2-1665">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1665">Core</span></span>

* <span data-ttu-id="091e2-1666">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="091e2-1666">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="091e2-1667">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="091e2-1667">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="091e2-1668">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="091e2-1668">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="091e2-1669">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="091e2-1669">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="091e2-1670">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="091e2-1670">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="091e2-1671">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="091e2-1671">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="091e2-1672">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="091e2-1672">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="091e2-1673">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="091e2-1673">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="091e2-1674">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="091e2-1674">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="091e2-1675">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="091e2-1675">core: Improved performance</span></span>
* <span data-ttu-id="091e2-1676">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="091e2-1676">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="091e2-1677">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="091e2-1677">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1678">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1678">ACS</span></span>

* <span data-ttu-id="091e2-1679">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="091e2-1679">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="091e2-1680">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="091e2-1680">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="091e2-1681">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="091e2-1681">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="091e2-1682">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="091e2-1682">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1683">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-1683">AppService</span></span>

* <span data-ttu-id="091e2-1684">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="091e2-1684">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="091e2-1685">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="091e2-1685">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="091e2-1686">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="091e2-1686">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="091e2-1687">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="091e2-1687">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="091e2-1688">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="091e2-1688">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="091e2-1689">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="091e2-1689">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="091e2-1690">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="091e2-1690">support slot swap with preview</span></span>
* <span data-ttu-id="091e2-1691">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="091e2-1691">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="091e2-1692">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="091e2-1692">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="091e2-1693">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="091e2-1693">CosmosDB</span></span>

* <span data-ttu-id="091e2-1694">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="091e2-1694">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="091e2-1695">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="091e2-1695">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="091e2-1696">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="091e2-1696">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="091e2-1697">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="091e2-1697">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="091e2-1698">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="091e2-1698">Data Lake Analytics</span></span>

* <span data-ttu-id="091e2-1699">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="091e2-1699">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="091e2-1700">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="091e2-1700">Add support for new catalog item type: package.</span></span> <span data-ttu-id="091e2-1701">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="091e2-1701">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="091e2-1702">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="091e2-1702">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="091e2-1703">Tabla</span><span class="sxs-lookup"><span data-stu-id="091e2-1703">Table</span></span>
  * <span data-ttu-id="091e2-1704">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="091e2-1704">Table valued function</span></span>
  * <span data-ttu-id="091e2-1705">Ver</span><span class="sxs-lookup"><span data-stu-id="091e2-1705">View</span></span>
  * <span data-ttu-id="091e2-1706">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="091e2-1706">Table Statistics.</span></span> <span data-ttu-id="091e2-1707">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="091e2-1707">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="091e2-1708">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="091e2-1708">Data Lake Store</span></span>

* <span data-ttu-id="091e2-1709">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="091e2-1709">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="091e2-1710">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="091e2-1710">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="091e2-1711">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="091e2-1711">missed help for access show.</span></span> <span data-ttu-id="091e2-1712">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="091e2-1712">adding it.</span></span> <span data-ttu-id="091e2-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="091e2-1713">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="091e2-1714">Buscar</span><span class="sxs-lookup"><span data-stu-id="091e2-1714">Find</span></span>

* <span data-ttu-id="091e2-1715">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="091e2-1715">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="091e2-1716">KeyVault</span><span class="sxs-lookup"><span data-stu-id="091e2-1716">KeyVault</span></span>

* <span data-ttu-id="091e2-1717">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="091e2-1717">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="091e2-1718">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="091e2-1718">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="091e2-1719">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="091e2-1719">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="091e2-1720">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="091e2-1720">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="091e2-1721">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="091e2-1721">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="091e2-1722">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-1722">Lab</span></span>

* <span data-ttu-id="091e2-1723">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-1723">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="091e2-1724">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-1724">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="091e2-1725">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-1725">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="091e2-1726">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-1726">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="091e2-1727">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="091e2-1727">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="091e2-1728">Supervisión</span><span class="sxs-lookup"><span data-stu-id="091e2-1728">Monitor</span></span>

* <span data-ttu-id="091e2-1729">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="091e2-1729">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="091e2-1730">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="091e2-1730">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="091e2-1731">Red</span><span class="sxs-lookup"><span data-stu-id="091e2-1731">Network</span></span>

* <span data-ttu-id="091e2-1732">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="091e2-1732">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="091e2-1733">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1733">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="091e2-1734">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="091e2-1734">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="091e2-1735">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="091e2-1735">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="091e2-1736">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="091e2-1736">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="091e2-1737">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="091e2-1737">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="091e2-1738">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="091e2-1738">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="091e2-1739">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="091e2-1739">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="091e2-1740">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="091e2-1740">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="091e2-1741">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="091e2-1741">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="091e2-1742">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="091e2-1742">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="091e2-1743">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1743">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="091e2-1744">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="091e2-1744">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="091e2-1745">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="091e2-1745">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="091e2-1746">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="091e2-1746">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="091e2-1747">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="091e2-1747">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="091e2-1748">Perfil</span><span class="sxs-lookup"><span data-stu-id="091e2-1748">Profile</span></span>

* <span data-ttu-id="091e2-1749">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="091e2-1749">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="091e2-1750">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="091e2-1750">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="091e2-1751">Redis</span><span class="sxs-lookup"><span data-stu-id="091e2-1751">Redis</span></span>

* <span data-ttu-id="091e2-1752">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="091e2-1752">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="091e2-1753">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="091e2-1753">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="091e2-1754">Recurso</span><span class="sxs-lookup"><span data-stu-id="091e2-1754">Resource</span></span>

* <span data-ttu-id="091e2-1755">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="091e2-1755">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="091e2-1756">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="091e2-1756">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="091e2-1757">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="091e2-1757">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="091e2-1758">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="091e2-1758">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="091e2-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="091e2-1759">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="091e2-1760">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="091e2-1760">Add docs for az lock update.</span></span> <span data-ttu-id="091e2-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="091e2-1761">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="091e2-1762">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="091e2-1762">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="091e2-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="091e2-1763">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="091e2-1764">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="091e2-1764">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="091e2-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="091e2-1765">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="091e2-1766">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="091e2-1766">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="091e2-1767">Rol</span><span class="sxs-lookup"><span data-stu-id="091e2-1767">Role</span></span>

* <span data-ttu-id="091e2-1768">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="091e2-1768">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="091e2-1769">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="091e2-1769">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="091e2-1770">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="091e2-1770">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="091e2-1771">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="091e2-1771">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="091e2-1772">SQL</span><span class="sxs-lookup"><span data-stu-id="091e2-1772">SQL</span></span>

* <span data-ttu-id="091e2-1773">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="091e2-1773">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="091e2-1774">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="091e2-1774">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="091e2-1775">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1775">Storage</span></span>

* <span data-ttu-id="091e2-1776">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="091e2-1776">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="091e2-1777">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="091e2-1777">Add support for incremental blob copy</span></span>
* <span data-ttu-id="091e2-1778">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="091e2-1778">Add support for large block blob upload</span></span>
* <span data-ttu-id="091e2-1779">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="091e2-1779">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1780">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1780">VM</span></span>

* <span data-ttu-id="091e2-1781">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="091e2-1781">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="091e2-1782">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="091e2-1782">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="091e2-1783">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="091e2-1783">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="091e2-1784">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="091e2-1784">az vm/vmss disk</span></span>
  3. <span data-ttu-id="091e2-1785">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="091e2-1785">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="091e2-1786">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="091e2-1786">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="091e2-1787">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="091e2-1787">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="091e2-1788">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1788">April 3, 2017</span></span>

<span data-ttu-id="091e2-1789">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="091e2-1789">Version 2.0.2</span></span>

<span data-ttu-id="091e2-1790">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="091e2-1790">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="091e2-1791">Núcleo</span><span class="sxs-lookup"><span data-stu-id="091e2-1791">Core</span></span>

* <span data-ttu-id="091e2-1792">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="091e2-1792">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="091e2-1793">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="091e2-1793">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="091e2-1794">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="091e2-1794">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="091e2-1795">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="091e2-1795">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="091e2-1796">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="091e2-1796">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="091e2-1797">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="091e2-1797">Add prompting for missing template parameters.</span></span> <span data-ttu-id="091e2-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="091e2-1798">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="091e2-1799">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="091e2-1799">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="091e2-1800">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="091e2-1800">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="091e2-1801">ACS</span><span class="sxs-lookup"><span data-stu-id="091e2-1801">ACS</span></span>

* <span data-ttu-id="091e2-1802">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="091e2-1802">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="091e2-1803">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="091e2-1803">Add support for ssh key password prompting.</span></span> <span data-ttu-id="091e2-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="091e2-1804">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="091e2-1805">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="091e2-1805">Add support for windows clusters.</span></span> <span data-ttu-id="091e2-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="091e2-1806">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="091e2-1807">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="091e2-1807">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="091e2-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="091e2-1808">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="091e2-1809">AppService</span><span class="sxs-lookup"><span data-stu-id="091e2-1809">AppService</span></span>

* <span data-ttu-id="091e2-1810">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="091e2-1810">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="091e2-1811">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="091e2-1811">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="091e2-1812">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="091e2-1812">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="091e2-1813">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="091e2-1813">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="091e2-1814">DataLake</span><span class="sxs-lookup"><span data-stu-id="091e2-1814">DataLake</span></span>

* <span data-ttu-id="091e2-1815">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="091e2-1815">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="091e2-1816">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="091e2-1816">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="091e2-1817">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="091e2-1817">DocuemntDB</span></span>

* <span data-ttu-id="091e2-1818">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="091e2-1818">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="091e2-1819">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="091e2-1819">VM</span></span>

* <span data-ttu-id="091e2-1820">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="091e2-1820">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="091e2-1821">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="091e2-1821">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="091e2-1822">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="091e2-1822">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="091e2-1823">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="091e2-1823">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="091e2-1824">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="091e2-1824">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="091e2-1825">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="091e2-1825">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="091e2-1826">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="091e2-1826">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="091e2-1827">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="091e2-1827">February 27, 2017</span></span>

<span data-ttu-id="091e2-1828">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="091e2-1828">Version 2.0.0</span></span>

<span data-ttu-id="091e2-1829">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="091e2-1829">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="091e2-1830">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="091e2-1830">Container Service (acs)</span></span>
- <span data-ttu-id="091e2-1831">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="091e2-1831">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="091e2-1832">Redes</span><span class="sxs-lookup"><span data-stu-id="091e2-1832">Networking</span></span>
- <span data-ttu-id="091e2-1833">Storage</span><span class="sxs-lookup"><span data-stu-id="091e2-1833">Storage</span></span>

<span data-ttu-id="091e2-1834">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="091e2-1834">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="091e2-1835">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="091e2-1835">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="091e2-1836">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="091e2-1836">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="091e2-1837">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="091e2-1837">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="091e2-1838">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="091e2-1838">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="091e2-1839">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="091e2-1839">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="091e2-1840">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="091e2-1840">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="091e2-1841">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="091e2-1841">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="091e2-1842">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="091e2-1842">Provide feedback from the command line with the `az feedback` command</span></span>

