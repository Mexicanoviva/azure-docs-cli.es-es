---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/20/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 7a2ab41dd6696d658d05ab76e44abf97626761aa
ms.sourcegitcommit: 14aa16beeec59e51890a6cba4906bdc8e19b94d0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/05/2018
ms.locfileid: "52892690"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="ef67e-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="ef67e-103">Azure CLI release notes</span></span>
## <a name="december-4-2018"></a><span data-ttu-id="ef67e-104">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-104">December 4, 2018</span></span>

<span data-ttu-id="ef67e-105">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="ef67e-105">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="ef67e-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-106">Core</span></span>
* <span data-ttu-id="ef67e-107">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="ef67e-107">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="ef67e-108">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="ef67e-108">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-109">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-109">Appservice</span></span>
* <span data-ttu-id="ef67e-110">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="ef67e-110">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="ef67e-111">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="ef67e-111">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-112">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-112">Network</span></span>
* <span data-ttu-id="ef67e-113">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="ef67e-113">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-114">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-114">Role</span></span>
* <span data-ttu-id="ef67e-115">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="ef67e-115">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="ef67e-116">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-116">VM</span></span>
* <span data-ttu-id="ef67e-117">[EN DESUSO] El parámetro `vm extension [show|wait] --expand` está en desuso</span><span class="sxs-lookup"><span data-stu-id="ef67e-117">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="ef67e-118">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="ef67e-118">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="ef67e-119">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="ef67e-119">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="ef67e-120">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="ef67e-120">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="ef67e-121">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-121">November 20, 2018</span></span>

<span data-ttu-id="ef67e-122">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="ef67e-122">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="ef67e-123">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-123">Core</span></span>
* <span data-ttu-id="ef67e-124">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="ef67e-124">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-125">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-125">ACR</span></span>
* <span data-ttu-id="ef67e-126">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="ef67e-126">Added context token to task step</span></span>
* <span data-ttu-id="ef67e-127">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="ef67e-127">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="ef67e-128">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-128">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-129">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-129">Appservice</span></span>
* <span data-ttu-id="ef67e-130">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="ef67e-130">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="ef67e-131">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-131">Updated the default `node_version`.</span></span> <span data-ttu-id="ef67e-132">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="ef67e-132">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="ef67e-133">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="ef67e-133">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="ef67e-134">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="ef67e-134">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="ef67e-135">IotCentral</span><span class="sxs-lookup"><span data-stu-id="ef67e-135">IotCentral</span></span>
* <span data-ttu-id="ef67e-136">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="ef67e-136">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-137">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ef67e-137">KeyVault</span></span>
* <span data-ttu-id="ef67e-138">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="ef67e-138">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-139">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-139">Network</span></span>
* <span data-ttu-id="ef67e-140">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="ef67e-140">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="ef67e-141">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="ef67e-141">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="ef67e-142">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="ef67e-142">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="ef67e-143">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-143">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-144">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ef67e-144">Rdbms</span></span>
* <span data-ttu-id="ef67e-145">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="ef67e-145">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="ef67e-146">Rbac</span><span class="sxs-lookup"><span data-stu-id="ef67e-146">Rbac</span></span>
* <span data-ttu-id="ef67e-147">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-147">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="ef67e-148">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-148">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="ef67e-149">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-149">Storage</span></span>
* <span data-ttu-id="ef67e-150">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="ef67e-150">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="ef67e-151">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-151">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="ef67e-152">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="ef67e-152">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="ef67e-153">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-153">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-154">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-154">VM</span></span>
* <span data-ttu-id="ef67e-155">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="ef67e-155">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="ef67e-156">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-156">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="ef67e-157">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-157">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="ef67e-158">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-158">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="ef67e-159">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-159">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="ef67e-160">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-160">Added `snapshot wait` command</span></span>
* <span data-ttu-id="ef67e-161">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-161">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="ef67e-162">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-162">November 6, 2018</span></span>

<span data-ttu-id="ef67e-163">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="ef67e-163">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-164">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-164">Core</span></span>
* <span data-ttu-id="ef67e-165">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="ef67e-165">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-166">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-166">ACR</span></span>
* <span data-ttu-id="ef67e-167">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="ef67e-167">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="ef67e-168">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="ef67e-168">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-169">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-169">ACS</span></span>
* <span data-ttu-id="ef67e-170">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="ef67e-170">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="ef67e-171">Advisor</span><span class="sxs-lookup"><span data-stu-id="ef67e-171">Advisor</span></span>
* <span data-ttu-id="ef67e-172">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="ef67e-172">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="ef67e-173">AMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-173">AMS</span></span>
* <span data-ttu-id="ef67e-174">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="ef67e-174">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="ef67e-175">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="ef67e-175">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="ef67e-176">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-176">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="ef67e-177">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-177">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="ef67e-178">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="ef67e-178">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="ef67e-179">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="ef67e-179">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="ef67e-180">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="ef67e-180">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="ef67e-181">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="ef67e-181">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="ef67e-182">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="ef67e-182">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="ef67e-183">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="ef67e-183">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="ef67e-184">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="ef67e-184">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="ef67e-185">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-185">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="ef67e-186">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="ef67e-186">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="ef67e-187">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="ef67e-187">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="ef67e-188">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-188">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="ef67e-189">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="ef67e-189">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="ef67e-190">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="ef67e-190">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-191">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-191">AppService</span></span>
* <span data-ttu-id="ef67e-192">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="ef67e-192">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="ef67e-193">Configuración</span><span class="sxs-lookup"><span data-stu-id="ef67e-193">Configure</span></span>
* <span data-ttu-id="ef67e-194">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="ef67e-194">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-195">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-195">Container</span></span>
* <span data-ttu-id="ef67e-196">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="ef67e-196">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="ef67e-197">EventHub</span><span class="sxs-lookup"><span data-stu-id="ef67e-197">EventHub</span></span>
* <span data-ttu-id="ef67e-198">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-198">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-199">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-199">Interactive</span></span>
* <span data-ttu-id="ef67e-200">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="ef67e-200">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-201">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-201">Monitor</span></span>
* <span data-ttu-id="ef67e-202">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-202">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-203">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-203">Network</span></span>
* <span data-ttu-id="ef67e-204">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="ef67e-204">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="ef67e-205">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="ef67e-205">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="ef67e-206">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-206">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="ef67e-207">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-207">Profile</span></span>
* <span data-ttu-id="ef67e-208">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="ef67e-208">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-209">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-209">RDBMS</span></span>
* <span data-ttu-id="ef67e-210">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="ef67e-210">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-211">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-211">Resource</span></span>
* <span data-ttu-id="ef67e-212">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="ef67e-212">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-213">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-213">Role</span></span>
* <span data-ttu-id="ef67e-214">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="ef67e-214">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="ef67e-215">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="ef67e-215">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="ef67e-216">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="ef67e-216">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-217">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-217">Storage</span></span>
* <span data-ttu-id="ef67e-218">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="ef67e-218">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-219">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-219">VM</span></span>
* <span data-ttu-id="ef67e-220">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="ef67e-220">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="ef67e-221">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="ef67e-221">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="ef67e-222">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="ef67e-222">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="ef67e-223">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="ef67e-223">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="ef67e-224">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="ef67e-224">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="ef67e-225">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="ef67e-225">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="ef67e-226">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-226">October 23, 2018</span></span>

<span data-ttu-id="ef67e-227">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="ef67e-227">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-228">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-228">Core</span></span>
* <span data-ttu-id="ef67e-229">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="ef67e-229">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="ef67e-230">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="ef67e-230">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-231">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-231">ACR</span></span>
* <span data-ttu-id="ef67e-232">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="ef67e-232">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="ef67e-233">CDN</span><span class="sxs-lookup"><span data-stu-id="ef67e-233">CDN</span></span>
* <span data-ttu-id="ef67e-234">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="ef67e-234">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="ef67e-235">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="ef67e-235">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-236">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-236">Container</span></span>
* <span data-ttu-id="ef67e-237">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="ef67e-237">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="ef67e-238">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-238">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="ef67e-239">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="ef67e-239">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="ef67e-240">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-240">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="ef67e-241">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="ef67e-241">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="ef67e-242">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="ef67e-242">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="ef67e-243">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="ef67e-243">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef67e-244">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-244">CosmosDB</span></span>
* <span data-ttu-id="ef67e-245">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-245">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-246">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-246">Interactive</span></span>
* <span data-ttu-id="ef67e-247">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="ef67e-247">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="ef67e-248">IoT Central</span><span class="sxs-lookup"><span data-stu-id="ef67e-248">IoT Central</span></span>
* <span data-ttu-id="ef67e-249">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="ef67e-249">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="ef67e-250">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="ef67e-250">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-251">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-251">Monitor</span></span>
* <span data-ttu-id="ef67e-252">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="ef67e-252">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="ef67e-253">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="ef67e-253">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="ef67e-254">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="ef67e-254">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ef67e-255">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="ef67e-255">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="ef67e-256">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="ef67e-256">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="ef67e-257">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="ef67e-257">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="ef67e-258">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="ef67e-258">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="ef67e-259">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="ef67e-259">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="ef67e-260">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="ef67e-260">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="ef67e-261">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-261">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-262">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-262">Network</span></span>
* <span data-ttu-id="ef67e-263">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="ef67e-263">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="ef67e-264">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="ef67e-264">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="ef67e-265">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ef67e-265">ServiceBus</span></span>
* <span data-ttu-id="ef67e-266">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="ef67e-266">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-267">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-267">SQL</span></span>
* <span data-ttu-id="ef67e-268">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="ef67e-268">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-269">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-269">Storage</span></span>
* <span data-ttu-id="ef67e-270">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="ef67e-270">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="ef67e-271">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="ef67e-271">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-272">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-272">VM</span></span>
* <span data-ttu-id="ef67e-273">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-273">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef67e-274">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-274">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="ef67e-275">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-275">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="ef67e-276">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-276">October 16, 2018</span></span>

<span data-ttu-id="ef67e-277">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="ef67e-277">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-278">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-278">VM</span></span>
* <span data-ttu-id="ef67e-279">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="ef67e-279">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="ef67e-280">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-280">October 9, 2018</span></span>

<span data-ttu-id="ef67e-281">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="ef67e-281">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-282">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-282">Core</span></span>
* <span data-ttu-id="ef67e-283">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="ef67e-283">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-284">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-284">ACR</span></span>
* <span data-ttu-id="ef67e-285">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="ef67e-285">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-286">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-286">ACS</span></span>
* <span data-ttu-id="ef67e-287">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="ef67e-287">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="ef67e-288">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="ef67e-288">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="ef67e-289">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="ef67e-289">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="ef67e-290">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="ef67e-290">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-291">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-291">Container</span></span>
* <span data-ttu-id="ef67e-292">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="ef67e-292">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="ef67e-293">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="ef67e-293">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="ef67e-294">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="ef67e-294">Event Hub</span></span>
* <span data-ttu-id="ef67e-295">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-295">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="ef67e-296">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="ef67e-296">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="ef67e-297">Extensiones</span><span class="sxs-lookup"><span data-stu-id="ef67e-297">Extensions</span></span>
* <span data-ttu-id="ef67e-298">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="ef67e-298">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="ef67e-299">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ef67e-299">HDInsight</span></span>
* <span data-ttu-id="ef67e-300">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="ef67e-300">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-301">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-301">IoT</span></span>
* <span data-ttu-id="ef67e-302">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="ef67e-302">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-303">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ef67e-303">KeyVault</span></span>
* <span data-ttu-id="ef67e-304">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="ef67e-304">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-305">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-305">Network</span></span>
* <span data-ttu-id="ef67e-306">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-306">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="ef67e-307">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="ef67e-307">See #6052</span></span>
* <span data-ttu-id="ef67e-308">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-308">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="ef67e-309">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="ef67e-309">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="ef67e-310">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="ef67e-310">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="ef67e-311">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="ef67e-311">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="ef67e-312">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="ef67e-312">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="ef67e-313">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-313">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-314">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-314">Role</span></span>
* <span data-ttu-id="ef67e-315">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="ef67e-315">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="ef67e-316">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="ef67e-316">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="ef67e-317">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="ef67e-317">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="ef67e-318">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="ef67e-318">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="ef67e-319">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="ef67e-319">Service Bus</span></span>
* <span data-ttu-id="ef67e-320">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="ef67e-320">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-321">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-321">VM</span></span>
* <span data-ttu-id="ef67e-322">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="ef67e-322">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="ef67e-323">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="ef67e-323">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="ef67e-324">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="ef67e-324">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="ef67e-325">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="ef67e-325">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="ef67e-326">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="ef67e-326">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="ef67e-327">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="ef67e-327">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="ef67e-328">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-328">September 21, 2018</span></span>

<span data-ttu-id="ef67e-329">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="ef67e-329">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-330">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-330">ACR</span></span>
* <span data-ttu-id="ef67e-331">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-331">Added ACR Task commands</span></span>
* <span data-ttu-id="ef67e-332">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="ef67e-332">Added quick run command</span></span>
* <span data-ttu-id="ef67e-333">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="ef67e-333">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="ef67e-334">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-334">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="ef67e-335">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="ef67e-335">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="ef67e-336">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="ef67e-336">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-337">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-337">ACS</span></span>
* <span data-ttu-id="ef67e-338">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="ef67e-338">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="ef67e-339">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="ef67e-339">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-340">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-340">AppService</span></span>

* <span data-ttu-id="ef67e-341">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="ef67e-341">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="ef67e-342">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="ef67e-342">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="ef67e-343">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="ef67e-343">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="ef67e-344">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="ef67e-344">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-345">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-345">Batch</span></span>
* <span data-ttu-id="ef67e-346">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="ef67e-346">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="ef67e-347">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="ef67e-347">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="ef67e-348">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-348">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="ef67e-349">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="ef67e-349">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef67e-350">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef67e-350">Batch AI</span></span> 
* <span data-ttu-id="ef67e-351">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-351">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef67e-352">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef67e-352">Cognitive Services</span></span>
* <span data-ttu-id="ef67e-353">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="ef67e-353">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="ef67e-354">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="ef67e-354">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="ef67e-355">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="ef67e-355">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="ef67e-356">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-356">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="ef67e-357">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-357">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="ef67e-358">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="ef67e-358">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-359">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-359">Container</span></span>
* <span data-ttu-id="ef67e-360">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="ef67e-360">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="ef67e-361">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="ef67e-361">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="ef67e-362">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-362">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="ef67e-363">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-363">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="ef67e-364">DataLake</span><span class="sxs-lookup"><span data-stu-id="ef67e-364">Datalake</span></span>
* <span data-ttu-id="ef67e-365">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-365">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="ef67e-366">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="ef67e-366">Interactive Shell</span></span>
* <span data-ttu-id="ef67e-367">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="ef67e-367">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="ef67e-368">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="ef67e-368">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-369">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-369">IoT</span></span>
* <span data-ttu-id="ef67e-370">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-370">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="ef67e-371">Key Vault</span><span class="sxs-lookup"><span data-stu-id="ef67e-371">Key Vault</span></span>
* <span data-ttu-id="ef67e-372">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="ef67e-372">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-373">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-373">Network</span></span>
* <span data-ttu-id="ef67e-374">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="ef67e-374">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="ef67e-375">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="ef67e-375">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="ef67e-376">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="ef67e-376">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="ef67e-377">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="ef67e-377">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="ef67e-378">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-378">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="ef67e-379">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-379">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="ef67e-380">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="ef67e-380">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="ef67e-381">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="ef67e-381">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="ef67e-382">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="ef67e-382">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="ef67e-383">`network express-route create/update`: se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="ef67e-383">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="ef67e-384">`network vnet subnet create/update`: se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="ef67e-384">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="ef67e-385">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-385">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="ef67e-386">`network traffic-manager profile create/update`: se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` a Monitor Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="ef67e-386">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="ef67e-387">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="ef67e-387">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="ef67e-388">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="ef67e-388">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="ef67e-389">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="ef67e-389">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="ef67e-390">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="ef67e-390">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="ef67e-391">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="ef67e-391">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-392">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-392">RDBMS</span></span>
* <span data-ttu-id="ef67e-393">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-393">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="ef67e-394">Reserva</span><span class="sxs-lookup"><span data-stu-id="ef67e-394">Reservation</span></span>
* <span data-ttu-id="ef67e-395">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="ef67e-395">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="ef67e-396">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-396">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="ef67e-397">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="ef67e-397">Manage App</span></span>
* <span data-ttu-id="ef67e-398">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="ef67e-398">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="ef67e-399">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="ef67e-399">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-400">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-400">Role</span></span>
* <span data-ttu-id="ef67e-401">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="ef67e-401">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="ef67e-402">SignalR</span><span class="sxs-lookup"><span data-stu-id="ef67e-402">SignalR</span></span>
* <span data-ttu-id="ef67e-403">Primera versión</span><span class="sxs-lookup"><span data-stu-id="ef67e-403">First release</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-404">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-404">Storage</span></span>
* <span data-ttu-id="ef67e-405">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="ef67e-405">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="ef67e-406">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="ef67e-406">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-407">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-407">VM</span></span>
* <span data-ttu-id="ef67e-408">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="ef67e-408">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="ef67e-409">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="ef67e-409">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="ef67e-410">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-410">August 28, 2018</span></span>

<span data-ttu-id="ef67e-411">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="ef67e-411">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-412">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-412">Core</span></span>

* <span data-ttu-id="ef67e-413">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="ef67e-413">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="ef67e-414">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="ef67e-414">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-415">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-415">ACR</span></span>

* <span data-ttu-id="ef67e-416">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="ef67e-416">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="ef67e-417">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="ef67e-417">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-418">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-418">ACS</span></span>

* <span data-ttu-id="ef67e-419">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="ef67e-419">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="ef67e-420">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="ef67e-420">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-421">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-421">AppService</span></span>

* <span data-ttu-id="ef67e-422">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="ef67e-422">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="ef67e-423">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-423">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="ef67e-424">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-424">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="ef67e-425">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="ef67e-425">Backup</span></span>

* <span data-ttu-id="ef67e-426">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-426">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="ef67e-427">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="ef67e-427">Bot Service</span></span>

* <span data-ttu-id="ef67e-428">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="ef67e-428">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef67e-429">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef67e-429">Cognitive Services</span></span>

* <span data-ttu-id="ef67e-430">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="ef67e-430">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-431">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-431">IoT</span></span>

* <span data-ttu-id="ef67e-432">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="ef67e-432">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-433">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-433">Monitor</span></span>

* <span data-ttu-id="ef67e-434">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="ef67e-434">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="ef67e-435">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="ef67e-435">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-436">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-436">Network</span></span>

* <span data-ttu-id="ef67e-437">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-437">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-438">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-438">Resource</span></span>

* <span data-ttu-id="ef67e-439">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-439">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-440">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-440">Storage</span></span>

* <span data-ttu-id="ef67e-441">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-441">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-442">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-442">VM</span></span>

* <span data-ttu-id="ef67e-443">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-443">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="ef67e-444">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-444">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="ef67e-445">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-445">Auguest 14, 2018</span></span>

<span data-ttu-id="ef67e-446">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="ef67e-446">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-447">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-447">Core</span></span>

* <span data-ttu-id="ef67e-448">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="ef67e-448">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="ef67e-449">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="ef67e-449">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="ef67e-450">Telemetría</span><span class="sxs-lookup"><span data-stu-id="ef67e-450">Telemetry</span></span>

* <span data-ttu-id="ef67e-451">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="ef67e-451">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-452">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-452">ACR</span></span>

* <span data-ttu-id="ef67e-453">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-453">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="ef67e-454">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="ef67e-454">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-455">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-455">ACS</span></span>

* <span data-ttu-id="ef67e-456">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="ef67e-456">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="ef67e-457">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="ef67e-457">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="ef67e-458">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="ef67e-458">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="ef67e-459">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="ef67e-459">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="ef67e-460">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="ef67e-460">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="ef67e-461">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-461">AppService</span></span>

* <span data-ttu-id="ef67e-462">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="ef67e-462">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="ef67e-463">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="ef67e-463">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="ef67e-464">BatchAI</span><span class="sxs-lookup"><span data-stu-id="ef67e-464">BatchAI</span></span>

* <span data-ttu-id="ef67e-465">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="ef67e-465">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="ef67e-466">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-466">Container</span></span>

* <span data-ttu-id="ef67e-467">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-467">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="ef67e-468">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-468">IoT</span></span>

* <span data-ttu-id="ef67e-469">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="ef67e-469">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="ef67e-470">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="ef67e-470">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="ef67e-471">Iot Central</span><span class="sxs-lookup"><span data-stu-id="ef67e-471">Iot Central</span></span>

* <span data-ttu-id="ef67e-472">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="ef67e-472">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-473">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ef67e-473">KeyVault</span></span>


* <span data-ttu-id="ef67e-474">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="ef67e-474">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="ef67e-475">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="ef67e-475">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="ef67e-476">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="ef67e-476">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="ef67e-477">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="ef67e-477">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="ef67e-478">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="ef67e-478">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="ef67e-479">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-479">Relay</span></span>

* <span data-ttu-id="ef67e-480">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="ef67e-480">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-481">Sql</span><span class="sxs-lookup"><span data-stu-id="ef67e-481">Sql</span></span>

* <span data-ttu-id="ef67e-482">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-482">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-483">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-483">Storage</span></span>

* <span data-ttu-id="ef67e-484">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="ef67e-484">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="ef67e-485">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="ef67e-485">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="ef67e-486">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="ef67e-486">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="ef67e-487">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="ef67e-487">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="ef67e-488">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-488">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-489">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-489">VM</span></span>

* <span data-ttu-id="ef67e-490">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="ef67e-490">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="ef67e-491">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-491">July 31, 2018</span></span>

<span data-ttu-id="ef67e-492">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="ef67e-492">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-493">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-493">ACR</span></span>

* <span data-ttu-id="ef67e-494">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-494">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="ef67e-495">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-495">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-496">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-496">ACS</span></span>

* <span data-ttu-id="ef67e-497">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="ef67e-497">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-498">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-498">Batch</span></span>

* <span data-ttu-id="ef67e-499">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="ef67e-499">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-500">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-500">Container</span></span>

* <span data-ttu-id="ef67e-501">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="ef67e-501">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-502">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-502">Network</span></span>

* <span data-ttu-id="ef67e-503">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ef67e-503">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="ef67e-504">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-504">Resource</span></span>

* <span data-ttu-id="ef67e-505">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="ef67e-505">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="ef67e-506">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="ef67e-506">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-507">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-507">Role</span></span>

* <span data-ttu-id="ef67e-508">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="ef67e-508">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="ef67e-509">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="ef67e-509">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="ef67e-510">Search</span><span class="sxs-lookup"><span data-stu-id="ef67e-510">Search</span></span>

* <span data-ttu-id="ef67e-511">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="ef67e-511">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="ef67e-512">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="ef67e-512">Service Bus</span></span>

* <span data-ttu-id="ef67e-513">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="ef67e-513">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="ef67e-514">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="ef67e-514">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="ef67e-515">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="ef67e-515">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="ef67e-516">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="ef67e-516">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-517">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-517">Storage</span></span>

* <span data-ttu-id="ef67e-518">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="ef67e-518">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="ef67e-519">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-519">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-520">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-520">VM</span></span>

* <span data-ttu-id="ef67e-521">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="ef67e-521">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="ef67e-522">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="ef67e-522">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="ef67e-523">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="ef67e-523">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="ef67e-524">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="ef67e-524">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="ef67e-525">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-525">July 18, 2018</span></span>

<span data-ttu-id="ef67e-526">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="ef67e-526">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-527">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-527">Core</span></span>

* <span data-ttu-id="ef67e-528">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="ef67e-528">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="ef67e-529">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="ef67e-529">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="ef67e-530">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-530">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-531">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-531">ACR</span></span>

* <span data-ttu-id="ef67e-532">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="ef67e-532">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="ef67e-533">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="ef67e-533">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="ef67e-534">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="ef67e-534">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="ef67e-535">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="ef67e-535">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-536">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-536">ACS</span></span>

* <span data-ttu-id="ef67e-537">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="ef67e-537">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-538">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-538">AppService</span></span>

* <span data-ttu-id="ef67e-539">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="ef67e-539">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-540">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-540">Batch</span></span>

* <span data-ttu-id="ef67e-541">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="ef67e-541">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="ef67e-542">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="ef67e-542">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef67e-543">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef67e-543">Batch AI</span></span>

* <span data-ttu-id="ef67e-544">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="ef67e-544">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-545">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-545">Container</span></span>

* <span data-ttu-id="ef67e-546">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="ef67e-546">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="ef67e-547">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="ef67e-547">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-548">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-548">Network</span></span>

* <span data-ttu-id="ef67e-549">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-549">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="ef67e-550">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-550">Added `network nic wait`</span></span>
* <span data-ttu-id="ef67e-551">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="ef67e-551">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="ef67e-552">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-552">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="ef67e-553">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-553">Resource</span></span>

* <span data-ttu-id="ef67e-554">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="ef67e-554">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="ef67e-555">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="ef67e-555">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="ef67e-556">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-556">Added `deployment wait` command</span></span>
* <span data-ttu-id="ef67e-557">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="ef67e-557">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-558">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-558">SQL</span></span>

* <span data-ttu-id="ef67e-559">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-559">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="ef67e-560">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="ef67e-560">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="ef67e-561">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="ef67e-561">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-562">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-562">Storage</span></span>

* <span data-ttu-id="ef67e-563">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="ef67e-563">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-564">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-564">VM</span></span>

* <span data-ttu-id="ef67e-565">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="ef67e-565">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="ef67e-566">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-566">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="ef67e-567">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-567">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ef67e-568">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-568">July 3, 2018</span></span>

<span data-ttu-id="ef67e-569">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="ef67e-569">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="ef67e-570">AKS</span><span class="sxs-lookup"><span data-stu-id="ef67e-570">AKS</span></span>

* <span data-ttu-id="ef67e-571">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="ef67e-571">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ef67e-572">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-572">July 3, 2018</span></span>

<span data-ttu-id="ef67e-573">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="ef67e-573">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-574">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-574">Core</span></span>

* <span data-ttu-id="ef67e-575">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="ef67e-575">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-576">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-576">ACR</span></span>

* <span data-ttu-id="ef67e-577">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="ef67e-577">Added polling build status</span></span>
* <span data-ttu-id="ef67e-578">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="ef67e-578">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="ef67e-579">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="ef67e-579">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-580">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-580">ACS</span></span>

* <span data-ttu-id="ef67e-581">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-581">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="ef67e-582">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="ef67e-582">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="ef67e-583">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-583">Updated options for `aks browse` command.</span></span> <span data-ttu-id="ef67e-584">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="ef67e-584">Added `--listen-port` support</span></span>
* <span data-ttu-id="ef67e-585">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-585">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="ef67e-586">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="ef67e-586">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="ef67e-587">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="ef67e-587">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-588">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-588">AppService</span></span>

* <span data-ttu-id="ef67e-589">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="ef67e-589">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="ef67e-590">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="ef67e-590">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="ef67e-591">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="ef67e-591">Backup</span></span>

* <span data-ttu-id="ef67e-592">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="ef67e-592">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="ef67e-593">BatchAI</span><span class="sxs-lookup"><span data-stu-id="ef67e-593">BatchAI</span></span>

* <span data-ttu-id="ef67e-594">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-594">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="ef67e-595">Nube</span><span class="sxs-lookup"><span data-stu-id="ef67e-595">Cloud</span></span>

* <span data-ttu-id="ef67e-596">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="ef67e-596">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-597">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-597">Container</span></span>

* <span data-ttu-id="ef67e-598">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="ef67e-598">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="ef67e-599">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="ef67e-599">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="ef67e-600">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="ef67e-600">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-601">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-601">Extension</span></span>

* <span data-ttu-id="ef67e-602">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="ef67e-602">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-603">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-603">Network</span></span>

* <span data-ttu-id="ef67e-604">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="ef67e-604">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-605">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ef67e-605">Rdbms</span></span>

* <span data-ttu-id="ef67e-606">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-606">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-607">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-607">Resource</span></span>

* <span data-ttu-id="ef67e-608">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="ef67e-608">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-609">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-609">VM</span></span>

* <span data-ttu-id="ef67e-610">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="ef67e-610">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="ef67e-611">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-611">June 25, 2018</span></span>

<span data-ttu-id="ef67e-612">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="ef67e-612">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="ef67e-613">CLI</span><span class="sxs-lookup"><span data-stu-id="ef67e-613">CLI</span></span>

* <span data-ttu-id="ef67e-614">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-614">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="ef67e-615">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-615">June 19, 2018</span></span>

<span data-ttu-id="ef67e-616">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="ef67e-616">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-617">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-617">Core</span></span>

* <span data-ttu-id="ef67e-618">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-618">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-619">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-619">ACR</span></span>

* <span data-ttu-id="ef67e-620">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="ef67e-620">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="ef67e-621">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="ef67e-621">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-622">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-622">ACS</span></span>

* <span data-ttu-id="ef67e-623">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-623">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="ef67e-624">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-624">Added `--update` support</span></span>
* <span data-ttu-id="ef67e-625">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="ef67e-625">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="ef67e-626">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="ef67e-626">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="ef67e-627">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="ef67e-627">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="ef67e-628">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="ef67e-628">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="ef67e-629">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="ef67e-629">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="ef67e-630">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="ef67e-630">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-631">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-631">AppService</span></span>

* <span data-ttu-id="ef67e-632">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="ef67e-632">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="ef67e-633">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="ef67e-633">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-634">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-634">Batch</span></span>

* <span data-ttu-id="ef67e-635">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="ef67e-635">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef67e-636">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef67e-636">Batch AI</span></span>

* <span data-ttu-id="ef67e-637">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="ef67e-637">Added support for workspaces.</span></span> <span data-ttu-id="ef67e-638">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="ef67e-638">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="ef67e-639">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-639">Added support for experiments.</span></span> <span data-ttu-id="ef67e-640">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="ef67e-640">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="ef67e-641">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="ef67e-641">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="ef67e-642">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-642">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="ef67e-643">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-643">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="ef67e-644">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-644">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="ef67e-645">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="ef67e-645">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="ef67e-646">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-646">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="ef67e-647">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-647">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="ef67e-648">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-648">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="ef67e-649">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-649">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="ef67e-650">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-650">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="ef67e-651">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-651">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="ef67e-652">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="ef67e-652">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="ef67e-653">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-653">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="ef67e-654">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="ef67e-654">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="ef67e-655">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="ef67e-655">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="ef67e-656">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="ef67e-656">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ef67e-657">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="ef67e-657">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="ef67e-658">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="ef67e-658">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="ef67e-659">Mapas</span><span class="sxs-lookup"><span data-stu-id="ef67e-659">Maps</span></span>

* <span data-ttu-id="ef67e-660">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-660">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-661">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-661">Network</span></span>

* <span data-ttu-id="ef67e-662">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="ef67e-662">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="ef67e-663">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-663">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="ef67e-664">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="ef67e-664">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="ef67e-665">Reservations</span><span class="sxs-lookup"><span data-stu-id="ef67e-665">Reservations</span></span>

* <span data-ttu-id="ef67e-666">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-666">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="ef67e-667">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-667">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="ef67e-668">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-668">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="ef67e-669">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-669">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="ef67e-670">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-670">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="ef67e-671">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-671">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-672">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-672">Role</span></span>

* <span data-ttu-id="ef67e-673">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="ef67e-673">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-674">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-674">SQL</span></span>

* <span data-ttu-id="ef67e-675">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="ef67e-675">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-676">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-676">Storage</span></span>

* <span data-ttu-id="ef67e-677">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="ef67e-677">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-678">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-678">VM</span></span>

* <span data-ttu-id="ef67e-679">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-679">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="ef67e-680">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="ef67e-680">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="ef67e-681">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="ef67e-681">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ef67e-682">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-682">June 13, 2018</span></span>

<span data-ttu-id="ef67e-683">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="ef67e-683">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-684">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-684">Core</span></span>

* <span data-ttu-id="ef67e-685">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="ef67e-685">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ef67e-686">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-686">June 13, 2018</span></span>

<span data-ttu-id="ef67e-687">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="ef67e-687">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="ef67e-688">AKS</span><span class="sxs-lookup"><span data-stu-id="ef67e-688">AKS</span></span>

* <span data-ttu-id="ef67e-689">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-689">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="ef67e-690">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="ef67e-690">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="ef67e-691">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-691">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="ef67e-692">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-692">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="ef67e-693">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-693">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-694">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-694">AppService</span></span>

* <span data-ttu-id="ef67e-695">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="ef67e-695">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ef67e-696">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-696">June 5, 2018</span></span>

<span data-ttu-id="ef67e-697">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="ef67e-697">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-698">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-698">Interactive</span></span>

* <span data-ttu-id="ef67e-699">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="ef67e-699">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ef67e-700">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-700">June 5, 2018</span></span>

<span data-ttu-id="ef67e-701">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="ef67e-701">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-702">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-702">Core</span></span>

* <span data-ttu-id="ef67e-703">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="ef67e-703">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="ef67e-704">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="ef67e-704">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-705">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-705">ACR</span></span>

* <span data-ttu-id="ef67e-706">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="ef67e-706">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="ef67e-707">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-707">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="ef67e-708">AKS</span><span class="sxs-lookup"><span data-stu-id="ef67e-708">AKS</span></span>

* <span data-ttu-id="ef67e-709">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="ef67e-709">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-710">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-710">Batch</span></span>

* <span data-ttu-id="ef67e-711">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="ef67e-711">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-712">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-712">IOT</span></span>

* <span data-ttu-id="ef67e-713">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="ef67e-713">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-714">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-714">Network</span></span>

* <span data-ttu-id="ef67e-715">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="ef67e-715">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ef67e-716">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="ef67e-716">Policy Insights</span></span>

* <span data-ttu-id="ef67e-717">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="ef67e-717">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="ef67e-718">ARM</span><span class="sxs-lookup"><span data-stu-id="ef67e-718">ARM</span></span>

* <span data-ttu-id="ef67e-719">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-719">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-720">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-720">SQL</span></span>

* <span data-ttu-id="ef67e-721">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="ef67e-721">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="ef67e-722">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="ef67e-722">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="ef67e-723">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-723">Storage</span></span>

* <span data-ttu-id="ef67e-724">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="ef67e-724">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-725">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-725">VM</span></span>

* <span data-ttu-id="ef67e-726">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="ef67e-726">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="ef67e-727">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-727">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="ef67e-728">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-728">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="ef67e-729">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-729">May 22, 2018</span></span>

<span data-ttu-id="ef67e-730">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="ef67e-730">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-731">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-731">Core</span></span>

* <span data-ttu-id="ef67e-732">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="ef67e-732">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-733">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-733">ACS</span></span>

* <span data-ttu-id="ef67e-734">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="ef67e-734">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="ef67e-735">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="ef67e-735">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-736">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-736">AppService</span></span>

* <span data-ttu-id="ef67e-737">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="ef67e-737">Improved generic update commands</span></span>
* <span data-ttu-id="ef67e-738">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="ef67e-738">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-739">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-739">Container</span></span>

* <span data-ttu-id="ef67e-740">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="ef67e-740">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="ef67e-741">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-741">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-742">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-742">Extension</span></span>

* <span data-ttu-id="ef67e-743">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="ef67e-743">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-744">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-744">Interactive</span></span>

* <span data-ttu-id="ef67e-745">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="ef67e-745">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="ef67e-746">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="ef67e-746">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-747">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ef67e-747">KeyVault</span></span>

* <span data-ttu-id="ef67e-748">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="ef67e-748">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-749">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-749">Network</span></span>

* <span data-ttu-id="ef67e-750">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="ef67e-750">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="ef67e-751">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="ef67e-751">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-752">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-752">SQL</span></span>

* <span data-ttu-id="ef67e-753">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="ef67e-753">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="ef67e-754">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="ef67e-754">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="ef67e-755">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="ef67e-755">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="ef67e-756">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="ef67e-756">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="ef67e-757">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="ef67e-757">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="ef67e-758">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-758">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="ef67e-759">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="ef67e-759">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="ef67e-760">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-760">`edition`.</span></span> <span data-ttu-id="ef67e-761">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="ef67e-761">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="ef67e-762">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-762">`elasticPoolName`.</span></span> <span data-ttu-id="ef67e-763">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="ef67e-763">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="ef67e-764">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="ef67e-764">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="ef67e-765">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-765">`edition`.</span></span> <span data-ttu-id="ef67e-766">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="ef67e-766">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="ef67e-767">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-767">`dtu`.</span></span> <span data-ttu-id="ef67e-768">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="ef67e-768">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="ef67e-769">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-769">`databaseDtuMin`.</span></span> <span data-ttu-id="ef67e-770">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="ef67e-770">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="ef67e-771">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-771">`databaseDtuMax`.</span></span> <span data-ttu-id="ef67e-772">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="ef67e-772">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="ef67e-773">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-773">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="ef67e-774">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-774">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-775">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-775">Storage</span></span>

* <span data-ttu-id="ef67e-776">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="ef67e-776">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="ef67e-777">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="ef67e-777">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-778">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-778">VM</span></span>

* <span data-ttu-id="ef67e-779">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-779">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="ef67e-780">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="ef67e-780">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="ef67e-781">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="ef67e-781">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="ef67e-782">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="ef67e-782">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="ef67e-783">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-783">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="ef67e-784">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-784">May 7, 2018</span></span>

<span data-ttu-id="ef67e-785">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="ef67e-785">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-786">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-786">Core</span></span>

* <span data-ttu-id="ef67e-787">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="ef67e-787">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="ef67e-788">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="ef67e-788">Added limited support for positional arguments</span></span>
* <span data-ttu-id="ef67e-789">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-789">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="ef67e-790">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="ef67e-790">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="ef67e-791">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-791">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="ef67e-792">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="ef67e-792">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="ef67e-793">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-793">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="ef67e-794">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="ef67e-794">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="ef67e-795">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-795">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-796">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-796">ACR</span></span>

* <span data-ttu-id="ef67e-797">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="ef67e-797">Added ACR Build commands</span></span>
* <span data-ttu-id="ef67e-798">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="ef67e-798">Improved resource not found error messages</span></span>
* <span data-ttu-id="ef67e-799">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="ef67e-799">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="ef67e-800">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="ef67e-800">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="ef67e-801">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-801">Improved repository commands error messages</span></span>
* <span data-ttu-id="ef67e-802">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="ef67e-802">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-803">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-803">ACS</span></span>

* <span data-ttu-id="ef67e-804">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-804">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="ef67e-805">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="ef67e-805">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="ef67e-806">AMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-806">AMS</span></span>

* <span data-ttu-id="ef67e-807">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="ef67e-807">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-808">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-808">Appservice</span></span>

* <span data-ttu-id="ef67e-809">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="ef67e-809">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="ef67e-810">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-810">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="ef67e-811">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="ef67e-811">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="ef67e-812">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-812">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ef67e-813">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef67e-813">Batch AI</span></span>

* <span data-ttu-id="ef67e-814">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="ef67e-814">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef67e-815">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef67e-815">Cognitive Services</span></span>

* <span data-ttu-id="ef67e-816">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="ef67e-816">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="ef67e-817">Consumo</span><span class="sxs-lookup"><span data-stu-id="ef67e-817">Consumption</span></span>

* <span data-ttu-id="ef67e-818">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="ef67e-818">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-819">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-819">Container</span></span>

* <span data-ttu-id="ef67e-820">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="ef67e-820">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ef67e-821">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef67e-821">Cosmos DB</span></span>

* <span data-ttu-id="ef67e-822">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ef67e-822">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="ef67e-823">DMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-823">DMS</span></span>

* <span data-ttu-id="ef67e-824">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-824">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-825">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-825">Extension</span></span>

* <span data-ttu-id="ef67e-826">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="ef67e-826">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-827">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-827">Interactive</span></span>

* <span data-ttu-id="ef67e-828">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="ef67e-828">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="ef67e-829">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="ef67e-829">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="ef67e-830">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="ef67e-830">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="ef67e-831">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-831">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="ef67e-832">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-832">Lab</span></span>

* <span data-ttu-id="ef67e-833">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="ef67e-833">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-834">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-834">Network</span></span>

* <span data-ttu-id="ef67e-835">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="ef67e-835">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="ef67e-836">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-836">Profile</span></span>

* <span data-ttu-id="ef67e-837">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-837">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="ef67e-838">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="ef67e-838">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="ef67e-839">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="ef67e-839">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="ef67e-840">Redis</span><span class="sxs-lookup"><span data-stu-id="ef67e-840">Redis</span></span>

* <span data-ttu-id="ef67e-841">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="ef67e-841">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="ef67e-842">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-842">Deprecated `redis list-all`.</span></span> <span data-ttu-id="ef67e-843">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-843">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="ef67e-844">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="ef67e-844">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="ef67e-845">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-845">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-846">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-846">Role</span></span>

* <span data-ttu-id="ef67e-847">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="ef67e-847">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-848">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-848">Storage</span></span>

* <span data-ttu-id="ef67e-849">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="ef67e-849">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="ef67e-850">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="ef67e-850">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="ef67e-851">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="ef67e-851">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="ef67e-852">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="ef67e-852">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="ef67e-853">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="ef67e-853">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-854">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-854">VM</span></span>

* <span data-ttu-id="ef67e-855">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="ef67e-855">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="ef67e-856">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="ef67e-856">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="ef67e-857">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="ef67e-857">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="ef67e-858">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="ef67e-858">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="ef67e-859">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="ef67e-859">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="ef67e-860">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="ef67e-860">Added write accelerator support</span></span>
* <span data-ttu-id="ef67e-861">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-861">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="ef67e-862">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="ef67e-862">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="ef67e-863">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="ef67e-863">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="ef67e-864">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-864">April 10, 2018</span></span>

<span data-ttu-id="ef67e-865">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="ef67e-865">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-866">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-866">ACR</span></span>

* <span data-ttu-id="ef67e-867">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="ef67e-867">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-868">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-868">ACS</span></span>

* <span data-ttu-id="ef67e-869">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="ef67e-869">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-870">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-870">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="ef67e-872">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="ef67e-872">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="ef67e-873">BatchAI</span><span class="sxs-lookup"><span data-stu-id="ef67e-873">BatchAI</span></span>

* <span data-ttu-id="ef67e-874">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="ef67e-874">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="ef67e-875">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="ef67e-875">Job level mounting</span></span>
  - <span data-ttu-id="ef67e-876">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="ef67e-876">Environment variables with secret values</span></span>
  - <span data-ttu-id="ef67e-877">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="ef67e-877">Performance counters settings</span></span>
  - <span data-ttu-id="ef67e-878">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="ef67e-878">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="ef67e-879">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="ef67e-879">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="ef67e-880">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="ef67e-880">Usage and limits reporting</span></span>
  - <span data-ttu-id="ef67e-881">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="ef67e-881">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="ef67e-882">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="ef67e-882">Support for custom images</span></span>
  - <span data-ttu-id="ef67e-883">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="ef67e-883">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="ef67e-884">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="ef67e-884">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="ef67e-885">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="ef67e-885">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="ef67e-886">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="ef67e-886">National clouds are supported</span></span>
* <span data-ttu-id="ef67e-887">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="ef67e-887">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="ef67e-888">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="ef67e-888">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="ef67e-889">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="ef67e-889">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="ef67e-890">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="ef67e-890">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="ef67e-891">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="ef67e-891">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="ef67e-892">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="ef67e-892">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="ef67e-893">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-893">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="ef67e-894">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="ef67e-894">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="ef67e-895">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="ef67e-895">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="ef67e-896">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-896">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="ef67e-897">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-897">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="ef67e-898">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="ef67e-898">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="ef67e-899">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-899">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="ef67e-900">Facturación</span><span class="sxs-lookup"><span data-stu-id="ef67e-900">Billing</span></span>

* <span data-ttu-id="ef67e-901">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="ef67e-901">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="ef67e-902">Consumo</span><span class="sxs-lookup"><span data-stu-id="ef67e-902">Consumption</span></span>

* <span data-ttu-id="ef67e-903">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-903">Added `marketplace` commands</span></span>
* <span data-ttu-id="ef67e-904">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="ef67e-904">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="ef67e-905">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="ef67e-905">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="ef67e-906">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="ef67e-906">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="ef67e-907">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="ef67e-907">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="ef67e-908">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="ef67e-908">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-909">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-909">Container</span></span>

* <span data-ttu-id="ef67e-910">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="ef67e-910">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="ef67e-911">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="ef67e-911">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-912">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-912">Extension</span></span>

* <span data-ttu-id="ef67e-913">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="ef67e-913">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-914">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-914">Interactive</span></span>

* <span data-ttu-id="ef67e-915">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="ef67e-915">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="ef67e-916">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-916">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="ef67e-917">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="ef67e-917">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-918">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-918">Network</span></span>

* <span data-ttu-id="ef67e-919">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-919">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="ef67e-920">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-920">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="ef67e-921">4910</span><span class="sxs-lookup"><span data-stu-id="ef67e-921">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="ef67e-922">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="ef67e-922">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="ef67e-923">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="ef67e-923">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="ef67e-924">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-924">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="ef67e-925">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-925">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="ef67e-926">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="ef67e-926">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-927">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-927">Profile</span></span>

* <span data-ttu-id="ef67e-928">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-928">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="ef67e-929">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="ef67e-929">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-930">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-930">RDBMS</span></span>

* <span data-ttu-id="ef67e-931">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-931">Added `georestore` command</span></span>
* <span data-ttu-id="ef67e-932">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-932">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-933">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-933">Resource</span></span>

* <span data-ttu-id="ef67e-934">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-934">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="ef67e-935">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-935">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-936">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-936">SQL</span></span>

* <span data-ttu-id="ef67e-937">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="ef67e-937">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-938">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-938">Storage</span></span>

* <span data-ttu-id="ef67e-939">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="ef67e-939">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-940">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-940">VM</span></span>

* <span data-ttu-id="ef67e-941">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-941">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="ef67e-942">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="ef67e-942">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="ef67e-944">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-944">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="ef67e-945">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="ef67e-945">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="ef67e-946">5718</span><span class="sxs-lookup"><span data-stu-id="ef67e-946">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="ef67e-947">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="ef67e-947">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="ef67e-948">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-948">March 27, 2018</span></span>

<span data-ttu-id="ef67e-949">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="ef67e-949">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-950">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-950">Core</span></span>

* <span data-ttu-id="ef67e-951">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="ef67e-951">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-952">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-952">ACS</span></span>

* <span data-ttu-id="ef67e-953">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="ef67e-953">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-954">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-954">Appservice</span></span>

* <span data-ttu-id="ef67e-955">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-955">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="ef67e-956">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-956">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ef67e-957">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="ef67e-957">Backup</span></span>

* <span data-ttu-id="ef67e-958">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-958">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="ef67e-959">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-959">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="ef67e-960">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="ef67e-960">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="ef67e-961">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="ef67e-961">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-962">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-962">Container</span></span>

* <span data-ttu-id="ef67e-963">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-963">Added `container exec` command.</span></span> <span data-ttu-id="ef67e-964">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="ef67e-964">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="ef67e-965">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-965">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-966">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-966">Extension</span></span>

* <span data-ttu-id="ef67e-967">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-967">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="ef67e-968">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="ef67e-968">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="ef67e-969">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="ef67e-969">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-970">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-970">Interactive</span></span>

* <span data-ttu-id="ef67e-971">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-971">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="ef67e-972">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="ef67e-972">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="ef67e-973">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-973">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="ef67e-974">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="ef67e-974">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="ef67e-975">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-975">Lab</span></span>

* <span data-ttu-id="ef67e-976">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="ef67e-976">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-977">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-977">Monitor</span></span>

* <span data-ttu-id="ef67e-978">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="ef67e-978">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="ef67e-979">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="ef67e-979">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="ef67e-980">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="ef67e-980">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-981">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-981">Network</span></span>

* <span data-ttu-id="ef67e-982">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="ef67e-982">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-983">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-983">Profile</span></span>

* <span data-ttu-id="ef67e-984">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="ef67e-984">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-985">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-985">RDBMS</span></span>

* <span data-ttu-id="ef67e-986">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="ef67e-986">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-987">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-987">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="ef67e-989">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-989">Role</span></span>

* <span data-ttu-id="ef67e-990">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-990">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="ef67e-991">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="ef67e-991">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="ef67e-992">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-992">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="ef67e-993">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-993">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="ef67e-994">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="ef67e-994">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-995">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-995">Storage</span></span>

* <span data-ttu-id="ef67e-996">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="ef67e-996">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="ef67e-997">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="ef67e-997">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-998">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-998">VM</span></span>

* <span data-ttu-id="ef67e-999">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="ef67e-999">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="ef67e-1000">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1000">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="ef67e-1001">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="ef67e-1001">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="ef67e-1002">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="ef67e-1002">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="ef67e-1003">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-1003">March 13, 2018</span></span>

<span data-ttu-id="ef67e-1004">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="ef67e-1004">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-1005">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-1005">ACR</span></span>

* <span data-ttu-id="ef67e-1006">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1006">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="ef67e-1007">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1007">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="ef67e-1008">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1008">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1009">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1009">ACS</span></span>

* <span data-ttu-id="ef67e-1010">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1010">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="ef67e-1011">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1011">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="ef67e-1012">Advisor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1012">Advisor</span></span>

* <span data-ttu-id="ef67e-1013">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1013">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="ef67e-1014">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1014">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="ef67e-1015">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1015">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="ef67e-1016">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1016">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="ef67e-1017">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1017">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1018">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1018">Appservice</span></span>

* <span data-ttu-id="ef67e-1019">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1019">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="ef67e-1020">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1020">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ef67e-1021">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="ef67e-1021">Eventhubs</span></span>

* <span data-ttu-id="ef67e-1022">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1022">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-1023">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1023">Extension</span></span>

* <span data-ttu-id="ef67e-1024">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1024">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-1025">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-1025">Interactive</span></span>

* <span data-ttu-id="ef67e-1026">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1026">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="ef67e-1027">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1027">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="ef67e-1028">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1028">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="ef67e-1029">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1029">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1030">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1030">Monitor</span></span>

* <span data-ttu-id="ef67e-1031">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1031">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="ef67e-1032">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1032">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="ef67e-1033">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1033">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="ef67e-1034">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1034">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1035">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1035">Network</span></span>

* <span data-ttu-id="ef67e-1036">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1036">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="ef67e-1037">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1037">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="ef67e-1038">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1038">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="ef67e-1039">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1039">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-1040">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1040">Profile</span></span>

* <span data-ttu-id="ef67e-1041">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1041">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="ef67e-1042">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1042">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-1043">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1043">RDBMS</span></span>

* <span data-ttu-id="ef67e-1044">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="ef67e-1044">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="ef67e-1045">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="ef67e-1045">Service Bus</span></span>

* <span data-ttu-id="ef67e-1046">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1046">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1047">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1047">Storage</span></span>

* <span data-ttu-id="ef67e-1048">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1048">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="ef67e-1049">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1049">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1050">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1050">VM</span></span>

* <span data-ttu-id="ef67e-1051">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1051">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="ef67e-1052">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1052">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="ef67e-1053">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1053">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="ef67e-1054">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1054">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="ef67e-1055">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-1055">February 27, 2018</span></span>

<span data-ttu-id="ef67e-1056">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="ef67e-1056">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-1057">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1057">Core</span></span>

* <span data-ttu-id="ef67e-1058">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="ef67e-1058">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="ef67e-1059">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1059">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="ef67e-1060">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1060">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1061">ACS</span></span>

* <span data-ttu-id="ef67e-1062">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="ef67e-1062">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="ef67e-1063">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="ef67e-1063">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="ef67e-1064">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1064">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="ef67e-1065">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1065">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1066">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1066">Appservice</span></span>

* <span data-ttu-id="ef67e-1067">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1067">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="ef67e-1068">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="ef67e-1068">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ef67e-1069">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef67e-1069">Cognitive Services</span></span>

* <span data-ttu-id="ef67e-1070">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef67e-1070">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="ef67e-1071">Consumo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1071">Consumption</span></span>

* <span data-ttu-id="ef67e-1072">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="ef67e-1072">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="ef67e-1073">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="ef67e-1073">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-1074">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1074">Container</span></span>

* <span data-ttu-id="ef67e-1075">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="ef67e-1075">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1076">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1076">Network</span></span>

* <span data-ttu-id="ef67e-1077">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1077">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1078">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1078">Resource</span></span>

* <span data-ttu-id="ef67e-1079">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="ef67e-1079">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-1080">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-1080">Role</span></span>

* <span data-ttu-id="ef67e-1081">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1081">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1082">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1082">SQL</span></span>

* <span data-ttu-id="ef67e-1083">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="ef67e-1083">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1084">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1084">Storage</span></span>

* <span data-ttu-id="ef67e-1085">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1085">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1086">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1086">VM</span></span>

* <span data-ttu-id="ef67e-1087">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1087">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="ef67e-1088">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-1088">February 13, 2018</span></span>

<span data-ttu-id="ef67e-1089">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="ef67e-1089">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-1090">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1090">Core</span></span>

* <span data-ttu-id="ef67e-1091">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="ef67e-1091">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1092">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1092">ACS</span></span>

* <span data-ttu-id="ef67e-1093">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1093">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="ef67e-1094">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1094">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="ef67e-1095">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="ef67e-1095">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="ef67e-1096">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1096">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="ef67e-1097">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1097">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="ef67e-1098">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1098">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="ef67e-1099">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="ef67e-1099">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="ef67e-1100">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1100">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1101">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1101">Appservice</span></span>

* <span data-ttu-id="ef67e-1102">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="ef67e-1102">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="ef67e-1103">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1103">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="ef67e-1104">CDN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1104">CDN</span></span>

* <span data-ttu-id="ef67e-1105">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1105">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-1106">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1106">Container</span></span>

* <span data-ttu-id="ef67e-1107">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="ef67e-1107">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="ef67e-1108">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-1108">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef67e-1109">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-1109">CosmosDB</span></span>

* <span data-ttu-id="ef67e-1110">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="ef67e-1110">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-1111">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1111">Extension</span></span>

* <span data-ttu-id="ef67e-1112">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1112">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="ef67e-1113">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1113">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="ef67e-1114">Comentarios</span><span class="sxs-lookup"><span data-stu-id="ef67e-1114">Feedback</span></span>

* <span data-ttu-id="ef67e-1115">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="ef67e-1115">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-1116">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-1116">Interactive</span></span>

* <span data-ttu-id="ef67e-1117">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="ef67e-1117">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="ef67e-1118">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="ef67e-1118">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-1119">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-1119">IoT</span></span>

* <span data-ttu-id="ef67e-1120">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1120">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ef67e-1121">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1121">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ef67e-1122">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1122">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="ef67e-1123">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="ef67e-1123">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1124">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1124">Monitor</span></span>

* <span data-ttu-id="ef67e-1125">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1125">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1126">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1126">Network</span></span>

* <span data-ttu-id="ef67e-1127">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1127">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="ef67e-1128">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1128">Profile</span></span>

* <span data-ttu-id="ef67e-1129">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1129">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1130">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1130">Resource</span></span>

* <span data-ttu-id="ef67e-1131">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1131">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-1132">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-1132">Role</span></span>

* <span data-ttu-id="ef67e-1133">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1133">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1134">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1134">SQL</span></span>

* <span data-ttu-id="ef67e-1135">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1135">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="ef67e-1136">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1136">Added `sql db rename`</span></span>
* <span data-ttu-id="ef67e-1137">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="ef67e-1137">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1138">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1138">Storage</span></span>

* <span data-ttu-id="ef67e-1139">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="ef67e-1139">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1140">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1140">VM</span></span>

* <span data-ttu-id="ef67e-1141">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="ef67e-1141">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="ef67e-1142">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="ef67e-1142">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="ef67e-1143">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="ef67e-1143">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="ef67e-1144">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-1144">January 31, 2018</span></span>

<span data-ttu-id="ef67e-1145">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="ef67e-1145">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-1146">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1146">Core</span></span>

* <span data-ttu-id="ef67e-1147">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="ef67e-1147">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="ef67e-1148">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="ef67e-1148">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="ef67e-1149">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1149">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="ef67e-1150">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1150">Use `--verbose` to see</span></span>
* <span data-ttu-id="ef67e-1151">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="ef67e-1151">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1152">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1152">ACS</span></span>

* <span data-ttu-id="ef67e-1153">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1153">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="ef67e-1154">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1154">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1155">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1155">Appservice</span></span>

* <span data-ttu-id="ef67e-1156">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="ef67e-1156">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="ef67e-1157">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="ef67e-1157">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="ef67e-1158">CDN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1158">CDN</span></span>

* <span data-ttu-id="ef67e-1159">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1159">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef67e-1160">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-1160">CosmosDB</span></span>

* <span data-ttu-id="ef67e-1161">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="ef67e-1161">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-1162">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-1162">Interactive</span></span>

* <span data-ttu-id="ef67e-1163">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="ef67e-1163">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1164">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1164">Network</span></span>

* <span data-ttu-id="ef67e-1165">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1165">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="ef67e-1166">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="ef67e-1166">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="ef67e-1167">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1167">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="ef67e-1168">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1168">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="ef67e-1169">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1169">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="ef67e-1170">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1170">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="ef67e-1171">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1171">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="ef67e-1172">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="ef67e-1172">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="ef67e-1173">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1173">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="ef67e-1174">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1174">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-1175">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1175">Profile</span></span>

* <span data-ttu-id="ef67e-1176">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="ef67e-1176">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1177">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1177">Resource</span></span>

* <span data-ttu-id="ef67e-1178">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1178">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1179">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1179">Storage</span></span>

* <span data-ttu-id="ef67e-1180">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="ef67e-1180">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="ef67e-1181">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="ef67e-1181">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="ef67e-1182">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1182">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="ef67e-1183">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1183">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="ef67e-1184">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="ef67e-1184">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1185">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1185">VM</span></span>

* <span data-ttu-id="ef67e-1186">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="ef67e-1186">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="ef67e-1187">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1187">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="ef67e-1188">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="ef67e-1188">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="ef67e-1189">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1189">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="ef67e-1190">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="ef67e-1190">January 17, 2018</span></span>

<span data-ttu-id="ef67e-1191">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="ef67e-1191">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-1192">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-1192">ACR</span></span>

* <span data-ttu-id="ef67e-1193">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="ef67e-1193">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="ef67e-1194">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="ef67e-1194">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1195">ACS</span></span>

* <span data-ttu-id="ef67e-1196">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1196">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="ef67e-1197">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1197">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1198">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1198">Appservice</span></span>

* <span data-ttu-id="ef67e-1199">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1199">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="ef67e-1200">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1200">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="ef67e-1201">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1201">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="ef67e-1202">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="ef67e-1202">Backup</span></span>

* <span data-ttu-id="ef67e-1203">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="ef67e-1203">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="ef67e-1204">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1204">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="ef67e-1205">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1205">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="ef67e-1206">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="ef67e-1206">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="ef67e-1207">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="ef67e-1207">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-1208">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-1208">Batch</span></span>

* <span data-ttu-id="ef67e-1209">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="ef67e-1209">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="ef67e-1210">Nube</span><span class="sxs-lookup"><span data-stu-id="ef67e-1210">Cloud</span></span>

* <span data-ttu-id="ef67e-1211">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="ef67e-1211">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="ef67e-1212">Consumo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1212">Consumption</span></span>

* <span data-ttu-id="ef67e-1213">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1213">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="ef67e-1214">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ef67e-1214">Event Grid</span></span>

* <span data-ttu-id="ef67e-1215">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1215">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ef67e-1216">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1216">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ef67e-1217">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1217">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="ef67e-1218">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1218">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="ef67e-1219">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1219">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="ef67e-1220">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1220">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="ef67e-1221">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1221">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="ef67e-1222">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="ef67e-1222">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-1223">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-1223">Interactive</span></span>

* <span data-ttu-id="ef67e-1224">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="ef67e-1224">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="ef67e-1225">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1225">Fixed errors on startup</span></span>
* <span data-ttu-id="ef67e-1226">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1226">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-1227">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-1227">IoT</span></span>

* <span data-ttu-id="ef67e-1228">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1228">Added support for device provisioning service</span></span>
* <span data-ttu-id="ef67e-1229">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1229">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="ef67e-1230">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-1230">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1231">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1231">Monitor</span></span>

* <span data-ttu-id="ef67e-1232">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1232">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="ef67e-1233">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1233">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="ef67e-1234">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1234">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1235">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1235">Network</span></span>

* <span data-ttu-id="ef67e-1236">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1236">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="ef67e-1237">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1237">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-1238">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1238">Profile</span></span>

* <span data-ttu-id="ef67e-1239">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="ef67e-1239">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-1240">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-1240">Role</span></span>

* <span data-ttu-id="ef67e-1241">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="ef67e-1241">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ef67e-1242">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ef67e-1242">Service Fabric</span></span>

* <span data-ttu-id="ef67e-1243">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="ef67e-1243">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="ef67e-1244">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1244">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1245">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1245">VM</span></span>

* <span data-ttu-id="ef67e-1246">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1246">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="ef67e-1247">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1247">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="ef67e-1248">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="ef67e-1248">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="ef67e-1249">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1249">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="ef67e-1250">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="ef67e-1250">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="ef67e-1251">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1251">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef67e-1252">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1252">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef67e-1253">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1253">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="ef67e-1254">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1254">December 19, 2017</span></span>

<span data-ttu-id="ef67e-1255">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="ef67e-1255">Version 2.0.23</span></span>

* <span data-ttu-id="ef67e-1256">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="ef67e-1256">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-1257">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1257">Container</span></span>

* <span data-ttu-id="ef67e-1258">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1258">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1259">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1259">Network</span></span>

* <span data-ttu-id="ef67e-1260">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1260">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="ef67e-1261">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1261">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1262">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1262">Storage</span></span>

* <span data-ttu-id="ef67e-1263">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="ef67e-1263">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1264">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1264">VM</span></span>

* <span data-ttu-id="ef67e-1265">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="ef67e-1265">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="ef67e-1266">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1266">December 5, 2017</span></span>

<span data-ttu-id="ef67e-1267">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="ef67e-1267">Version 2.0.22</span></span>

* <span data-ttu-id="ef67e-1268">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1268">Removed `az component` commands.</span></span> <span data-ttu-id="ef67e-1269">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1269">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-1270">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1270">Core</span></span>
* <span data-ttu-id="ef67e-1271">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="ef67e-1271">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="ef67e-1272">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="ef67e-1272">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1273">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1273">ACS</span></span>

* <span data-ttu-id="ef67e-1274">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1274">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="ef67e-1275">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1275">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="ef67e-1276">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="ef67e-1276">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="ef67e-1277">Advisor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1277">Advisor</span></span>

* <span data-ttu-id="ef67e-1278">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1278">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1279">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1279">Appservice</span></span>

* <span data-ttu-id="ef67e-1280">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1280">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="ef67e-1281">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1281">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="ef67e-1282">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1282">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="ef67e-1283">Consumo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1283">Consumption</span></span>

* <span data-ttu-id="ef67e-1284">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="ef67e-1284">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-1285">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1285">Container</span></span>

* <span data-ttu-id="ef67e-1286">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="ef67e-1286">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1287">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1287">Monitor</span></span>

* <span data-ttu-id="ef67e-1288">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="ef67e-1288">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1289">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1289">Resource</span></span>

* <span data-ttu-id="ef67e-1290">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1290">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-1291">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-1291">Role</span></span>

* <span data-ttu-id="ef67e-1292">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1292">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="ef67e-1293">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="ef67e-1293">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="ef67e-1294">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1294">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1295">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1295">SQL</span></span>

* <span data-ttu-id="ef67e-1296">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1296">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="ef67e-1297">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1297">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1298">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1298">VM</span></span>

* <span data-ttu-id="ef67e-1299">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1299">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="ef67e-1300">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1300">November 14, 2017</span></span>

<span data-ttu-id="ef67e-1301">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="ef67e-1301">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-1302">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-1302">ACR</span></span>

* <span data-ttu-id="ef67e-1303">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="ef67e-1303">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="ef67e-1304">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1304">ACS</span></span>

* <span data-ttu-id="ef67e-1305">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1305">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="ef67e-1306">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1306">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="ef67e-1307">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1307">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="ef67e-1308">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="ef67e-1308">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="ef67e-1309">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="ef67e-1309">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1310">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1310">Appservice</span></span>

* <span data-ttu-id="ef67e-1311">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="ef67e-1311">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="ef67e-1312">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1312">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="ef67e-1313">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1313">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="ef67e-1314">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1314">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="ef67e-1315">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="ef67e-1315">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="ef67e-1316">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="ef67e-1316">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-1317">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-1317">Batch</span></span>

* <span data-ttu-id="ef67e-1318">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1318">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="ef67e-1319">Batchai</span><span class="sxs-lookup"><span data-stu-id="ef67e-1319">Batchai</span></span>

* <span data-ttu-id="ef67e-1320">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1320">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="ef67e-1321">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1321">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="ef67e-1322">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1322">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="ef67e-1323">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1323">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="ef67e-1324">Nube</span><span class="sxs-lookup"><span data-stu-id="ef67e-1324">Cloud</span></span>

* <span data-ttu-id="ef67e-1325">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="ef67e-1325">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-1326">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1326">Container</span></span>

* <span data-ttu-id="ef67e-1327">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1327">Added support to open multiple ports</span></span>
* <span data-ttu-id="ef67e-1328">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="ef67e-1328">Added container group restart policy</span></span>
* <span data-ttu-id="ef67e-1329">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="ef67e-1329">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="ef67e-1330">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="ef67e-1330">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ef67e-1331">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ef67e-1331">Data Lake Analytics</span></span>

* <span data-ttu-id="ef67e-1332">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="ef67e-1332">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ef67e-1333">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef67e-1333">Data Lake Store</span></span>

* <span data-ttu-id="ef67e-1334">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="ef67e-1334">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-1335">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1335">Extension</span></span>

* <span data-ttu-id="ef67e-1336">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="ef67e-1336">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="ef67e-1337">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="ef67e-1337">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-1338">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-1338">IoT</span></span>

* <span data-ttu-id="ef67e-1339">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="ef67e-1339">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1340">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1340">Monitor</span></span>

* <span data-ttu-id="ef67e-1341">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1341">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1342">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1342">Network</span></span>

* <span data-ttu-id="ef67e-1343">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="ef67e-1343">Added support for CAA DNS records</span></span>
* <span data-ttu-id="ef67e-1344">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1344">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="ef67e-1345">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1345">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="ef67e-1346">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1346">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="ef67e-1347">Reservations</span><span class="sxs-lookup"><span data-stu-id="ef67e-1347">Reservations</span></span>

* <span data-ttu-id="ef67e-1348">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="ef67e-1348">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1349">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1349">Resource</span></span>

* <span data-ttu-id="ef67e-1350">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1350">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1351">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1351">SQL</span></span>

* <span data-ttu-id="ef67e-1352">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1352">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1353">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1353">Storage</span></span>

* <span data-ttu-id="ef67e-1354">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="ef67e-1354">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="ef67e-1355">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="ef67e-1355">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="ef67e-1356">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1356">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="ef67e-1357">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1357">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="ef67e-1358">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1358">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="ef67e-1359">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1359">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="ef67e-1360">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1360">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1361">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1361">VM</span></span>

* <span data-ttu-id="ef67e-1362">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1362">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="ef67e-1363">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="ef67e-1363">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="ef67e-1364">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="ef67e-1364">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="ef67e-1365">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1365">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="ef67e-1366">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1366">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="ef67e-1367">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1367">October 24, 2017</span></span>

<span data-ttu-id="ef67e-1368">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="ef67e-1368">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-1369">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1369">Core</span></span>

* <span data-ttu-id="ef67e-1370">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1370">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-1371">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-1371">ACR</span></span>

* <span data-ttu-id="ef67e-1372">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="ef67e-1372">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="ef67e-1373">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="ef67e-1373">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="ef67e-1374">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="ef67e-1374">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1375">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1375">ACS</span></span>

* <span data-ttu-id="ef67e-1376">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1376">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="ef67e-1377">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="ef67e-1377">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1378">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1378">Appservice</span></span>

* <span data-ttu-id="ef67e-1379">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1379">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="ef67e-1380">Componente</span><span class="sxs-lookup"><span data-stu-id="ef67e-1380">Component</span></span>

* <span data-ttu-id="ef67e-1381">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="ef67e-1381">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1382">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1382">Monitor</span></span>

* <span data-ttu-id="ef67e-1383">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1383">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1384">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1384">Resource</span></span>

* <span data-ttu-id="ef67e-1385">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1385">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="ef67e-1386">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1386">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1387">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1387">VM</span></span>

* <span data-ttu-id="ef67e-1388">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1388">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="ef67e-1389">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1389">October 9, 2017</span></span>

<span data-ttu-id="ef67e-1390">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="ef67e-1390">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-1391">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1391">Core</span></span>

* <span data-ttu-id="ef67e-1392">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="ef67e-1392">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1393">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1393">Appservice</span></span>

* <span data-ttu-id="ef67e-1394">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1394">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-1395">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-1395">Batch</span></span>

* <span data-ttu-id="ef67e-1396">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="ef67e-1396">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="ef67e-1397">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="ef67e-1397">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="ef67e-1398">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-1398">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="ef67e-1399">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="ef67e-1399">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="ef67e-1400">Batchai</span><span class="sxs-lookup"><span data-stu-id="ef67e-1400">Batchai</span></span>

* <span data-ttu-id="ef67e-1401">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-1401">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-1402">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ef67e-1402">Keyvault</span></span>

* <span data-ttu-id="ef67e-1403">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1403">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="ef67e-1404">(#4448)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1404">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="ef67e-1405">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1405">Network</span></span>

* <span data-ttu-id="ef67e-1406">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1406">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="ef67e-1407">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="ef67e-1407">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1408">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1408">Resource</span></span>

* <span data-ttu-id="ef67e-1409">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1409">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="ef67e-1410">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="ef67e-1410">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="ef67e-1411">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1411">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="ef67e-1412">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1412">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1413">Sql</span><span class="sxs-lookup"><span data-stu-id="ef67e-1413">Sql</span></span>

* <span data-ttu-id="ef67e-1414">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="ef67e-1414">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="ef67e-1415">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1415">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="ef67e-1416">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1416">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1417">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1417">Storage</span></span>

* <span data-ttu-id="ef67e-1418">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1418">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1419">Vm</span><span class="sxs-lookup"><span data-stu-id="ef67e-1419">Vm</span></span>

* <span data-ttu-id="ef67e-1420">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="ef67e-1420">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="ef67e-1421">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1421">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="ef67e-1422">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1422">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="ef67e-1423">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1423">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="ef67e-1424">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1424">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="ef67e-1425">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1425">September 22, 2017</span></span>

<span data-ttu-id="ef67e-1426">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="ef67e-1426">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1427">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1427">Resource</span></span>

* <span data-ttu-id="ef67e-1428">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1428">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="ef67e-1429">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="ef67e-1429">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="ef67e-1430">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1430">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="ef67e-1431">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1431">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1432">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1432">Network</span></span>

* <span data-ttu-id="ef67e-1433">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1433">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="ef67e-1434">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1434">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="ef67e-1435">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1435">Added `asg` application security group commands</span></span>
* <span data-ttu-id="ef67e-1436">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1436">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="ef67e-1437">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1437">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ef67e-1438">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1438">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="ef67e-1439">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1439">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1440">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1440">Storage</span></span>

* <span data-ttu-id="ef67e-1441">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="ef67e-1441">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ef67e-1442">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="ef67e-1442">Eventgrid</span></span>

* <span data-ttu-id="ef67e-1443">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1443">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1444">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1444">SQL</span></span>

* <span data-ttu-id="ef67e-1445">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1445">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="ef67e-1446">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="ef67e-1446">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="ef67e-1447">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1447">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-1448">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ef67e-1448">Keyvault</span></span>

* <span data-ttu-id="ef67e-1449">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="ef67e-1449">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1450">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1450">VM</span></span>

* <span data-ttu-id="ef67e-1451">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1451">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="ef67e-1452">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="ef67e-1452">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="ef67e-1453">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1453">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="ef67e-1454">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1454">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="ef67e-1455">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1455">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="ef67e-1456">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1456">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1457">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1457">ACS</span></span>

* <span data-ttu-id="ef67e-1458">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1458">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1459">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1459">Appservice</span></span>

* <span data-ttu-id="ef67e-1460">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1460">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ef67e-1461">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="ef67e-1461">Backup</span></span>

* <span data-ttu-id="ef67e-1462">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1462">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="ef67e-1463">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1463">September 11, 2017</span></span>

<span data-ttu-id="ef67e-1464">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="ef67e-1464">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="ef67e-1465">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1465">Core</span></span>

* <span data-ttu-id="ef67e-1466">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1466">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="ef67e-1467">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1467">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1468">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1468">Acs</span></span>

* <span data-ttu-id="ef67e-1469">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1469">Added `acs list-locations` command</span></span>
* <span data-ttu-id="ef67e-1470">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1470">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1471">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1471">Appservice</span></span>

* <span data-ttu-id="ef67e-1472">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1472">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="ef67e-1473">CDN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1473">CDN</span></span>

* <span data-ttu-id="ef67e-1474">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1474">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="ef67e-1475">Extensión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1475">Extension</span></span>

* <span data-ttu-id="ef67e-1476">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="ef67e-1476">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-1477">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ef67e-1477">Keyvault</span></span>

* <span data-ttu-id="ef67e-1478">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1478">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1479">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1479">Network</span></span>

* <span data-ttu-id="ef67e-1480">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1480">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ef67e-1481">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1481">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="ef67e-1482">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1482">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="ef67e-1483">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1483">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ef67e-1484">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1484">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1485">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1485">Resource</span></span>

* <span data-ttu-id="ef67e-1486">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1486">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="ef67e-1487">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1487">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="ef67e-1488">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1488">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="ef67e-1489">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="ef67e-1489">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1490">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1490">SQL</span></span>

* <span data-ttu-id="ef67e-1491">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1491">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1492">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1492">VM</span></span>

* <span data-ttu-id="ef67e-1493">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1493">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="ef67e-1494">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1494">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="ef67e-1495">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1495">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="ef67e-1496">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1496">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="ef67e-1497">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1497">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="ef67e-1498">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1498">August 31, 2017</span></span>

<span data-ttu-id="ef67e-1499">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="ef67e-1499">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-1500">Keyvault</span><span class="sxs-lookup"><span data-stu-id="ef67e-1500">Keyvault</span></span>

* <span data-ttu-id="ef67e-1501">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1501">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="ef67e-1502">Sf</span><span class="sxs-lookup"><span data-stu-id="ef67e-1502">Sf</span></span>

* <span data-ttu-id="ef67e-1503">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1503">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1504">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1504">Storage</span></span>

* <span data-ttu-id="ef67e-1505">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1505">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="ef67e-1506">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1506">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="ef67e-1507">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1507">August 28, 2017</span></span>

<span data-ttu-id="ef67e-1508">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="ef67e-1508">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="ef67e-1509">CLI</span><span class="sxs-lookup"><span data-stu-id="ef67e-1509">CLI</span></span>

* <span data-ttu-id="ef67e-1510">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1510">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1511">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1511">ACS</span></span>

* <span data-ttu-id="ef67e-1512">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1512">Corrected preview regions</span></span>
* <span data-ttu-id="ef67e-1513">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1513">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="ef67e-1514">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="ef67e-1514">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1515">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1515">Appservice</span></span>

* <span data-ttu-id="ef67e-1516">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1516">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="ef67e-1517">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1517">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="ef67e-1518">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1518">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="ef67e-1519">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1519">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="ef67e-1520">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1520">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-1521">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-1521">IoT</span></span>

* <span data-ttu-id="ef67e-1522">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1522">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1523">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1523">Network</span></span>

* <span data-ttu-id="ef67e-1524">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1524">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ef67e-1525">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1525">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="ef67e-1526">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1526">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ef67e-1527">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1527">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ef67e-1528">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1528">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-1529">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1529">Profile</span></span>

* <span data-ttu-id="ef67e-1530">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1530">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ef67e-1531">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ef67e-1531">Service Fabric</span></span>

* <span data-ttu-id="ef67e-1532">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1532">Preview release</span></span>
* <span data-ttu-id="ef67e-1533">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1533">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="ef67e-1534">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1534">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="ef67e-1535">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1535">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1536">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1536">Storage</span></span>

* <span data-ttu-id="ef67e-1537">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1537">Enabled setting blob tier</span></span>
* <span data-ttu-id="ef67e-1538">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1538">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="ef67e-1539">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1539">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="ef67e-1540">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1540">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="ef67e-1541">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1541">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="ef67e-1542">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="ef67e-1542">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1543">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1543">VM</span></span>

* <span data-ttu-id="ef67e-1544">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1544">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="ef67e-1545">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1545">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="ef67e-1546">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1546">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="ef67e-1547">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1547">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="ef67e-1548">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1548">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="ef67e-1549">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1549">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="ef67e-1550">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1550">August 15, 2017</span></span>

<span data-ttu-id="ef67e-1551">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ef67e-1551">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1552">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1552">ACS</span></span>

* <span data-ttu-id="ef67e-1553">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="ef67e-1553">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1554">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1554">Appservice</span></span>

* <span data-ttu-id="ef67e-1555">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1555">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ef67e-1556">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ef67e-1556">Event Grid</span></span>

* <span data-ttu-id="ef67e-1557">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1557">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ef67e-1558">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1558">August 11, 2017</span></span>

<span data-ttu-id="ef67e-1559">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ef67e-1559">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1560">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1560">ACS</span></span>

* <span data-ttu-id="ef67e-1561">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1561">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-1562">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-1562">Batch</span></span>

* <span data-ttu-id="ef67e-1563">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1563">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ef67e-1564">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1564">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ef67e-1565">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1565">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ef67e-1566">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1566">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ef67e-1567">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1567">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ef67e-1568">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1568">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ef67e-1569">Componente</span><span class="sxs-lookup"><span data-stu-id="ef67e-1569">Component</span></span>

* <span data-ttu-id="ef67e-1570">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1570">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ef67e-1571">Contenedor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1571">Container</span></span>

* <span data-ttu-id="ef67e-1572">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1572">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ef67e-1573">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef67e-1573">Data Lake Store</span></span>

* <span data-ttu-id="ef67e-1574">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1574">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ef67e-1575">Event Grid</span><span class="sxs-lookup"><span data-stu-id="ef67e-1575">Event Grid</span></span>

* <span data-ttu-id="ef67e-1576">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1576">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1577">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1577">Network</span></span>

* <span data-ttu-id="ef67e-1578">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1578">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ef67e-1579">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1579">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ef67e-1580">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1580">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ef67e-1581">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1581">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-1582">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1582">Profile</span></span>

* <span data-ttu-id="ef67e-1583">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1583">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1584">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1584">Storage</span></span>

* <span data-ttu-id="ef67e-1585">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1585">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1586">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1586">VM</span></span>

* <span data-ttu-id="ef67e-1587">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1587">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ef67e-1588">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1588">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ef67e-1589">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1589">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ef67e-1590">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1590">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ef67e-1591">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1591">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ef67e-1592">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1592">July 28, 2017</span></span>

<span data-ttu-id="ef67e-1593">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ef67e-1593">Version 2.0.12</span></span>

* <span data-ttu-id="ef67e-1594">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1594">Added container commands</span></span>
* <span data-ttu-id="ef67e-1595">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1595">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ef67e-1596">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1596">Core</span></span>

* <span data-ttu-id="ef67e-1597">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1597">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ef67e-1598">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1598">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ef67e-1599">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1599">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ef67e-1600">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1600">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ef67e-1601">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1601">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ef67e-1602">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1602">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ef67e-1603">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1603">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ef67e-1604">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1604">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ef67e-1605">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1605">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ef67e-1606">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1606">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ef67e-1607">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1607">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ef67e-1608">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1608">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ef67e-1609">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1609">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ef67e-1610">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1610">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ef67e-1611">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1611">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ef67e-1612">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1612">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ef67e-1613">ACR</span><span class="sxs-lookup"><span data-stu-id="ef67e-1613">ACR</span></span>

* <span data-ttu-id="ef67e-1614">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1614">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ef67e-1615">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1615">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ef67e-1616">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1616">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ef67e-1617">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1617">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ef67e-1618">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1618">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ef67e-1619">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1619">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1620">ACS</span></span>

* <span data-ttu-id="ef67e-1621">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1621">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1622">Appservice</span><span class="sxs-lookup"><span data-stu-id="ef67e-1622">Appservice</span></span>

* <span data-ttu-id="ef67e-1623">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1623">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ef67e-1624">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1624">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ef67e-1625">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1625">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ef67e-1626">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1626">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ef67e-1627">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1627">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ef67e-1628">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1628">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ef67e-1629">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1629">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ef67e-1630">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1630">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ef67e-1631">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1631">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ef67e-1632">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1632">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ef67e-1633">Batch</span><span class="sxs-lookup"><span data-stu-id="ef67e-1633">Batch</span></span>

* <span data-ttu-id="ef67e-1634">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1634">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ef67e-1635">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1635">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ef67e-1636">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1636">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ef67e-1637">CDN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1637">CDN</span></span>

* <span data-ttu-id="ef67e-1638">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="ef67e-1638">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="ef67e-1639">Nube</span><span class="sxs-lookup"><span data-stu-id="ef67e-1639">Cloud</span></span>

* <span data-ttu-id="ef67e-1640">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1640">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ef67e-1641">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1641">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ef67e-1642">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1642">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ef67e-1643">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1643">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ef67e-1644">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1644">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef67e-1645">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-1645">CosmosDB</span></span>

* <span data-ttu-id="ef67e-1646">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1646">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ef67e-1647">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="ef67e-1647">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ef67e-1648">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ef67e-1648">Data Lake Analytics</span></span>

* <span data-ttu-id="ef67e-1649">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1649">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ef67e-1650">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1650">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ef67e-1651">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1651">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ef67e-1652">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef67e-1652">Data Lake Store</span></span>

* <span data-ttu-id="ef67e-1653">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1653">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ef67e-1654">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1654">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ef67e-1655">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1655">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ef67e-1656">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1656">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ef67e-1657">Interactive</span><span class="sxs-lookup"><span data-stu-id="ef67e-1657">Interactive</span></span>

* <span data-ttu-id="ef67e-1658">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1658">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ef67e-1659">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1659">Increased test coverage</span></span>
* <span data-ttu-id="ef67e-1660">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1660">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ef67e-1661">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1661">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ef67e-1662">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1662">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ef67e-1663">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1663">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ef67e-1664">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1664">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ef67e-1665">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1665">Added `--progress` flag</span></span>
* <span data-ttu-id="ef67e-1666">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1666">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ef67e-1667">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1667">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ef67e-1668">IoT</span><span class="sxs-lookup"><span data-stu-id="ef67e-1668">IoT</span></span>

* <span data-ttu-id="ef67e-1669">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1669">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ef67e-1670">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1670">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ef67e-1671">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="ef67e-1671">Key vault</span></span>

* <span data-ttu-id="ef67e-1672">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1672">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ef67e-1673">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1673">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ef67e-1674">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1674">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ef67e-1675">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1675">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ef67e-1676">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1676">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ef67e-1677">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1677">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ef67e-1678">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="ef67e-1678">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ef67e-1679">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1679">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ef67e-1680">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1680">Lab</span></span>

* <span data-ttu-id="ef67e-1681">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1681">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ef67e-1682">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1682">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1683">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1683">Monitor</span></span>

* <span data-ttu-id="ef67e-1684">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1684">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ef67e-1685">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1685">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ef67e-1686">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1686">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ef67e-1687">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1687">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ef67e-1688">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1688">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ef67e-1689">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1689">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ef67e-1690">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1690">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ef67e-1691">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1691">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ef67e-1692">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1692">`location` no longer required</span></span>
  * <span data-ttu-id="ef67e-1693">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1693">Add name and ID support for target</span></span>
  * <span data-ttu-id="ef67e-1694">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1694">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ef67e-1695">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1695">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ef67e-1696">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1696">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ef67e-1697">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1697">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ef67e-1698">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1698">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ef67e-1699">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1699">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1700">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1700">Network</span></span>

* <span data-ttu-id="ef67e-1701">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1701">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ef67e-1702">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1702">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ef67e-1703">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1703">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ef67e-1704">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1704">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ef67e-1705">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1705">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ef67e-1706">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1706">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ef67e-1707">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1707">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ef67e-1708">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1708">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ef67e-1709">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1709">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ef67e-1710">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1710">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ef67e-1711">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1711">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ef67e-1712">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1712">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ef67e-1713">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1713">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ef67e-1714">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1714">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ef67e-1715">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1715">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ef67e-1716">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1716">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ef67e-1717">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1717">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ef67e-1718">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1718">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ef67e-1719">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1719">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ef67e-1720">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1720">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ef67e-1721">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1721">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ef67e-1722">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1722">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ef67e-1723">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1723">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ef67e-1724">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1724">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ef67e-1725">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1725">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ef67e-1726">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1726">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ef67e-1727">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1727">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-1728">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1728">Profile</span></span>

* <span data-ttu-id="ef67e-1729">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1729">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ef67e-1730">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1730">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ef67e-1731">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="ef67e-1731">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ef67e-1732">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1732">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ef67e-1733">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1733">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ef67e-1734">RDBMS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1734">RDBMS</span></span>

* <span data-ttu-id="ef67e-1735">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1735">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ef67e-1736">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1736">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ef67e-1737">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1737">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ef67e-1738">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1738">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1739">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1739">Resource</span></span>

* <span data-ttu-id="ef67e-1740">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1740">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ef67e-1741">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1741">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ef67e-1742">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1742">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ef67e-1743">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1743">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ef67e-1744">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1744">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ef67e-1745">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1745">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ef67e-1746">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1746">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ef67e-1747">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1747">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-1748">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-1748">Role</span></span>

* <span data-ttu-id="ef67e-1749">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1749">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ef67e-1750">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1750">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ef67e-1751">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1751">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ef67e-1752">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1752">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ef67e-1753">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1753">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ef67e-1754">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ef67e-1754">Service Fabric</span></span>
* <span data-ttu-id="ef67e-1755">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1755">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ef67e-1756">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1756">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ef67e-1757">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1757">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1758">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1758">SQL</span></span>

* <span data-ttu-id="ef67e-1759">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1759">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ef67e-1760">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1760">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ef67e-1761">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1761">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1762">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1762">Storage</span></span>

* <span data-ttu-id="ef67e-1763">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1763">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ef67e-1764">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1764">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ef67e-1765">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1765">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ef67e-1766">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1766">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="ef67e-1767">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1767">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="ef67e-1768">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1768">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1769">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1769">VM</span></span>

* <span data-ttu-id="ef67e-1770">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="ef67e-1770">Support configuring nsg</span></span>
* <span data-ttu-id="ef67e-1771">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1771">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ef67e-1772">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1772">Support managed service identities</span></span>
* <span data-ttu-id="ef67e-1773">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1773">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="ef67e-1774">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="ef67e-1774">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ef67e-1775">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1775">May 10, 2017</span></span>

<span data-ttu-id="ef67e-1776">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ef67e-1776">Version 2.0.6</span></span>

* <span data-ttu-id="ef67e-1777">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1777">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ef67e-1778">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1778">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ef67e-1779">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef67e-1779">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="ef67e-1780">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ef67e-1780">Include Cognitive Services module</span></span>
* <span data-ttu-id="ef67e-1781">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ef67e-1781">Include Service Fabric module</span></span>
* <span data-ttu-id="ef67e-1782">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1782">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="ef67e-1783">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1783">Add support for CDN commands</span></span>
* <span data-ttu-id="ef67e-1784">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="ef67e-1784">Remove Container module</span></span>
* <span data-ttu-id="ef67e-1785">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1785">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ef67e-1786">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1786">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ef67e-1787">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1787">Core</span></span>

* <span data-ttu-id="ef67e-1788">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="ef67e-1788">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="ef67e-1789">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1789">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ef67e-1790">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1790">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ef67e-1791">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1791">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ef67e-1792">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1792">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ef67e-1793">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1793">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ef67e-1794">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1794">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ef67e-1795">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1795">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ef67e-1796">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1796">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ef67e-1797">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="ef67e-1797">core: Improved performance</span></span>
* <span data-ttu-id="ef67e-1798">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="ef67e-1798">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ef67e-1799">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="ef67e-1799">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1800">ACS</span></span>

* <span data-ttu-id="ef67e-1801">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="ef67e-1801">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ef67e-1802">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="ef67e-1802">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ef67e-1803">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="ef67e-1803">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ef67e-1804">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1804">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1805">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-1805">AppService</span></span>

* <span data-ttu-id="ef67e-1806">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1806">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ef67e-1807">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1807">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ef67e-1808">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1808">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ef67e-1809">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="ef67e-1809">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ef67e-1810">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1810">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ef67e-1811">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1811">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ef67e-1812">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1812">support slot swap with preview</span></span>
* <span data-ttu-id="ef67e-1813">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1813">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ef67e-1814">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1814">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ef67e-1815">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-1815">CosmosDB</span></span>

* <span data-ttu-id="ef67e-1816">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-1816">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="ef67e-1817">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1817">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ef67e-1818">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="ef67e-1818">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ef67e-1819">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="ef67e-1819">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ef67e-1820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ef67e-1820">Data Lake Analytics</span></span>

* <span data-ttu-id="ef67e-1821">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="ef67e-1821">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="ef67e-1822">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="ef67e-1822">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ef67e-1823">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1823">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ef67e-1824">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="ef67e-1824">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ef67e-1825">Tabla</span><span class="sxs-lookup"><span data-stu-id="ef67e-1825">Table</span></span>
  * <span data-ttu-id="ef67e-1826">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="ef67e-1826">Table valued function</span></span>
  * <span data-ttu-id="ef67e-1827">Ver</span><span class="sxs-lookup"><span data-stu-id="ef67e-1827">View</span></span>
  * <span data-ttu-id="ef67e-1828">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1828">Table Statistics.</span></span> <span data-ttu-id="ef67e-1829">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="ef67e-1829">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ef67e-1830">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef67e-1830">Data Lake Store</span></span>

* <span data-ttu-id="ef67e-1831">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="ef67e-1831">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="ef67e-1832">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1832">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ef67e-1833">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1833">missed help for access show.</span></span> <span data-ttu-id="ef67e-1834">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1834">adding it.</span></span> <span data-ttu-id="ef67e-1835">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1835">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ef67e-1836">Buscar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1836">Find</span></span>

* <span data-ttu-id="ef67e-1837">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="ef67e-1837">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ef67e-1838">KeyVault</span><span class="sxs-lookup"><span data-stu-id="ef67e-1838">KeyVault</span></span>

* <span data-ttu-id="ef67e-1839">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="ef67e-1839">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ef67e-1840">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="ef67e-1840">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="ef67e-1841">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="ef67e-1841">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ef67e-1842">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1842">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="ef67e-1843">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1843">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ef67e-1844">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1844">Lab</span></span>

* <span data-ttu-id="ef67e-1845">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1845">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="ef67e-1846">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1846">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="ef67e-1847">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1847">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="ef67e-1848">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1848">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="ef67e-1849">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="ef67e-1849">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="ef67e-1850">Supervisión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1850">Monitor</span></span>

* <span data-ttu-id="ef67e-1851">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1851">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ef67e-1852">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1852">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ef67e-1853">Red</span><span class="sxs-lookup"><span data-stu-id="ef67e-1853">Network</span></span>

* <span data-ttu-id="ef67e-1854">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1854">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="ef67e-1855">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1855">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="ef67e-1856">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="ef67e-1856">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="ef67e-1857">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="ef67e-1857">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="ef67e-1858">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="ef67e-1858">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="ef67e-1859">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ef67e-1859">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="ef67e-1860">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1860">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="ef67e-1861">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="ef67e-1861">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="ef67e-1862">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1862">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="ef67e-1863">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="ef67e-1863">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ef67e-1864">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1864">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="ef67e-1865">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1865">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="ef67e-1866">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="ef67e-1866">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="ef67e-1867">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="ef67e-1867">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="ef67e-1868">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="ef67e-1868">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="ef67e-1869">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1869">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="ef67e-1870">Perfil</span><span class="sxs-lookup"><span data-stu-id="ef67e-1870">Profile</span></span>

* <span data-ttu-id="ef67e-1871">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1871">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ef67e-1872">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1872">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ef67e-1873">Redis</span><span class="sxs-lookup"><span data-stu-id="ef67e-1873">Redis</span></span>

* <span data-ttu-id="ef67e-1874">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="ef67e-1874">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ef67e-1875">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="ef67e-1875">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="ef67e-1876">Recurso</span><span class="sxs-lookup"><span data-stu-id="ef67e-1876">Resource</span></span>

* <span data-ttu-id="ef67e-1877">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1877">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ef67e-1878">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1878">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ef67e-1879">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1879">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ef67e-1880">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="ef67e-1880">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ef67e-1881">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1881">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ef67e-1882">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="ef67e-1882">Add docs for az lock update.</span></span> <span data-ttu-id="ef67e-1883">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1883">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ef67e-1884">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="ef67e-1884">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ef67e-1885">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1885">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ef67e-1886">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="ef67e-1886">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ef67e-1887">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1887">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ef67e-1888">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1888">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ef67e-1889">Rol</span><span class="sxs-lookup"><span data-stu-id="ef67e-1889">Role</span></span>

* <span data-ttu-id="ef67e-1890">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1890">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ef67e-1891">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1891">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ef67e-1892">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1892">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ef67e-1893">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="ef67e-1893">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ef67e-1894">SQL</span><span class="sxs-lookup"><span data-stu-id="ef67e-1894">SQL</span></span>

* <span data-ttu-id="ef67e-1895">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="ef67e-1895">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="ef67e-1896">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1896">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ef67e-1897">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1897">Storage</span></span>

* <span data-ttu-id="ef67e-1898">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1898">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="ef67e-1899">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="ef67e-1899">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ef67e-1900">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="ef67e-1900">Add support for large block blob upload</span></span>
* <span data-ttu-id="ef67e-1901">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="ef67e-1901">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1902">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1902">VM</span></span>

* <span data-ttu-id="ef67e-1903">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="ef67e-1903">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ef67e-1904">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1904">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ef67e-1905">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ef67e-1905">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ef67e-1906">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ef67e-1906">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ef67e-1907">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="ef67e-1907">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ef67e-1908">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="ef67e-1908">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ef67e-1909">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1909">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ef67e-1910">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1910">April 3, 2017</span></span>

<span data-ttu-id="ef67e-1911">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ef67e-1911">Version 2.0.2</span></span>

<span data-ttu-id="ef67e-1912">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="ef67e-1912">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="ef67e-1913">Núcleo</span><span class="sxs-lookup"><span data-stu-id="ef67e-1913">Core</span></span>

* <span data-ttu-id="ef67e-1914">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="ef67e-1914">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="ef67e-1915">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1915">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ef67e-1916">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1916">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ef67e-1917">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1917">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ef67e-1918">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1918">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ef67e-1919">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1919">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ef67e-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1920">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ef67e-1921">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="ef67e-1921">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ef67e-1922">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="ef67e-1922">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="ef67e-1923">ACS</span><span class="sxs-lookup"><span data-stu-id="ef67e-1923">ACS</span></span>

* <span data-ttu-id="ef67e-1924">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1924">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ef67e-1925">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1925">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ef67e-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1926">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ef67e-1927">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1927">Add support for windows clusters.</span></span> <span data-ttu-id="ef67e-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1928">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ef67e-1929">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="ef67e-1929">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ef67e-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1930">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="ef67e-1931">AppService</span><span class="sxs-lookup"><span data-stu-id="ef67e-1931">AppService</span></span>

* <span data-ttu-id="ef67e-1932">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1932">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ef67e-1933">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1933">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ef67e-1934">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1934">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ef67e-1935">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1935">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="ef67e-1936">DataLake</span><span class="sxs-lookup"><span data-stu-id="ef67e-1936">DataLake</span></span>

* <span data-ttu-id="ef67e-1937">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ef67e-1937">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="ef67e-1938">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ef67e-1938">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="ef67e-1939">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ef67e-1939">DocuemntDB</span></span>

* <span data-ttu-id="ef67e-1940">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1940">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ef67e-1941">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="ef67e-1941">VM</span></span>

* <span data-ttu-id="ef67e-1942">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1942">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ef67e-1943">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1943">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ef67e-1944">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1944">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ef67e-1945">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1945">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ef67e-1946">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1946">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ef67e-1947">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1947">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="ef67e-1948">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="ef67e-1948">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ef67e-1949">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="ef67e-1949">February 27, 2017</span></span>

<span data-ttu-id="ef67e-1950">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ef67e-1950">Version 2.0.0</span></span>

<span data-ttu-id="ef67e-1951">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1951">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="ef67e-1952">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1952">Container Service (acs)</span></span>
- <span data-ttu-id="ef67e-1953">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1953">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ef67e-1954">Redes</span><span class="sxs-lookup"><span data-stu-id="ef67e-1954">Networking</span></span>
- <span data-ttu-id="ef67e-1955">Storage</span><span class="sxs-lookup"><span data-stu-id="ef67e-1955">Storage</span></span>

<span data-ttu-id="ef67e-1956">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1956">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="ef67e-1957">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="ef67e-1957">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="ef67e-1958">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="ef67e-1958">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="ef67e-1959">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="ef67e-1959">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="ef67e-1960">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ef67e-1960">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="ef67e-1961">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="ef67e-1961">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ef67e-1962">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1962">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ef67e-1963">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="ef67e-1963">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="ef67e-1964">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="ef67e-1964">Provide feedback from the command line with the `az feedback` command</span></span>

