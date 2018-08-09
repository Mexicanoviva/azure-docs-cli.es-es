---
title: Notas de la versión de la CLI de Azure 2.0
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/03/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 549317fb3ffffbe5f392e7a2bbc5cb4ed10b7e89
ms.sourcegitcommit: 772aad0d9696156d6e87fa00e255dfd0b6394d23
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/08/2018
ms.locfileid: "39718021"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="00cb7-103">Notas de la versión de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="00cb7-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="00cb7-104">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-104">July 31, 2018</span></span>

<span data-ttu-id="00cb7-105">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="00cb7-105">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-106">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-106">ACR</span></span>

* <span data-ttu-id="00cb7-107">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-107">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="00cb7-108">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-108">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-109">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-109">ACS</span></span>

* <span data-ttu-id="00cb7-110">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="00cb7-110">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-111">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-111">Batch</span></span>

* <span data-ttu-id="00cb7-112">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="00cb7-112">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-113">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-113">Container</span></span>

* <span data-ttu-id="00cb7-114">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="00cb7-114">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-115">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-115">Network</span></span>

* <span data-ttu-id="00cb7-116">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="00cb7-116">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="00cb7-117">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-117">Resource</span></span>

* <span data-ttu-id="00cb7-118">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="00cb7-118">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="00cb7-119">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="00cb7-119">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-120">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-120">Role</span></span>

* <span data-ttu-id="00cb7-121">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="00cb7-121">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="00cb7-122">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="00cb7-122">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="00cb7-123">Search</span><span class="sxs-lookup"><span data-stu-id="00cb7-123">Search</span></span>

* <span data-ttu-id="00cb7-124">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="00cb7-124">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="00cb7-125">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="00cb7-125">Service Bus</span></span>

* <span data-ttu-id="00cb7-126">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="00cb7-126">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="00cb7-127">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="00cb7-127">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="00cb7-128">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="00cb7-128">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="00cb7-129">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="00cb7-129">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-130">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-130">Storage</span></span>

* <span data-ttu-id="00cb7-131">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="00cb7-131">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="00cb7-132">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-132">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-133">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-133">VM</span></span>

* <span data-ttu-id="00cb7-134">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="00cb7-134">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="00cb7-135">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="00cb7-135">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="00cb7-136">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="00cb7-136">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="00cb7-137">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="00cb7-137">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="00cb7-138">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-138">July 18, 2018</span></span>

<span data-ttu-id="00cb7-139">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="00cb7-139">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-140">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-140">Core</span></span>

* <span data-ttu-id="00cb7-141">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="00cb7-141">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="00cb7-142">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="00cb7-142">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="00cb7-143">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-143">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-144">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-144">ACR</span></span>

* <span data-ttu-id="00cb7-145">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="00cb7-145">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="00cb7-146">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="00cb7-146">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="00cb7-147">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="00cb7-147">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="00cb7-148">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="00cb7-148">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-149">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-149">ACS</span></span>

* <span data-ttu-id="00cb7-150">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="00cb7-150">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-151">AppService</span><span class="sxs-lookup"><span data-stu-id="00cb7-151">AppService</span></span>

* <span data-ttu-id="00cb7-152">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="00cb7-152">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-153">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-153">Batch</span></span>

* <span data-ttu-id="00cb7-154">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="00cb7-154">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="00cb7-155">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="00cb7-155">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="00cb7-156">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00cb7-156">Batch AI</span></span>

* <span data-ttu-id="00cb7-157">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="00cb7-157">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-158">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-158">Container</span></span>

* <span data-ttu-id="00cb7-159">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="00cb7-159">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="00cb7-160">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="00cb7-160">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-161">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-161">Network</span></span>

* <span data-ttu-id="00cb7-162">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-162">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="00cb7-163">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-163">Added `network nic wait`</span></span>
* <span data-ttu-id="00cb7-164">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="00cb7-164">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="00cb7-165">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="00cb7-165">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="00cb7-166">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-166">Resource</span></span>

* <span data-ttu-id="00cb7-167">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="00cb7-167">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="00cb7-168">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="00cb7-168">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="00cb7-169">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-169">Added `deployment wait` command</span></span>
* <span data-ttu-id="00cb7-170">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="00cb7-170">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-171">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-171">SQL</span></span>

* <span data-ttu-id="00cb7-172">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-172">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="00cb7-173">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="00cb7-173">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="00cb7-174">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="00cb7-174">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-175">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-175">Storage</span></span>

* <span data-ttu-id="00cb7-176">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="00cb7-176">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-177">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-177">VM</span></span>

* <span data-ttu-id="00cb7-178">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="00cb7-178">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="00cb7-179">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-179">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="00cb7-180">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-180">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="00cb7-181">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-181">July 3, 2018</span></span>

<span data-ttu-id="00cb7-182">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="00cb7-182">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="00cb7-183">AKS</span><span class="sxs-lookup"><span data-stu-id="00cb7-183">AKS</span></span>

* <span data-ttu-id="00cb7-184">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="00cb7-184">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="00cb7-185">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-185">July 3, 2018</span></span>

<span data-ttu-id="00cb7-186">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="00cb7-186">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-187">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-187">Core</span></span>

* <span data-ttu-id="00cb7-188">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="00cb7-188">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-189">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-189">ACR</span></span>

* <span data-ttu-id="00cb7-190">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="00cb7-190">Added polling build status</span></span>
* <span data-ttu-id="00cb7-191">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="00cb7-191">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="00cb7-192">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="00cb7-192">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-193">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-193">ACS</span></span>

* <span data-ttu-id="00cb7-194">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="00cb7-194">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="00cb7-195">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="00cb7-195">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="00cb7-196">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-196">Updated options for `aks browse` command.</span></span> <span data-ttu-id="00cb7-197">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="00cb7-197">Added `--listen-port` support</span></span>
* <span data-ttu-id="00cb7-198">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-198">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="00cb7-199">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="00cb7-199">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="00cb7-200">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="00cb7-200">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-201">AppService</span><span class="sxs-lookup"><span data-stu-id="00cb7-201">AppService</span></span>

* <span data-ttu-id="00cb7-202">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="00cb7-202">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="00cb7-203">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="00cb7-203">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="00cb7-204">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="00cb7-204">Backup</span></span>

* <span data-ttu-id="00cb7-205">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="00cb7-205">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="00cb7-206">BatchAI</span><span class="sxs-lookup"><span data-stu-id="00cb7-206">BatchAI</span></span>

* <span data-ttu-id="00cb7-207">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="00cb7-207">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="00cb7-208">Nube</span><span class="sxs-lookup"><span data-stu-id="00cb7-208">Cloud</span></span>

* <span data-ttu-id="00cb7-209">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="00cb7-209">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-210">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-210">Container</span></span>

* <span data-ttu-id="00cb7-211">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="00cb7-211">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="00cb7-212">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="00cb7-212">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="00cb7-213">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="00cb7-213">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-214">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-214">Extension</span></span>

* <span data-ttu-id="00cb7-215">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="00cb7-215">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-216">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-216">Network</span></span>

* <span data-ttu-id="00cb7-217">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="00cb7-217">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="00cb7-218">Rdbms</span><span class="sxs-lookup"><span data-stu-id="00cb7-218">Rdbms</span></span>

* <span data-ttu-id="00cb7-219">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-219">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-220">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-220">Resource</span></span>

* <span data-ttu-id="00cb7-221">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="00cb7-221">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-222">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-222">VM</span></span>

* <span data-ttu-id="00cb7-223">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="00cb7-223">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="00cb7-224">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-224">June 25, 2018</span></span>

<span data-ttu-id="00cb7-225">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="00cb7-225">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="00cb7-226">CLI</span><span class="sxs-lookup"><span data-stu-id="00cb7-226">CLI</span></span>

* <span data-ttu-id="00cb7-227">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-227">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="00cb7-228">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-228">June 19, 2018</span></span>

<span data-ttu-id="00cb7-229">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="00cb7-229">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-230">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-230">Core</span></span>

* <span data-ttu-id="00cb7-231">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-231">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-232">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-232">ACR</span></span>

* <span data-ttu-id="00cb7-233">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="00cb7-233">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="00cb7-234">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="00cb7-234">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-235">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-235">ACS</span></span>

* <span data-ttu-id="00cb7-236">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-236">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="00cb7-237">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-237">Added `--update` support</span></span>
* <span data-ttu-id="00cb7-238">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="00cb7-238">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="00cb7-239">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="00cb7-239">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="00cb7-240">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="00cb7-240">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="00cb7-241">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="00cb7-241">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="00cb7-242">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="00cb7-242">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="00cb7-243">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="00cb7-243">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-244">AppService</span><span class="sxs-lookup"><span data-stu-id="00cb7-244">AppService</span></span>

* <span data-ttu-id="00cb7-245">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="00cb7-245">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="00cb7-246">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="00cb7-246">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-247">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-247">Batch</span></span>

* <span data-ttu-id="00cb7-248">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="00cb7-248">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="00cb7-249">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00cb7-249">Batch AI</span></span>

* <span data-ttu-id="00cb7-250">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="00cb7-250">Added support for workspaces.</span></span> <span data-ttu-id="00cb7-251">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="00cb7-251">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="00cb7-252">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-252">Added support for experiments.</span></span> <span data-ttu-id="00cb7-253">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="00cb7-253">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="00cb7-254">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="00cb7-254">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="00cb7-255">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-255">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="00cb7-256">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-256">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="00cb7-257">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-257">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="00cb7-258">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="00cb7-258">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="00cb7-259">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-259">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="00cb7-260">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-260">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="00cb7-261">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-261">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="00cb7-262">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-262">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="00cb7-263">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-263">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="00cb7-264">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-264">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="00cb7-265">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="00cb7-265">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="00cb7-266">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-266">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="00cb7-267">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="00cb7-267">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="00cb7-268">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="00cb7-268">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="00cb7-269">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="00cb7-269">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="00cb7-270">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="00cb7-270">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="00cb7-271">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="00cb7-271">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="00cb7-272">Mapas</span><span class="sxs-lookup"><span data-stu-id="00cb7-272">Maps</span></span>

* <span data-ttu-id="00cb7-273">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-273">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-274">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-274">Network</span></span>

* <span data-ttu-id="00cb7-275">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="00cb7-275">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="00cb7-276">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-276">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="00cb7-277">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="00cb7-277">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="00cb7-278">Reservations</span><span class="sxs-lookup"><span data-stu-id="00cb7-278">Reservations</span></span>

* <span data-ttu-id="00cb7-279">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-279">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="00cb7-280">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-280">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="00cb7-281">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-281">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="00cb7-282">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-282">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="00cb7-283">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-283">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="00cb7-284">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-284">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-285">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-285">Role</span></span>

* <span data-ttu-id="00cb7-286">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="00cb7-286">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-287">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-287">SQL</span></span>

* <span data-ttu-id="00cb7-288">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="00cb7-288">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-289">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-289">Storage</span></span>

* <span data-ttu-id="00cb7-290">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="00cb7-290">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-291">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-291">VM</span></span>

* <span data-ttu-id="00cb7-292">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-292">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="00cb7-293">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="00cb7-293">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="00cb7-294">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="00cb7-294">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="00cb7-295">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-295">June 13, 2018</span></span>

<span data-ttu-id="00cb7-296">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="00cb7-296">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-297">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-297">Core</span></span>

* <span data-ttu-id="00cb7-298">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="00cb7-298">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="00cb7-299">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-299">June 13, 2018</span></span>

<span data-ttu-id="00cb7-300">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="00cb7-300">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="00cb7-301">AKS</span><span class="sxs-lookup"><span data-stu-id="00cb7-301">AKS</span></span>

* <span data-ttu-id="00cb7-302">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-302">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="00cb7-303">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="00cb7-303">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="00cb7-304">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-304">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="00cb7-305">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-305">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="00cb7-306">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-306">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-307">AppService</span><span class="sxs-lookup"><span data-stu-id="00cb7-307">AppService</span></span>

* <span data-ttu-id="00cb7-308">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="00cb7-308">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="00cb7-309">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-309">June 5, 2018</span></span>

<span data-ttu-id="00cb7-310">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="00cb7-310">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-311">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-311">Interactive</span></span>

* <span data-ttu-id="00cb7-312">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="00cb7-312">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="00cb7-313">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-313">June 5, 2018</span></span>

<span data-ttu-id="00cb7-314">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="00cb7-314">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-315">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-315">Core</span></span>

* <span data-ttu-id="00cb7-316">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="00cb7-316">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="00cb7-317">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="00cb7-317">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-318">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-318">ACR</span></span>

* <span data-ttu-id="00cb7-319">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="00cb7-319">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="00cb7-320">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-320">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="00cb7-321">AKS</span><span class="sxs-lookup"><span data-stu-id="00cb7-321">AKS</span></span>

* <span data-ttu-id="00cb7-322">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="00cb7-322">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-323">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-323">Batch</span></span>

* <span data-ttu-id="00cb7-324">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="00cb7-324">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="00cb7-325">IoT</span><span class="sxs-lookup"><span data-stu-id="00cb7-325">IOT</span></span>

* <span data-ttu-id="00cb7-326">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="00cb7-326">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-327">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-327">Network</span></span>

* <span data-ttu-id="00cb7-328">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="00cb7-328">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="00cb7-329">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="00cb7-329">Policy Insights</span></span>

* <span data-ttu-id="00cb7-330">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="00cb7-330">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="00cb7-331">ARM</span><span class="sxs-lookup"><span data-stu-id="00cb7-331">ARM</span></span>

* <span data-ttu-id="00cb7-332">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-332">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-333">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-333">SQL</span></span>

* <span data-ttu-id="00cb7-334">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="00cb7-334">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="00cb7-335">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="00cb7-335">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="00cb7-336">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-336">Storage</span></span>

* <span data-ttu-id="00cb7-337">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="00cb7-337">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-338">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-338">VM</span></span>

* <span data-ttu-id="00cb7-339">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="00cb7-339">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="00cb7-340">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-340">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="00cb7-341">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-341">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="00cb7-342">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-342">May 22, 2018</span></span>

<span data-ttu-id="00cb7-343">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="00cb7-343">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-344">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-344">Core</span></span>

* <span data-ttu-id="00cb7-345">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="00cb7-345">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-346">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-346">ACS</span></span>

* <span data-ttu-id="00cb7-347">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="00cb7-347">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="00cb7-348">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="00cb7-348">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-349">AppService</span><span class="sxs-lookup"><span data-stu-id="00cb7-349">AppService</span></span>

* <span data-ttu-id="00cb7-350">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="00cb7-350">Improved generic update commands</span></span>
* <span data-ttu-id="00cb7-351">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="00cb7-351">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-352">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-352">Container</span></span>

* <span data-ttu-id="00cb7-353">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="00cb7-353">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="00cb7-354">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="00cb7-354">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-355">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-355">Extension</span></span>

* <span data-ttu-id="00cb7-356">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="00cb7-356">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-357">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-357">Interactive</span></span>

* <span data-ttu-id="00cb7-358">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="00cb7-358">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="00cb7-359">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="00cb7-359">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="00cb7-360">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00cb7-360">KeyVault</span></span>

* <span data-ttu-id="00cb7-361">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="00cb7-361">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-362">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-362">Network</span></span>

* <span data-ttu-id="00cb7-363">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="00cb7-363">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="00cb7-364">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="00cb7-364">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-365">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-365">SQL</span></span>

* <span data-ttu-id="00cb7-366">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="00cb7-366">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="00cb7-367">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="00cb7-367">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="00cb7-368">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="00cb7-368">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="00cb7-369">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="00cb7-369">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="00cb7-370">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="00cb7-370">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="00cb7-371">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-371">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="00cb7-372">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="00cb7-372">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="00cb7-373">`edition`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-373">`edition`.</span></span> <span data-ttu-id="00cb7-374">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="00cb7-374">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="00cb7-375">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-375">`elasticPoolName`.</span></span> <span data-ttu-id="00cb7-376">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="00cb7-376">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="00cb7-377">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="00cb7-377">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="00cb7-378">`edition`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-378">`edition`.</span></span> <span data-ttu-id="00cb7-379">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="00cb7-379">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="00cb7-380">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-380">`dtu`.</span></span> <span data-ttu-id="00cb7-381">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="00cb7-381">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="00cb7-382">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-382">`databaseDtuMin`.</span></span> <span data-ttu-id="00cb7-383">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="00cb7-383">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="00cb7-384">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-384">`databaseDtuMax`.</span></span> <span data-ttu-id="00cb7-385">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="00cb7-385">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="00cb7-386">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-386">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="00cb7-387">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-387">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-388">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-388">Storage</span></span>

* <span data-ttu-id="00cb7-389">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="00cb7-389">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="00cb7-390">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="00cb7-390">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-391">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-391">VM</span></span>

* <span data-ttu-id="00cb7-392">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-392">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="00cb7-393">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="00cb7-393">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="00cb7-394">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="00cb7-394">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="00cb7-395">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="00cb7-395">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="00cb7-396">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-396">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="00cb7-397">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-397">May 7, 2018</span></span>

<span data-ttu-id="00cb7-398">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="00cb7-398">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-399">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-399">Core</span></span>

* <span data-ttu-id="00cb7-400">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="00cb7-400">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="00cb7-401">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="00cb7-401">Added limited support for positional arguments</span></span>
* <span data-ttu-id="00cb7-402">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-402">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="00cb7-403">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="00cb7-403">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="00cb7-404">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-404">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="00cb7-405">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="00cb7-405">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="00cb7-406">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-406">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="00cb7-407">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="00cb7-407">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="00cb7-408">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-408">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-409">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-409">ACR</span></span>

* <span data-ttu-id="00cb7-410">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="00cb7-410">Added ACR Build commands</span></span>
* <span data-ttu-id="00cb7-411">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="00cb7-411">Improved resource not found error messages</span></span>
* <span data-ttu-id="00cb7-412">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="00cb7-412">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="00cb7-413">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="00cb7-413">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="00cb7-414">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-414">Improved repository commands error messages</span></span>
* <span data-ttu-id="00cb7-415">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="00cb7-415">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-416">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-416">ACS</span></span>

* <span data-ttu-id="00cb7-417">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="00cb7-417">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="00cb7-418">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="00cb7-418">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="00cb7-419">AMS</span><span class="sxs-lookup"><span data-stu-id="00cb7-419">AMS</span></span>

* <span data-ttu-id="00cb7-420">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="00cb7-420">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-421">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-421">Appservice</span></span>

* <span data-ttu-id="00cb7-422">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="00cb7-422">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="00cb7-423">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-423">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="00cb7-424">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="00cb7-424">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="00cb7-425">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="00cb7-425">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="00cb7-426">Batch AI</span><span class="sxs-lookup"><span data-stu-id="00cb7-426">Batch AI</span></span>

* <span data-ttu-id="00cb7-427">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="00cb7-427">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="00cb7-428">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00cb7-428">Cognitive Services</span></span>

* <span data-ttu-id="00cb7-429">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="00cb7-429">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="00cb7-430">Consumo</span><span class="sxs-lookup"><span data-stu-id="00cb7-430">Consumption</span></span>

* <span data-ttu-id="00cb7-431">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="00cb7-431">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-432">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-432">Container</span></span>

* <span data-ttu-id="00cb7-433">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="00cb7-433">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="00cb7-434">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="00cb7-434">Cosmos DB</span></span>

* <span data-ttu-id="00cb7-435">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="00cb7-435">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="00cb7-436">DMS</span><span class="sxs-lookup"><span data-stu-id="00cb7-436">DMS</span></span>

* <span data-ttu-id="00cb7-437">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-437">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-438">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-438">Extension</span></span>

* <span data-ttu-id="00cb7-439">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="00cb7-439">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-440">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-440">Interactive</span></span>

* <span data-ttu-id="00cb7-441">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="00cb7-441">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="00cb7-442">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="00cb7-442">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="00cb7-443">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="00cb7-443">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="00cb7-444">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-444">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="00cb7-445">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-445">Lab</span></span>

* <span data-ttu-id="00cb7-446">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="00cb7-446">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-447">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-447">Network</span></span>

* <span data-ttu-id="00cb7-448">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="00cb7-448">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="00cb7-449">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-449">Profile</span></span>

* <span data-ttu-id="00cb7-450">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-450">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="00cb7-451">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="00cb7-451">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="00cb7-452">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="00cb7-452">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="00cb7-453">Redis</span><span class="sxs-lookup"><span data-stu-id="00cb7-453">Redis</span></span>

* <span data-ttu-id="00cb7-454">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="00cb7-454">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="00cb7-455">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-455">Deprecated `redis list-all`.</span></span> <span data-ttu-id="00cb7-456">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="00cb7-456">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="00cb7-457">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="00cb7-457">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="00cb7-458">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-458">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-459">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-459">Role</span></span>

* <span data-ttu-id="00cb7-460">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="00cb7-460">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-461">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-461">Storage</span></span>

* <span data-ttu-id="00cb7-462">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="00cb7-462">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="00cb7-463">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="00cb7-463">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="00cb7-464">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="00cb7-464">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="00cb7-465">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="00cb7-465">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="00cb7-466">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="00cb7-466">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-467">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-467">VM</span></span>

* <span data-ttu-id="00cb7-468">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="00cb7-468">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="00cb7-469">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="00cb7-469">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="00cb7-470">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="00cb7-470">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="00cb7-471">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="00cb7-471">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="00cb7-472">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="00cb7-472">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="00cb7-473">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="00cb7-473">Added write accelerator support</span></span>
* <span data-ttu-id="00cb7-474">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-474">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="00cb7-475">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="00cb7-475">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="00cb7-476">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="00cb7-476">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="00cb7-477">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-477">April 10, 2018</span></span>

<span data-ttu-id="00cb7-478">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="00cb7-478">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-479">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-479">ACR</span></span>

* <span data-ttu-id="00cb7-480">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="00cb7-480">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-481">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-481">ACS</span></span>

* <span data-ttu-id="00cb7-482">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="00cb7-482">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-483">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-483">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="00cb7-485">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="00cb7-485">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="00cb7-486">BatchAI</span><span class="sxs-lookup"><span data-stu-id="00cb7-486">BatchAI</span></span>

* <span data-ttu-id="00cb7-487">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="00cb7-487">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="00cb7-488">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="00cb7-488">Job level mounting</span></span>
 - <span data-ttu-id="00cb7-489">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="00cb7-489">Environment variables with secret values</span></span>
 - <span data-ttu-id="00cb7-490">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="00cb7-490">Performance counters settings</span></span>
 - <span data-ttu-id="00cb7-491">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="00cb7-491">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="00cb7-492">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="00cb7-492">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="00cb7-493">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="00cb7-493">Usage and limits reporting</span></span>
 - <span data-ttu-id="00cb7-494">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="00cb7-494">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="00cb7-495">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="00cb7-495">Support for custom images</span></span>
 - <span data-ttu-id="00cb7-496">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="00cb7-496">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="00cb7-497">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="00cb7-497">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="00cb7-498">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="00cb7-498">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="00cb7-499">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="00cb7-499">National clouds are supported</span></span>
* <span data-ttu-id="00cb7-500">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="00cb7-500">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="00cb7-501">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="00cb7-501">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="00cb7-502">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="00cb7-502">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="00cb7-503">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="00cb7-503">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="00cb7-504">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="00cb7-504">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="00cb7-505">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="00cb7-505">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="00cb7-506">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-506">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="00cb7-507">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="00cb7-507">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="00cb7-508">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="00cb7-508">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="00cb7-509">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-509">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="00cb7-510">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-510">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="00cb7-511">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="00cb7-511">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="00cb7-512">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-512">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="00cb7-513">Facturación</span><span class="sxs-lookup"><span data-stu-id="00cb7-513">Billing</span></span>

* <span data-ttu-id="00cb7-514">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="00cb7-514">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="00cb7-515">Consumo</span><span class="sxs-lookup"><span data-stu-id="00cb7-515">Consumption</span></span>

* <span data-ttu-id="00cb7-516">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-516">Added `marketplace` commands</span></span>
* <span data-ttu-id="00cb7-517">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="00cb7-517">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="00cb7-518">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="00cb7-518">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="00cb7-519">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="00cb7-519">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="00cb7-520">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="00cb7-520">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="00cb7-521">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="00cb7-521">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-522">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-522">Container</span></span>

* <span data-ttu-id="00cb7-523">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="00cb7-523">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="00cb7-524">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="00cb7-524">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-525">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-525">Extension</span></span>

* <span data-ttu-id="00cb7-526">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="00cb7-526">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-527">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-527">Interactive</span></span>

* <span data-ttu-id="00cb7-528">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="00cb7-528">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="00cb7-529">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-529">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="00cb7-530">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="00cb7-530">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-531">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-531">Network</span></span>

* <span data-ttu-id="00cb7-532">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-532">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="00cb7-533">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-533">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="00cb7-534">4910</span><span class="sxs-lookup"><span data-stu-id="00cb7-534">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="00cb7-535">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="00cb7-535">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="00cb7-536">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="00cb7-536">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="00cb7-537">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-537">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="00cb7-538">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-538">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="00cb7-539">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="00cb7-539">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-540">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-540">Profile</span></span>

* <span data-ttu-id="00cb7-541">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="00cb7-541">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="00cb7-542">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="00cb7-542">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="00cb7-543">RDBMS</span><span class="sxs-lookup"><span data-stu-id="00cb7-543">RDBMS</span></span>

* <span data-ttu-id="00cb7-544">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-544">Added `georestore` command</span></span>
* <span data-ttu-id="00cb7-545">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-545">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-546">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-546">Resource</span></span>

* <span data-ttu-id="00cb7-547">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-547">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="00cb7-548">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-548">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-549">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-549">SQL</span></span>

* <span data-ttu-id="00cb7-550">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="00cb7-550">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-551">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-551">Storage</span></span>

* <span data-ttu-id="00cb7-552">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="00cb7-552">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-553">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-553">VM</span></span>

* <span data-ttu-id="00cb7-554">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-554">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="00cb7-555">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="00cb7-555">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="00cb7-557">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-557">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="00cb7-558">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="00cb7-558">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="00cb7-559">5718</span><span class="sxs-lookup"><span data-stu-id="00cb7-559">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="00cb7-560">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="00cb7-560">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="00cb7-561">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-561">March 27, 2018</span></span>

<span data-ttu-id="00cb7-562">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="00cb7-562">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-563">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-563">Core</span></span>

* <span data-ttu-id="00cb7-564">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="00cb7-564">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-565">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-565">ACS</span></span>

* <span data-ttu-id="00cb7-566">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="00cb7-566">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-567">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-567">Appservice</span></span>

* <span data-ttu-id="00cb7-568">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-568">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="00cb7-569">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-569">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="00cb7-570">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="00cb7-570">Backup</span></span>

* <span data-ttu-id="00cb7-571">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-571">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="00cb7-572">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-572">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="00cb7-573">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="00cb7-573">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="00cb7-574">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="00cb7-574">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-575">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-575">Container</span></span>

* <span data-ttu-id="00cb7-576">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-576">Added `container exec` command.</span></span> <span data-ttu-id="00cb7-577">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="00cb7-577">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="00cb7-578">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="00cb7-578">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-579">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-579">Extension</span></span>

* <span data-ttu-id="00cb7-580">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="00cb7-580">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="00cb7-581">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="00cb7-581">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="00cb7-582">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="00cb7-582">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-583">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-583">Interactive</span></span>

* <span data-ttu-id="00cb7-584">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-584">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="00cb7-585">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="00cb7-585">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="00cb7-586">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-586">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="00cb7-587">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="00cb7-587">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="00cb7-588">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-588">Lab</span></span>

* <span data-ttu-id="00cb7-589">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="00cb7-589">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-590">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-590">Monitor</span></span>

* <span data-ttu-id="00cb7-591">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="00cb7-591">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="00cb7-592">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="00cb7-592">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="00cb7-593">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="00cb7-593">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-594">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-594">Network</span></span>

* <span data-ttu-id="00cb7-595">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="00cb7-595">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-596">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-596">Profile</span></span>

* <span data-ttu-id="00cb7-597">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="00cb7-597">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="00cb7-598">RDBMS</span><span class="sxs-lookup"><span data-stu-id="00cb7-598">RDBMS</span></span>

* <span data-ttu-id="00cb7-599">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="00cb7-599">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-600">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-600">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="00cb7-602">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-602">Role</span></span>

* <span data-ttu-id="00cb7-603">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-603">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="00cb7-604">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="00cb7-604">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="00cb7-605">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-605">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="00cb7-606">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-606">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="00cb7-607">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="00cb7-607">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-608">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-608">Storage</span></span>

* <span data-ttu-id="00cb7-609">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="00cb7-609">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="00cb7-610">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="00cb7-610">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-611">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-611">VM</span></span>

* <span data-ttu-id="00cb7-612">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="00cb7-612">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="00cb7-613">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-613">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="00cb7-614">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="00cb7-614">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="00cb7-615">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="00cb7-615">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="00cb7-616">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-616">March 13, 2018</span></span>

<span data-ttu-id="00cb7-617">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="00cb7-617">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-618">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-618">ACR</span></span>

* <span data-ttu-id="00cb7-619">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-619">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="00cb7-620">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-620">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="00cb7-621">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-621">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-622">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-622">ACS</span></span>

* <span data-ttu-id="00cb7-623">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="00cb7-623">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="00cb7-624">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="00cb7-624">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="00cb7-625">Advisor</span><span class="sxs-lookup"><span data-stu-id="00cb7-625">Advisor</span></span>

* <span data-ttu-id="00cb7-626">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="00cb7-626">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="00cb7-627">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-627">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="00cb7-628">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="00cb7-628">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="00cb7-629">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="00cb7-629">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="00cb7-630">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-630">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-631">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-631">Appservice</span></span>

* <span data-ttu-id="00cb7-632">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-632">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="00cb7-633">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-633">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="00cb7-634">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="00cb7-634">Eventhubs</span></span>

* <span data-ttu-id="00cb7-635">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="00cb7-635">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-636">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-636">Extension</span></span>

* <span data-ttu-id="00cb7-637">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="00cb7-637">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-638">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-638">Interactive</span></span>

* <span data-ttu-id="00cb7-639">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="00cb7-639">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="00cb7-640">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="00cb7-640">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="00cb7-641">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="00cb7-641">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="00cb7-642">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="00cb7-642">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-643">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-643">Monitor</span></span>

* <span data-ttu-id="00cb7-644">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-644">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="00cb7-645">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-645">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="00cb7-646">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-646">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="00cb7-647">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-647">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-648">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-648">Network</span></span>

* <span data-ttu-id="00cb7-649">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-649">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="00cb7-650">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="00cb7-650">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="00cb7-651">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-651">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="00cb7-652">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-652">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-653">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-653">Profile</span></span>

* <span data-ttu-id="00cb7-654">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-654">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="00cb7-655">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-655">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="00cb7-656">RDBMS</span><span class="sxs-lookup"><span data-stu-id="00cb7-656">RDBMS</span></span>

* <span data-ttu-id="00cb7-657">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="00cb7-657">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="00cb7-658">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="00cb7-658">Service Bus</span></span>

* <span data-ttu-id="00cb7-659">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="00cb7-659">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-660">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-660">Storage</span></span>

* <span data-ttu-id="00cb7-661">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="00cb7-661">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="00cb7-662">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="00cb7-662">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-663">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-663">VM</span></span>

* <span data-ttu-id="00cb7-664">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="00cb7-664">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="00cb7-665">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-665">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="00cb7-666">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-666">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="00cb7-667">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="00cb7-667">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="00cb7-668">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-668">February 27, 2018</span></span>

<span data-ttu-id="00cb7-669">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="00cb7-669">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-670">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-670">Core</span></span>

* <span data-ttu-id="00cb7-671">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="00cb7-671">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="00cb7-672">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="00cb7-672">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="00cb7-673">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="00cb7-673">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-674">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-674">ACS</span></span>

* <span data-ttu-id="00cb7-675">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="00cb7-675">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="00cb7-676">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="00cb7-676">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="00cb7-677">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="00cb7-677">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="00cb7-678">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="00cb7-678">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-679">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-679">Appservice</span></span>

* <span data-ttu-id="00cb7-680">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="00cb7-680">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="00cb7-681">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="00cb7-681">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="00cb7-682">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00cb7-682">Cognitive Services</span></span>

* <span data-ttu-id="00cb7-683">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00cb7-683">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="00cb7-684">Consumo</span><span class="sxs-lookup"><span data-stu-id="00cb7-684">Consumption</span></span>

* <span data-ttu-id="00cb7-685">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="00cb7-685">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="00cb7-686">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="00cb7-686">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-687">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-687">Container</span></span>

* <span data-ttu-id="00cb7-688">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="00cb7-688">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-689">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-689">Network</span></span>

* <span data-ttu-id="00cb7-690">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="00cb7-690">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-691">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-691">Resource</span></span>

* <span data-ttu-id="00cb7-692">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="00cb7-692">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-693">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-693">Role</span></span>

* <span data-ttu-id="00cb7-694">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="00cb7-694">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-695">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-695">SQL</span></span>

* <span data-ttu-id="00cb7-696">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="00cb7-696">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-697">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-697">Storage</span></span>

* <span data-ttu-id="00cb7-698">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-698">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-699">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-699">VM</span></span>

* <span data-ttu-id="00cb7-700">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="00cb7-700">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="00cb7-701">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-701">February 13, 2018</span></span>

<span data-ttu-id="00cb7-702">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="00cb7-702">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-703">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-703">Core</span></span>

* <span data-ttu-id="00cb7-704">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="00cb7-704">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-705">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-705">ACS</span></span>

* <span data-ttu-id="00cb7-706">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-706">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="00cb7-707">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-707">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="00cb7-708">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="00cb7-708">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="00cb7-709">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="00cb7-709">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="00cb7-710">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="00cb7-710">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="00cb7-711">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="00cb7-711">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="00cb7-712">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="00cb7-712">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="00cb7-713">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="00cb7-713">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-714">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-714">Appservice</span></span>

* <span data-ttu-id="00cb7-715">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="00cb7-715">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="00cb7-716">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="00cb7-716">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="00cb7-717">CDN</span><span class="sxs-lookup"><span data-stu-id="00cb7-717">CDN</span></span>

* <span data-ttu-id="00cb7-718">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-718">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-719">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-719">Container</span></span>

* <span data-ttu-id="00cb7-720">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="00cb7-720">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="00cb7-721">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="00cb7-721">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00cb7-722">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00cb7-722">CosmosDB</span></span>

* <span data-ttu-id="00cb7-723">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="00cb7-723">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-724">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-724">Extension</span></span>

* <span data-ttu-id="00cb7-725">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-725">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="00cb7-726">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-726">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="00cb7-727">Comentarios</span><span class="sxs-lookup"><span data-stu-id="00cb7-727">Feedback</span></span>

* <span data-ttu-id="00cb7-728">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="00cb7-728">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-729">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-729">Interactive</span></span>

* <span data-ttu-id="00cb7-730">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="00cb7-730">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="00cb7-731">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="00cb7-731">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="00cb7-732">IoT</span><span class="sxs-lookup"><span data-stu-id="00cb7-732">IoT</span></span>

* <span data-ttu-id="00cb7-733">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-733">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="00cb7-734">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-734">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="00cb7-735">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-735">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="00cb7-736">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="00cb7-736">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-737">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-737">Monitor</span></span>

* <span data-ttu-id="00cb7-738">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-738">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-739">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-739">Network</span></span>

* <span data-ttu-id="00cb7-740">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="00cb7-740">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="00cb7-741">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-741">Profile</span></span>

* <span data-ttu-id="00cb7-742">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="00cb7-742">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-743">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-743">Resource</span></span>

* <span data-ttu-id="00cb7-744">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="00cb7-744">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-745">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-745">Role</span></span>

* <span data-ttu-id="00cb7-746">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-746">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-747">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-747">SQL</span></span>

* <span data-ttu-id="00cb7-748">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-748">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="00cb7-749">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-749">Added `sql db rename`</span></span>
* <span data-ttu-id="00cb7-750">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="00cb7-750">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-751">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-751">Storage</span></span>

* <span data-ttu-id="00cb7-752">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="00cb7-752">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-753">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-753">VM</span></span>

* <span data-ttu-id="00cb7-754">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="00cb7-754">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="00cb7-755">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="00cb7-755">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="00cb7-756">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="00cb7-756">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="00cb7-757">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-757">January 31, 2018</span></span>

<span data-ttu-id="00cb7-758">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="00cb7-758">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-759">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-759">Core</span></span>

* <span data-ttu-id="00cb7-760">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="00cb7-760">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="00cb7-761">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="00cb7-761">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="00cb7-762">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="00cb7-762">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="00cb7-763">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="00cb7-763">Use `--verbose` to see</span></span>
* <span data-ttu-id="00cb7-764">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="00cb7-764">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-765">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-765">ACS</span></span>

* <span data-ttu-id="00cb7-766">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="00cb7-766">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="00cb7-767">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="00cb7-767">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-768">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-768">Appservice</span></span>

* <span data-ttu-id="00cb7-769">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="00cb7-769">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="00cb7-770">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="00cb7-770">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="00cb7-771">CDN</span><span class="sxs-lookup"><span data-stu-id="00cb7-771">CDN</span></span>

* <span data-ttu-id="00cb7-772">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-772">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00cb7-773">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00cb7-773">CosmosDB</span></span>

* <span data-ttu-id="00cb7-774">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="00cb7-774">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-775">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-775">Interactive</span></span>

* <span data-ttu-id="00cb7-776">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="00cb7-776">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-777">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-777">Network</span></span>

* <span data-ttu-id="00cb7-778">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-778">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="00cb7-779">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="00cb7-779">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="00cb7-780">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-780">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="00cb7-781">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-781">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="00cb7-782">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="00cb7-782">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="00cb7-783">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="00cb7-783">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="00cb7-784">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="00cb7-784">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="00cb7-785">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="00cb7-785">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="00cb7-786">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="00cb7-786">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="00cb7-787">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="00cb7-787">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-788">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-788">Profile</span></span>

* <span data-ttu-id="00cb7-789">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="00cb7-789">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-790">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-790">Resource</span></span>

* <span data-ttu-id="00cb7-791">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="00cb7-791">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-792">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-792">Storage</span></span>

* <span data-ttu-id="00cb7-793">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="00cb7-793">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="00cb7-794">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="00cb7-794">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="00cb7-795">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="00cb7-795">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="00cb7-796">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-796">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="00cb7-797">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="00cb7-797">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-798">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-798">VM</span></span>

* <span data-ttu-id="00cb7-799">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="00cb7-799">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="00cb7-800">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="00cb7-800">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="00cb7-801">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="00cb7-801">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="00cb7-802">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-802">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="00cb7-803">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="00cb7-803">January 17, 2018</span></span>

<span data-ttu-id="00cb7-804">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="00cb7-804">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-805">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-805">ACR</span></span>

* <span data-ttu-id="00cb7-806">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="00cb7-806">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="00cb7-807">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="00cb7-807">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-808">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-808">ACS</span></span>

* <span data-ttu-id="00cb7-809">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="00cb7-809">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="00cb7-810">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="00cb7-810">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-811">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-811">Appservice</span></span>

* <span data-ttu-id="00cb7-812">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="00cb7-812">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="00cb7-813">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="00cb7-813">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="00cb7-814">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="00cb7-814">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="00cb7-815">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="00cb7-815">Backup</span></span>

* <span data-ttu-id="00cb7-816">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="00cb7-816">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="00cb7-817">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="00cb7-817">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="00cb7-818">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="00cb7-818">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="00cb7-819">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="00cb7-819">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="00cb7-820">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="00cb7-820">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-821">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-821">Batch</span></span>

* <span data-ttu-id="00cb7-822">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="00cb7-822">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="00cb7-823">Nube</span><span class="sxs-lookup"><span data-stu-id="00cb7-823">Cloud</span></span>

* <span data-ttu-id="00cb7-824">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="00cb7-824">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="00cb7-825">Consumo</span><span class="sxs-lookup"><span data-stu-id="00cb7-825">Consumption</span></span>

* <span data-ttu-id="00cb7-826">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="00cb7-826">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="00cb7-827">Event Grid</span><span class="sxs-lookup"><span data-stu-id="00cb7-827">Event Grid</span></span>

* <span data-ttu-id="00cb7-828">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="00cb7-828">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="00cb7-829">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="00cb7-829">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="00cb7-830">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-830">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="00cb7-831">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="00cb7-831">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="00cb7-832">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-832">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="00cb7-833">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-833">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="00cb7-834">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="00cb7-834">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="00cb7-835">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="00cb7-835">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-836">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-836">Interactive</span></span>

* <span data-ttu-id="00cb7-837">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="00cb7-837">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="00cb7-838">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="00cb7-838">Fixed errors on startup</span></span>
* <span data-ttu-id="00cb7-839">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="00cb7-839">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="00cb7-840">IoT</span><span class="sxs-lookup"><span data-stu-id="00cb7-840">IoT</span></span>

* <span data-ttu-id="00cb7-841">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="00cb7-841">Added support for device provisioning service</span></span>
* <span data-ttu-id="00cb7-842">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-842">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="00cb7-843">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="00cb7-843">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-844">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-844">Monitor</span></span>

* <span data-ttu-id="00cb7-845">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-845">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="00cb7-846">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-846">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="00cb7-847">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="00cb7-847">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-848">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-848">Network</span></span>

* <span data-ttu-id="00cb7-849">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-849">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="00cb7-850">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-850">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-851">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-851">Profile</span></span>

* <span data-ttu-id="00cb7-852">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="00cb7-852">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-853">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-853">Role</span></span>

* <span data-ttu-id="00cb7-854">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="00cb7-854">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="00cb7-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00cb7-855">Service Fabric</span></span>

* <span data-ttu-id="00cb7-856">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="00cb7-856">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="00cb7-857">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="00cb7-857">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-858">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-858">VM</span></span>

* <span data-ttu-id="00cb7-859">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="00cb7-859">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="00cb7-860">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="00cb7-860">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="00cb7-861">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="00cb7-861">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="00cb7-862">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="00cb7-862">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="00cb7-863">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="00cb7-863">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="00cb7-864">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-864">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="00cb7-865">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-865">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="00cb7-866">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="00cb7-866">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="00cb7-867">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-867">December 19, 2017</span></span>

<span data-ttu-id="00cb7-868">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="00cb7-868">Version 2.0.23</span></span>

* <span data-ttu-id="00cb7-869">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="00cb7-869">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-870">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-870">Container</span></span>

* <span data-ttu-id="00cb7-871">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-871">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-872">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-872">Network</span></span>

* <span data-ttu-id="00cb7-873">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-873">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="00cb7-874">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-874">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-875">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-875">Storage</span></span>

* <span data-ttu-id="00cb7-876">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="00cb7-876">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-877">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-877">VM</span></span>

* <span data-ttu-id="00cb7-878">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="00cb7-878">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="00cb7-879">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-879">December 5, 2017</span></span>

<span data-ttu-id="00cb7-880">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="00cb7-880">Version 2.0.22</span></span>

* <span data-ttu-id="00cb7-881">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-881">Removed `az component` commands.</span></span> <span data-ttu-id="00cb7-882">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="00cb7-882">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-883">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-883">Core</span></span>
* <span data-ttu-id="00cb7-884">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="00cb7-884">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="00cb7-885">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="00cb7-885">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-886">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-886">ACS</span></span>

* <span data-ttu-id="00cb7-887">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="00cb7-887">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="00cb7-888">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-888">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="00cb7-889">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="00cb7-889">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="00cb7-890">Advisor</span><span class="sxs-lookup"><span data-stu-id="00cb7-890">Advisor</span></span>

* <span data-ttu-id="00cb7-891">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="00cb7-891">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-892">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-892">Appservice</span></span>

* <span data-ttu-id="00cb7-893">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="00cb7-893">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="00cb7-894">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="00cb7-894">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="00cb7-895">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="00cb7-895">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="00cb7-896">Consumo</span><span class="sxs-lookup"><span data-stu-id="00cb7-896">Consumption</span></span>

* <span data-ttu-id="00cb7-897">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="00cb7-897">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-898">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-898">Container</span></span>

* <span data-ttu-id="00cb7-899">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="00cb7-899">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-900">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-900">Monitor</span></span>

* <span data-ttu-id="00cb7-901">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="00cb7-901">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-902">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-902">Resource</span></span>

* <span data-ttu-id="00cb7-903">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="00cb7-903">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-904">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-904">Role</span></span>

* <span data-ttu-id="00cb7-905">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="00cb7-905">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="00cb7-906">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="00cb7-906">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="00cb7-907">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="00cb7-907">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-908">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-908">SQL</span></span>

* <span data-ttu-id="00cb7-909">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="00cb7-909">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="00cb7-910">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-910">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-911">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-911">VM</span></span>

* <span data-ttu-id="00cb7-912">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="00cb7-912">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="00cb7-913">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-913">November 14, 2017</span></span>

<span data-ttu-id="00cb7-914">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="00cb7-914">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-915">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-915">ACR</span></span>

* <span data-ttu-id="00cb7-916">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="00cb7-916">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="00cb7-917">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-917">ACS</span></span>

* <span data-ttu-id="00cb7-918">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="00cb7-918">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="00cb7-919">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-919">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="00cb7-920">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="00cb7-920">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="00cb7-921">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="00cb7-921">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="00cb7-922">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="00cb7-922">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-923">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-923">Appservice</span></span>

* <span data-ttu-id="00cb7-924">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="00cb7-924">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="00cb7-925">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="00cb7-925">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="00cb7-926">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="00cb7-926">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="00cb7-927">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="00cb7-927">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="00cb7-928">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="00cb7-928">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="00cb7-929">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="00cb7-929">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-930">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-930">Batch</span></span>

* <span data-ttu-id="00cb7-931">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="00cb7-931">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="00cb7-932">Batchai</span><span class="sxs-lookup"><span data-stu-id="00cb7-932">Batchai</span></span>

* <span data-ttu-id="00cb7-933">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-933">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="00cb7-934">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-934">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="00cb7-935">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="00cb7-935">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="00cb7-936">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-936">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="00cb7-937">Nube</span><span class="sxs-lookup"><span data-stu-id="00cb7-937">Cloud</span></span>

* <span data-ttu-id="00cb7-938">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="00cb7-938">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-939">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-939">Container</span></span>

* <span data-ttu-id="00cb7-940">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="00cb7-940">Added support to open multiple ports</span></span>
* <span data-ttu-id="00cb7-941">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="00cb7-941">Added container group restart policy</span></span>
* <span data-ttu-id="00cb7-942">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="00cb7-942">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="00cb7-943">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="00cb7-943">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="00cb7-944">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00cb7-944">Data Lake Analytics</span></span>

* <span data-ttu-id="00cb7-945">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="00cb7-945">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="00cb7-946">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00cb7-946">Data Lake Store</span></span>

* <span data-ttu-id="00cb7-947">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="00cb7-947">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-948">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-948">Extension</span></span>

* <span data-ttu-id="00cb7-949">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="00cb7-949">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="00cb7-950">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="00cb7-950">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="00cb7-951">IoT</span><span class="sxs-lookup"><span data-stu-id="00cb7-951">IoT</span></span>

* <span data-ttu-id="00cb7-952">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="00cb7-952">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-953">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-953">Monitor</span></span>

* <span data-ttu-id="00cb7-954">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-954">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-955">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-955">Network</span></span>

* <span data-ttu-id="00cb7-956">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="00cb7-956">Added support for CAA DNS records</span></span>
* <span data-ttu-id="00cb7-957">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-957">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="00cb7-958">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-958">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="00cb7-959">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="00cb7-959">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="00cb7-960">Reservations</span><span class="sxs-lookup"><span data-stu-id="00cb7-960">Reservations</span></span>

* <span data-ttu-id="00cb7-961">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="00cb7-961">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-962">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-962">Resource</span></span>

* <span data-ttu-id="00cb7-963">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-963">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-964">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-964">SQL</span></span>

* <span data-ttu-id="00cb7-965">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-965">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-966">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-966">Storage</span></span>

* <span data-ttu-id="00cb7-967">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="00cb7-967">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="00cb7-968">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="00cb7-968">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="00cb7-969">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="00cb7-969">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="00cb7-970">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="00cb7-970">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="00cb7-971">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-971">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="00cb7-972">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="00cb7-972">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="00cb7-973">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="00cb7-973">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-974">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-974">VM</span></span>

* <span data-ttu-id="00cb7-975">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="00cb7-975">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="00cb7-976">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="00cb7-976">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="00cb7-977">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="00cb7-977">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="00cb7-978">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-978">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="00cb7-979">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="00cb7-979">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="00cb7-980">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-980">October 24, 2017</span></span>

<span data-ttu-id="00cb7-981">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="00cb7-981">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-982">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-982">Core</span></span>

* <span data-ttu-id="00cb7-983">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="00cb7-983">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-984">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-984">ACR</span></span>

* <span data-ttu-id="00cb7-985">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="00cb7-985">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="00cb7-986">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="00cb7-986">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="00cb7-987">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="00cb7-987">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-988">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-988">ACS</span></span>

* <span data-ttu-id="00cb7-989">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="00cb7-989">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="00cb7-990">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="00cb7-990">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-991">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-991">Appservice</span></span>

* <span data-ttu-id="00cb7-992">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="00cb7-992">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="00cb7-993">Componente</span><span class="sxs-lookup"><span data-stu-id="00cb7-993">Component</span></span>

* <span data-ttu-id="00cb7-994">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="00cb7-994">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-995">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-995">Monitor</span></span>

* <span data-ttu-id="00cb7-996">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-996">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-997">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-997">Resource</span></span>

* <span data-ttu-id="00cb7-998">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="00cb7-998">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="00cb7-999">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="00cb7-999">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1000">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1000">VM</span></span>

* <span data-ttu-id="00cb7-1001">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1001">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="00cb7-1002">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1002">October 9, 2017</span></span>

<span data-ttu-id="00cb7-1003">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="00cb7-1003">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-1004">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-1004">Core</span></span>

* <span data-ttu-id="00cb7-1005">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="00cb7-1005">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1006">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-1006">Appservice</span></span>

* <span data-ttu-id="00cb7-1007">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1007">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-1008">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-1008">Batch</span></span>

* <span data-ttu-id="00cb7-1009">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="00cb7-1009">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="00cb7-1010">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="00cb7-1010">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="00cb7-1011">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-1011">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="00cb7-1012">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="00cb7-1012">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="00cb7-1013">Batchai</span><span class="sxs-lookup"><span data-stu-id="00cb7-1013">Batchai</span></span>

* <span data-ttu-id="00cb7-1014">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-1014">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="00cb7-1015">Keyvault</span><span class="sxs-lookup"><span data-stu-id="00cb7-1015">Keyvault</span></span>

* <span data-ttu-id="00cb7-1016">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1016">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="00cb7-1017">(#4448)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1017">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="00cb7-1018">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-1018">Network</span></span>

* <span data-ttu-id="00cb7-1019">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="00cb7-1019">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="00cb7-1020">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="00cb7-1020">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-1021">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-1021">Resource</span></span>

* <span data-ttu-id="00cb7-1022">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-1022">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="00cb7-1023">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="00cb7-1023">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="00cb7-1024">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="00cb7-1024">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="00cb7-1025">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-1025">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-1026">Sql</span><span class="sxs-lookup"><span data-stu-id="00cb7-1026">Sql</span></span>

* <span data-ttu-id="00cb7-1027">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="00cb7-1027">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="00cb7-1028">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="00cb7-1028">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="00cb7-1029">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="00cb7-1029">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-1030">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1030">Storage</span></span>

* <span data-ttu-id="00cb7-1031">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="00cb7-1031">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1032">Vm</span><span class="sxs-lookup"><span data-stu-id="00cb7-1032">Vm</span></span>

* <span data-ttu-id="00cb7-1033">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="00cb7-1033">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="00cb7-1034">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1034">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="00cb7-1035">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1035">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="00cb7-1036">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1036">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="00cb7-1037">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1037">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="00cb7-1038">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1038">September 22, 2017</span></span>

<span data-ttu-id="00cb7-1039">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="00cb7-1039">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-1040">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-1040">Resource</span></span>

* <span data-ttu-id="00cb7-1041">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="00cb7-1041">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="00cb7-1042">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="00cb7-1042">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="00cb7-1043">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1043">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="00cb7-1044">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1044">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-1045">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-1045">Network</span></span>

* <span data-ttu-id="00cb7-1046">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1046">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="00cb7-1047">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1047">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="00cb7-1048">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1048">Added `asg` application security group commands</span></span>
* <span data-ttu-id="00cb7-1049">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1049">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="00cb7-1050">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1050">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="00cb7-1051">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1051">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="00cb7-1052">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1052">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-1053">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1053">Storage</span></span>

* <span data-ttu-id="00cb7-1054">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="00cb7-1054">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="00cb7-1055">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="00cb7-1055">Eventgrid</span></span>

* <span data-ttu-id="00cb7-1056">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="00cb7-1056">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-1057">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-1057">SQL</span></span>

* <span data-ttu-id="00cb7-1058">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1058">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="00cb7-1059">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="00cb7-1059">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="00cb7-1060">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1060">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="00cb7-1061">Keyvault</span><span class="sxs-lookup"><span data-stu-id="00cb7-1061">Keyvault</span></span>

* <span data-ttu-id="00cb7-1062">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="00cb7-1062">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1063">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1063">VM</span></span>

* <span data-ttu-id="00cb7-1064">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1064">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="00cb7-1065">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="00cb7-1065">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="00cb7-1066">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1066">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="00cb7-1067">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1067">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="00cb7-1068">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1068">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="00cb7-1069">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1069">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1070">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1070">ACS</span></span>

* <span data-ttu-id="00cb7-1071">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1071">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1072">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-1072">Appservice</span></span>

* <span data-ttu-id="00cb7-1073">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1073">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="00cb7-1074">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="00cb7-1074">Backup</span></span>

* <span data-ttu-id="00cb7-1075">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="00cb7-1075">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="00cb7-1076">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1076">September 11, 2017</span></span>

<span data-ttu-id="00cb7-1077">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="00cb7-1077">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="00cb7-1078">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-1078">Core</span></span>

* <span data-ttu-id="00cb7-1079">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1079">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="00cb7-1080">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1080">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1081">Acs</span></span>

* <span data-ttu-id="00cb7-1082">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1082">Added `acs list-locations` command</span></span>
* <span data-ttu-id="00cb7-1083">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1083">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1084">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-1084">Appservice</span></span>

* <span data-ttu-id="00cb7-1085">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1085">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="00cb7-1086">CDN</span><span class="sxs-lookup"><span data-stu-id="00cb7-1086">CDN</span></span>

* <span data-ttu-id="00cb7-1087">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1087">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="00cb7-1088">Extensión</span><span class="sxs-lookup"><span data-stu-id="00cb7-1088">Extension</span></span>

* <span data-ttu-id="00cb7-1089">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="00cb7-1089">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="00cb7-1090">Keyvault</span><span class="sxs-lookup"><span data-stu-id="00cb7-1090">Keyvault</span></span>

* <span data-ttu-id="00cb7-1091">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1091">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-1092">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-1092">Network</span></span>

* <span data-ttu-id="00cb7-1093">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1093">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="00cb7-1094">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1094">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="00cb7-1095">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1095">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="00cb7-1096">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1096">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="00cb7-1097">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1097">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-1098">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-1098">Resource</span></span>

* <span data-ttu-id="00cb7-1099">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1099">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="00cb7-1100">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1100">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="00cb7-1101">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1101">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="00cb7-1102">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="00cb7-1102">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-1103">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-1103">SQL</span></span>

* <span data-ttu-id="00cb7-1104">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1104">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1105">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1105">VM</span></span>

* <span data-ttu-id="00cb7-1106">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1106">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="00cb7-1107">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1107">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="00cb7-1108">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1108">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="00cb7-1109">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1109">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="00cb7-1110">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1110">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="00cb7-1111">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1111">August 31, 2017</span></span>

<span data-ttu-id="00cb7-1112">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="00cb7-1112">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="00cb7-1113">Keyvault</span><span class="sxs-lookup"><span data-stu-id="00cb7-1113">Keyvault</span></span>

* <span data-ttu-id="00cb7-1114">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1114">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="00cb7-1115">Sf</span><span class="sxs-lookup"><span data-stu-id="00cb7-1115">Sf</span></span>

* <span data-ttu-id="00cb7-1116">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1116">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-1117">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1117">Storage</span></span>

* <span data-ttu-id="00cb7-1118">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1118">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="00cb7-1119">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1119">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="00cb7-1120">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1120">August 28, 2017</span></span>

<span data-ttu-id="00cb7-1121">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="00cb7-1121">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="00cb7-1122">CLI</span><span class="sxs-lookup"><span data-stu-id="00cb7-1122">CLI</span></span>

* <span data-ttu-id="00cb7-1123">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1123">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1124">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1124">ACS</span></span>

* <span data-ttu-id="00cb7-1125">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="00cb7-1125">Corrected preview regions</span></span>
* <span data-ttu-id="00cb7-1126">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1126">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="00cb7-1127">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="00cb7-1127">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1128">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-1128">Appservice</span></span>

* <span data-ttu-id="00cb7-1129">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1129">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="00cb7-1130">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1130">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="00cb7-1131">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1131">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="00cb7-1132">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1132">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="00cb7-1133">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1133">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="00cb7-1134">IoT</span><span class="sxs-lookup"><span data-stu-id="00cb7-1134">IoT</span></span>

* <span data-ttu-id="00cb7-1135">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1135">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-1136">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-1136">Network</span></span>

* <span data-ttu-id="00cb7-1137">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1137">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="00cb7-1138">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1138">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="00cb7-1139">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1139">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="00cb7-1140">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1140">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="00cb7-1141">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1141">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-1142">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-1142">Profile</span></span>

* <span data-ttu-id="00cb7-1143">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1143">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="00cb7-1144">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00cb7-1144">Service Fabric</span></span>

* <span data-ttu-id="00cb7-1145">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="00cb7-1145">Preview release</span></span>
* <span data-ttu-id="00cb7-1146">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1146">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="00cb7-1147">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1147">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="00cb7-1148">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1148">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-1149">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1149">Storage</span></span>

* <span data-ttu-id="00cb7-1150">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1150">Enabled setting blob tier</span></span>
* <span data-ttu-id="00cb7-1151">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1151">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="00cb7-1152">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1152">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="00cb7-1153">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1153">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="00cb7-1154">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1154">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="00cb7-1155">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="00cb7-1155">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1156">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1156">VM</span></span>

* <span data-ttu-id="00cb7-1157">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1157">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="00cb7-1158">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1158">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="00cb7-1159">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1159">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="00cb7-1160">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1160">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="00cb7-1161">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1161">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="00cb7-1162">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1162">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="00cb7-1163">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1163">August 15, 2017</span></span>

<span data-ttu-id="00cb7-1164">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="00cb7-1164">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1165">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1165">ACS</span></span>

* <span data-ttu-id="00cb7-1166">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="00cb7-1166">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1167">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-1167">Appservice</span></span>

* <span data-ttu-id="00cb7-1168">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1168">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="00cb7-1169">Event Grid</span><span class="sxs-lookup"><span data-stu-id="00cb7-1169">Event Grid</span></span>

* <span data-ttu-id="00cb7-1170">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1170">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="00cb7-1171">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1171">August 11, 2017</span></span>

<span data-ttu-id="00cb7-1172">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="00cb7-1172">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1173">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1173">ACS</span></span>

* <span data-ttu-id="00cb7-1174">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="00cb7-1174">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-1175">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-1175">Batch</span></span>

* <span data-ttu-id="00cb7-1176">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1176">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="00cb7-1177">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1177">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="00cb7-1178">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1178">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="00cb7-1179">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1179">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="00cb7-1180">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1180">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="00cb7-1181">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1181">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="00cb7-1182">Componente</span><span class="sxs-lookup"><span data-stu-id="00cb7-1182">Component</span></span>

* <span data-ttu-id="00cb7-1183">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1183">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="00cb7-1184">Contenedor</span><span class="sxs-lookup"><span data-stu-id="00cb7-1184">Container</span></span>

* <span data-ttu-id="00cb7-1185">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1185">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="00cb7-1186">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00cb7-1186">Data Lake Store</span></span>

* <span data-ttu-id="00cb7-1187">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1187">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="00cb7-1188">Event Grid</span><span class="sxs-lookup"><span data-stu-id="00cb7-1188">Event Grid</span></span>

* <span data-ttu-id="00cb7-1189">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1189">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-1190">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-1190">Network</span></span>

* <span data-ttu-id="00cb7-1191">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1191">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="00cb7-1192">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1192">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="00cb7-1193">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1193">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="00cb7-1194">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1194">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-1195">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-1195">Profile</span></span>

* <span data-ttu-id="00cb7-1196">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1196">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-1197">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1197">Storage</span></span>

* <span data-ttu-id="00cb7-1198">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1198">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1199">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1199">VM</span></span>

* <span data-ttu-id="00cb7-1200">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1200">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="00cb7-1201">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1201">Exposed `list-skus` command</span></span>
* <span data-ttu-id="00cb7-1202">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1202">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="00cb7-1203">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1203">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="00cb7-1204">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1204">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="00cb7-1205">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1205">July 28, 2017</span></span>

<span data-ttu-id="00cb7-1206">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="00cb7-1206">Version 2.0.12</span></span>

* <span data-ttu-id="00cb7-1207">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1207">Added container commands</span></span>
* <span data-ttu-id="00cb7-1208">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1208">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="00cb7-1209">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-1209">Core</span></span>

* <span data-ttu-id="00cb7-1210">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1210">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="00cb7-1211">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1211">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="00cb7-1212">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1212">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="00cb7-1213">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1213">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="00cb7-1214">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1214">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="00cb7-1215">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1215">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="00cb7-1216">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1216">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="00cb7-1217">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1217">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="00cb7-1218">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1218">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="00cb7-1219">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1219">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="00cb7-1220">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1220">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="00cb7-1221">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1221">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="00cb7-1222">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1222">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="00cb7-1223">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1223">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="00cb7-1224">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1224">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="00cb7-1225">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1225">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="00cb7-1226">ACR</span><span class="sxs-lookup"><span data-stu-id="00cb7-1226">ACR</span></span>

* <span data-ttu-id="00cb7-1227">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1227">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="00cb7-1228">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1228">Support SKU update for managed registries</span></span>
* <span data-ttu-id="00cb7-1229">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1229">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="00cb7-1230">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1230">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="00cb7-1231">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1231">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="00cb7-1232">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1232">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1233">ACS</span></span>

* <span data-ttu-id="00cb7-1234">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1234">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1235">Appservice</span><span class="sxs-lookup"><span data-stu-id="00cb7-1235">Appservice</span></span>

* <span data-ttu-id="00cb7-1236">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1236">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="00cb7-1237">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1237">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="00cb7-1238">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1238">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="00cb7-1239">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1239">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="00cb7-1240">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1240">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="00cb7-1241">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1241">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="00cb7-1242">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1242">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="00cb7-1243">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1243">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="00cb7-1244">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1244">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="00cb7-1245">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1245">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="00cb7-1246">Batch</span><span class="sxs-lookup"><span data-stu-id="00cb7-1246">Batch</span></span>

* <span data-ttu-id="00cb7-1247">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1247">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="00cb7-1248">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1248">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="00cb7-1249">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1249">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="00cb7-1250">CDN</span><span class="sxs-lookup"><span data-stu-id="00cb7-1250">CDN</span></span>

* <span data-ttu-id="00cb7-1251">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="00cb7-1251">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="00cb7-1252">Nube</span><span class="sxs-lookup"><span data-stu-id="00cb7-1252">Cloud</span></span>

* <span data-ttu-id="00cb7-1253">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1253">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="00cb7-1254">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1254">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="00cb7-1255">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1255">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="00cb7-1256">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1256">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="00cb7-1257">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1257">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00cb7-1258">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00cb7-1258">CosmosDB</span></span>

* <span data-ttu-id="00cb7-1259">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1259">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="00cb7-1260">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="00cb7-1260">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="00cb7-1261">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00cb7-1261">Data Lake Analytics</span></span>

* <span data-ttu-id="00cb7-1262">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1262">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="00cb7-1263">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1263">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="00cb7-1264">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1264">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="00cb7-1265">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00cb7-1265">Data Lake Store</span></span>

* <span data-ttu-id="00cb7-1266">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1266">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="00cb7-1267">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1267">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="00cb7-1268">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1268">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="00cb7-1269">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1269">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="00cb7-1270">Interactive</span><span class="sxs-lookup"><span data-stu-id="00cb7-1270">Interactive</span></span>

* <span data-ttu-id="00cb7-1271">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1271">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="00cb7-1272">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1272">Increased test coverage</span></span>
* <span data-ttu-id="00cb7-1273">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1273">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="00cb7-1274">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1274">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="00cb7-1275">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1275">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="00cb7-1276">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1276">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="00cb7-1277">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1277">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="00cb7-1278">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1278">Added `--progress` flag</span></span>
* <span data-ttu-id="00cb7-1279">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1279">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="00cb7-1280">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1280">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="00cb7-1281">IoT</span><span class="sxs-lookup"><span data-stu-id="00cb7-1281">IoT</span></span>

* <span data-ttu-id="00cb7-1282">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1282">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="00cb7-1283">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1283">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="00cb7-1284">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="00cb7-1284">Key vault</span></span>

* <span data-ttu-id="00cb7-1285">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="00cb7-1285">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="00cb7-1286">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1286">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="00cb7-1287">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1287">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="00cb7-1288">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1288">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="00cb7-1289">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1289">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="00cb7-1290">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1290">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="00cb7-1291">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="00cb7-1291">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="00cb7-1292">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1292">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="00cb7-1293">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-1293">Lab</span></span>

* <span data-ttu-id="00cb7-1294">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1294">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="00cb7-1295">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1295">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-1296">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-1296">Monitor</span></span>

* <span data-ttu-id="00cb7-1297">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1297">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="00cb7-1298">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1298">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="00cb7-1299">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1299">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="00cb7-1300">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1300">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="00cb7-1301">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1301">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="00cb7-1302">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="00cb7-1302">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="00cb7-1303">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1303">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="00cb7-1304">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1304">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="00cb7-1305">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1305">`location` no longer required</span></span>
  * <span data-ttu-id="00cb7-1306">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1306">Add name and ID support for target</span></span>
  * <span data-ttu-id="00cb7-1307">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1307">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="00cb7-1308">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1308">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="00cb7-1309">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1309">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="00cb7-1310">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1310">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="00cb7-1311">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1311">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="00cb7-1312">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1312">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-1313">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-1313">Network</span></span>

* <span data-ttu-id="00cb7-1314">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1314">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="00cb7-1315">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1315">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="00cb7-1316">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1316">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="00cb7-1317">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1317">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="00cb7-1318">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1318">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="00cb7-1319">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1319">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="00cb7-1320">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1320">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="00cb7-1321">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1321">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="00cb7-1322">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1322">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="00cb7-1323">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1323">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="00cb7-1324">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1324">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="00cb7-1325">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1325">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="00cb7-1326">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1326">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="00cb7-1327">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1327">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="00cb7-1328">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1328">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="00cb7-1329">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1329">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="00cb7-1330">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1330">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="00cb7-1331">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1331">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="00cb7-1332">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1332">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="00cb7-1333">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1333">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="00cb7-1334">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1334">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="00cb7-1335">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1335">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="00cb7-1336">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1336">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="00cb7-1337">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1337">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="00cb7-1338">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1338">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="00cb7-1339">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1339">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="00cb7-1340">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1340">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-1341">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-1341">Profile</span></span>

* <span data-ttu-id="00cb7-1342">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1342">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="00cb7-1343">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1343">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="00cb7-1344">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="00cb7-1344">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="00cb7-1345">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1345">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="00cb7-1346">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1346">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="00cb7-1347">RDBMS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1347">RDBMS</span></span>

* <span data-ttu-id="00cb7-1348">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1348">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="00cb7-1349">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1349">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="00cb7-1350">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1350">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="00cb7-1351">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1351">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-1352">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-1352">Resource</span></span>

* <span data-ttu-id="00cb7-1353">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1353">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="00cb7-1354">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1354">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="00cb7-1355">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1355">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="00cb7-1356">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1356">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="00cb7-1357">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1357">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="00cb7-1358">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1358">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="00cb7-1359">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1359">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="00cb7-1360">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1360">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-1361">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-1361">Role</span></span>

* <span data-ttu-id="00cb7-1362">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1362">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="00cb7-1363">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1363">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="00cb7-1364">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1364">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="00cb7-1365">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1365">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="00cb7-1366">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1366">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="00cb7-1367">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00cb7-1367">Service Fabric</span></span>
* <span data-ttu-id="00cb7-1368">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1368">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="00cb7-1369">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1369">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="00cb7-1370">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1370">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-1371">SQL</span></span>

* <span data-ttu-id="00cb7-1372">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1372">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="00cb7-1373">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1373">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="00cb7-1374">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1374">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-1375">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1375">Storage</span></span>

* <span data-ttu-id="00cb7-1376">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1376">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="00cb7-1377">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1377">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="00cb7-1378">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1378">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="00cb7-1379">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1379">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="00cb7-1380">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1380">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="00cb7-1381">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1381">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1382">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1382">VM</span></span>

* <span data-ttu-id="00cb7-1383">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="00cb7-1383">Support configuring nsg</span></span>
* <span data-ttu-id="00cb7-1384">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1384">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="00cb7-1385">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1385">Support managed service identities</span></span>
* <span data-ttu-id="00cb7-1386">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1386">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="00cb7-1387">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="00cb7-1387">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="00cb7-1388">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1388">May 10, 2017</span></span>

<span data-ttu-id="00cb7-1389">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="00cb7-1389">Version 2.0.6</span></span>

* <span data-ttu-id="00cb7-1390">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1390">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="00cb7-1391">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1391">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="00cb7-1392">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00cb7-1392">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="00cb7-1393">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="00cb7-1393">Include Cognitive Services module</span></span>
* <span data-ttu-id="00cb7-1394">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="00cb7-1394">Include Service Fabric module</span></span>
* <span data-ttu-id="00cb7-1395">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1395">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="00cb7-1396">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="00cb7-1396">Add support for CDN commands</span></span>
* <span data-ttu-id="00cb7-1397">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="00cb7-1397">Remove Container module</span></span>
* <span data-ttu-id="00cb7-1398">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1398">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="00cb7-1399">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1399">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="00cb7-1400">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-1400">Core</span></span>

* <span data-ttu-id="00cb7-1401">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="00cb7-1401">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="00cb7-1402">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1402">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="00cb7-1403">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1403">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="00cb7-1404">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1404">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="00cb7-1405">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1405">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="00cb7-1406">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1406">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="00cb7-1407">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1407">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="00cb7-1408">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1408">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="00cb7-1409">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1409">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="00cb7-1410">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="00cb7-1410">core: Improved performance</span></span>
* <span data-ttu-id="00cb7-1411">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="00cb7-1411">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="00cb7-1412">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="00cb7-1412">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1413">ACS</span></span>

* <span data-ttu-id="00cb7-1414">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="00cb7-1414">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="00cb7-1415">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="00cb7-1415">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="00cb7-1416">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="00cb7-1416">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="00cb7-1417">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1417">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1418">AppService</span><span class="sxs-lookup"><span data-stu-id="00cb7-1418">AppService</span></span>

* <span data-ttu-id="00cb7-1419">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1419">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="00cb7-1420">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="00cb7-1420">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="00cb7-1421">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1421">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="00cb7-1422">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="00cb7-1422">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="00cb7-1423">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="00cb7-1423">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="00cb7-1424">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1424">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="00cb7-1425">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="00cb7-1425">support slot swap with preview</span></span>
* <span data-ttu-id="00cb7-1426">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1426">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="00cb7-1427">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1427">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="00cb7-1428">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00cb7-1428">CosmosDB</span></span>

* <span data-ttu-id="00cb7-1429">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="00cb7-1429">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="00cb7-1430">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="00cb7-1430">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="00cb7-1431">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="00cb7-1431">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="00cb7-1432">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="00cb7-1432">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="00cb7-1433">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00cb7-1433">Data Lake Analytics</span></span>

* <span data-ttu-id="00cb7-1434">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="00cb7-1434">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="00cb7-1435">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="00cb7-1435">Add support for new catalog item type: package.</span></span> <span data-ttu-id="00cb7-1436">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1436">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="00cb7-1437">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="00cb7-1437">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="00cb7-1438">Tabla</span><span class="sxs-lookup"><span data-stu-id="00cb7-1438">Table</span></span>
  * <span data-ttu-id="00cb7-1439">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="00cb7-1439">Table valued function</span></span>
  * <span data-ttu-id="00cb7-1440">Ver</span><span class="sxs-lookup"><span data-stu-id="00cb7-1440">View</span></span>
  * <span data-ttu-id="00cb7-1441">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1441">Table Statistics.</span></span> <span data-ttu-id="00cb7-1442">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="00cb7-1442">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="00cb7-1443">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00cb7-1443">Data Lake Store</span></span>

* <span data-ttu-id="00cb7-1444">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="00cb7-1444">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="00cb7-1445">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1445">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="00cb7-1446">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1446">missed help for access show.</span></span> <span data-ttu-id="00cb7-1447">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1447">adding it.</span></span> <span data-ttu-id="00cb7-1448">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1448">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="00cb7-1449">Buscar</span><span class="sxs-lookup"><span data-stu-id="00cb7-1449">Find</span></span>

* <span data-ttu-id="00cb7-1450">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="00cb7-1450">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="00cb7-1451">KeyVault</span><span class="sxs-lookup"><span data-stu-id="00cb7-1451">KeyVault</span></span>

* <span data-ttu-id="00cb7-1452">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="00cb7-1452">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="00cb7-1453">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="00cb7-1453">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="00cb7-1454">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="00cb7-1454">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="00cb7-1455">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="00cb7-1455">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="00cb7-1456">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1456">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="00cb7-1457">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-1457">Lab</span></span>

* <span data-ttu-id="00cb7-1458">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-1458">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="00cb7-1459">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-1459">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="00cb7-1460">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-1460">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="00cb7-1461">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-1461">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="00cb7-1462">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="00cb7-1462">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="00cb7-1463">Supervisión</span><span class="sxs-lookup"><span data-stu-id="00cb7-1463">Monitor</span></span>

* <span data-ttu-id="00cb7-1464">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1464">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="00cb7-1465">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1465">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="00cb7-1466">Red</span><span class="sxs-lookup"><span data-stu-id="00cb7-1466">Network</span></span>

* <span data-ttu-id="00cb7-1467">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1467">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="00cb7-1468">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1468">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="00cb7-1469">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="00cb7-1469">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="00cb7-1470">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="00cb7-1470">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="00cb7-1471">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="00cb7-1471">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="00cb7-1472">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="00cb7-1472">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="00cb7-1473">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="00cb7-1473">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="00cb7-1474">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="00cb7-1474">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="00cb7-1475">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1475">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="00cb7-1476">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="00cb7-1476">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="00cb7-1477">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1477">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="00cb7-1478">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1478">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="00cb7-1479">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="00cb7-1479">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="00cb7-1480">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="00cb7-1480">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="00cb7-1481">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="00cb7-1481">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="00cb7-1482">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="00cb7-1482">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="00cb7-1483">Perfil</span><span class="sxs-lookup"><span data-stu-id="00cb7-1483">Profile</span></span>

* <span data-ttu-id="00cb7-1484">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1484">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="00cb7-1485">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1485">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="00cb7-1486">Redis</span><span class="sxs-lookup"><span data-stu-id="00cb7-1486">Redis</span></span>

* <span data-ttu-id="00cb7-1487">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="00cb7-1487">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="00cb7-1488">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="00cb7-1488">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="00cb7-1489">Recurso</span><span class="sxs-lookup"><span data-stu-id="00cb7-1489">Resource</span></span>

* <span data-ttu-id="00cb7-1490">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1490">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="00cb7-1491">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1491">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="00cb7-1492">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1492">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="00cb7-1493">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="00cb7-1493">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="00cb7-1494">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1494">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="00cb7-1495">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="00cb7-1495">Add docs for az lock update.</span></span> <span data-ttu-id="00cb7-1496">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1496">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="00cb7-1497">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="00cb7-1497">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="00cb7-1498">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1498">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="00cb7-1499">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="00cb7-1499">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="00cb7-1500">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1500">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="00cb7-1501">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1501">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="00cb7-1502">Rol</span><span class="sxs-lookup"><span data-stu-id="00cb7-1502">Role</span></span>

* <span data-ttu-id="00cb7-1503">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1503">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="00cb7-1504">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1504">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="00cb7-1505">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1505">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="00cb7-1506">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="00cb7-1506">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="00cb7-1507">SQL</span><span class="sxs-lookup"><span data-stu-id="00cb7-1507">SQL</span></span>

* <span data-ttu-id="00cb7-1508">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="00cb7-1508">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="00cb7-1509">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1509">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="00cb7-1510">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1510">Storage</span></span>

* <span data-ttu-id="00cb7-1511">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1511">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="00cb7-1512">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="00cb7-1512">Add support for incremental blob copy</span></span>
* <span data-ttu-id="00cb7-1513">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="00cb7-1513">Add support for large block blob upload</span></span>
* <span data-ttu-id="00cb7-1514">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="00cb7-1514">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1515">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1515">VM</span></span>

* <span data-ttu-id="00cb7-1516">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="00cb7-1516">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="00cb7-1517">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="00cb7-1517">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="00cb7-1518">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="00cb7-1518">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="00cb7-1519">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="00cb7-1519">az vm/vmss disk</span></span>
  3. <span data-ttu-id="00cb7-1520">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="00cb7-1520">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="00cb7-1521">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="00cb7-1521">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="00cb7-1522">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1522">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="00cb7-1523">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1523">April 3, 2017</span></span>

<span data-ttu-id="00cb7-1524">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="00cb7-1524">Version 2.0.2</span></span>

<span data-ttu-id="00cb7-1525">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="00cb7-1525">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="00cb7-1526">Núcleo</span><span class="sxs-lookup"><span data-stu-id="00cb7-1526">Core</span></span>

* <span data-ttu-id="00cb7-1527">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="00cb7-1527">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="00cb7-1528">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1528">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="00cb7-1529">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1529">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="00cb7-1530">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1530">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="00cb7-1531">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1531">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="00cb7-1532">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1532">Add prompting for missing template parameters.</span></span> <span data-ttu-id="00cb7-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="00cb7-1534">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="00cb7-1534">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="00cb7-1535">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="00cb7-1535">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="00cb7-1536">ACS</span><span class="sxs-lookup"><span data-stu-id="00cb7-1536">ACS</span></span>

* <span data-ttu-id="00cb7-1537">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1537">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="00cb7-1538">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1538">Add support for ssh key password prompting.</span></span> <span data-ttu-id="00cb7-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="00cb7-1540">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1540">Add support for windows clusters.</span></span> <span data-ttu-id="00cb7-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="00cb7-1542">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="00cb7-1542">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="00cb7-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="00cb7-1544">AppService</span><span class="sxs-lookup"><span data-stu-id="00cb7-1544">AppService</span></span>

* <span data-ttu-id="00cb7-1545">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1545">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="00cb7-1546">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1546">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="00cb7-1547">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1547">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="00cb7-1548">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1548">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="00cb7-1549">DataLake</span><span class="sxs-lookup"><span data-stu-id="00cb7-1549">DataLake</span></span>

* <span data-ttu-id="00cb7-1550">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="00cb7-1550">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="00cb7-1551">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="00cb7-1551">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="00cb7-1552">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="00cb7-1552">DocuemntDB</span></span>

* <span data-ttu-id="00cb7-1553">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1553">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="00cb7-1554">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="00cb7-1554">VM</span></span>

* <span data-ttu-id="00cb7-1555">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1555">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="00cb7-1556">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1556">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="00cb7-1557">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1557">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="00cb7-1558">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1558">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="00cb7-1559">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1559">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="00cb7-1560">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1560">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="00cb7-1561">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="00cb7-1561">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="00cb7-1562">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="00cb7-1562">February 27, 2017</span></span>

<span data-ttu-id="00cb7-1563">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="00cb7-1563">Version 2.0.0</span></span>

<span data-ttu-id="00cb7-1564">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="00cb7-1564">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="00cb7-1565">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1565">Container Service (acs)</span></span>
- <span data-ttu-id="00cb7-1566">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1566">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="00cb7-1567">Redes</span><span class="sxs-lookup"><span data-stu-id="00cb7-1567">Networking</span></span>
- <span data-ttu-id="00cb7-1568">Storage</span><span class="sxs-lookup"><span data-stu-id="00cb7-1568">Storage</span></span>

<span data-ttu-id="00cb7-1569">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1569">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="00cb7-1570">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="00cb7-1570">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="00cb7-1571">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="00cb7-1571">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="00cb7-1572">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="00cb7-1572">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="00cb7-1573">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="00cb7-1573">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="00cb7-1574">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="00cb7-1574">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="00cb7-1575">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1575">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="00cb7-1576">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="00cb7-1576">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="00cb7-1577">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="00cb7-1577">Provide feedback from the command line with the `az feedback` command</span></span>

