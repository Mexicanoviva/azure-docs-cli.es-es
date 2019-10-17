---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 32137c5e6ef403461114b0e09970f93c9248c100
ms.sourcegitcommit: 69f52b032167a01509fdf15431e3e4e89a7e20ef
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/15/2019
ms.locfileid: "72324011"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="3707c-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="3707c-103">Azure CLI release notes</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="3707c-104">15 de octubre de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-104">October 15, 2019</span></span>

<span data-ttu-id="3707c-105">Versión 2.0.75</span><span class="sxs-lookup"><span data-stu-id="3707c-105">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="3707c-106">AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-106">AKS</span></span>

* <span data-ttu-id="3707c-107">Se ha cambiado el valor predeterminado de `--load-balancer-sku` a `standard` si es compatible con la versión de Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="3707c-107">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="3707c-108">Se ha cambiado el valor predeterminado de `--vm-set-type` a `virtualmachinescalesets` si es compatible con la versión de Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="3707c-108">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-109">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-109">AMS</span></span>

* <span data-ttu-id="3707c-110">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `job start` a `job create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-110">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="3707c-111">[CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--ask` de `content-key-policy create` para que use una cadena hexadecimal de 32 caracteres en lugar de UTF8.</span><span class="sxs-lookup"><span data-stu-id="3707c-111">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-112">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-112">AppService</span></span>

* <span data-ttu-id="3707c-113">Se han agregado comandos `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="3707c-113">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="3707c-114">Se ha agregado un mejor control de errores a `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="3707c-114">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="3707c-115">Se ha agregado compatibilidad para la SKU `Isolated` a `appservice plan update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-115">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="3707c-116">ARM</span><span class="sxs-lookup"><span data-stu-id="3707c-116">ARM</span></span>

* <span data-ttu-id="3707c-117">Se ha agregado el parámetro `--handle-extended-json-format` a `deployment create` para admitir varias líneas y comentarios en la plantilla JSON.</span><span class="sxs-lookup"><span data-stu-id="3707c-117">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="3707c-118">Proceso</span><span class="sxs-lookup"><span data-stu-id="3707c-118">Compute</span></span>

* <span data-ttu-id="3707c-119">Se ha agregado el parámetro `--enable-agent` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-119">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="3707c-120">Se ha cambiado `vm create` para que use SKU de IP pública estándar automáticamente al usar zonas.</span><span class="sxs-lookup"><span data-stu-id="3707c-120">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="3707c-121">Se ha cambiado `vm create` para que cree automáticamente un nombre de equipo válido para una máquina virtual si no se proporciona ninguno.</span><span class="sxs-lookup"><span data-stu-id="3707c-121">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="3707c-122">Se ha agregado el parámetro `--computer-name-prefix` a `vmss create` para admitir el prefijo de nombre de equipo personalizado de las máquinas virtuales en el VMSS.</span><span class="sxs-lookup"><span data-stu-id="3707c-122">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="3707c-123">Agregue el parámetro `--workspace` a `vm create` para habilitar automáticamente el área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="3707c-123">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="3707c-124">Se ha actualizado la versión de API de galerías a 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="3707c-124">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="3707c-125">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-125">Core</span></span>

* <span data-ttu-id="3707c-126">Se ha agregado la comprobación de la sintaxis del parámetro `--set` en el comando de actualización genérico.</span><span class="sxs-lookup"><span data-stu-id="3707c-126">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-127">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-127">IoT</span></span>

* <span data-ttu-id="3707c-128">Se ha corregido un problema por el que `iot hub show` producía un error con el mensaje "recurso no encontrado".</span><span class="sxs-lookup"><span data-stu-id="3707c-128">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-129">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-129">Monitor</span></span>

* <span data-ttu-id="3707c-130">Se ha agregado compatibilidad para CRUD a `monitor log-analytics workspace`.</span><span class="sxs-lookup"><span data-stu-id="3707c-130">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-131">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-131">Network</span></span>

* <span data-ttu-id="3707c-132">Se ha agregado compatibilidad para la vinculación virtual entre inquilinos a `network private-dns link vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-132">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="3707c-133">[CAMBIO IMPORTANTE] Se ha cambiado `network vnet subnet list` para requerir los parámetros `--resource-group` y `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="3707c-133">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-134">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-134">SQL</span></span>

* <span data-ttu-id="3707c-135">Se han agregado comandos a `sql mi ad-admin` que admiten la configuración de un administrador de AAD en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="3707c-135">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-136">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-136">Storage</span></span>

* <span data-ttu-id="3707c-137">Se ha agregado el parámetro `--preserve-s2s-access-tier` a `storage copy` para conservar el nivel de acceso durante la copia de servicio a servicio.</span><span class="sxs-lookup"><span data-stu-id="3707c-137">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="3707c-138">Se ha agregado el parámetro `--enable-large-file-share` a `storage account [create|update]` para admitir recursos compartidos de archivos grandes para la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="3707c-138">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="3707c-139">24 de septiembre de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-139">September 24, 2019</span></span>

<span data-ttu-id="3707c-140">Versión 2.0.74</span><span class="sxs-lookup"><span data-stu-id="3707c-140">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-141">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-141">ACR</span></span>

* <span data-ttu-id="3707c-142">Se ha agregado un parámetro `--type` obligatorio a `acr config retention update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-142">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="3707c-143">[CAMBIO IMPORTANTE] Se ha cambiado el nombre del parámetro `--name -n` a `--registry -r ` para el grupo de comandos `acr config`.</span><span class="sxs-lookup"><span data-stu-id="3707c-143">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="3707c-144">AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-144">AKS</span></span>

* <span data-ttu-id="3707c-145">Se ha agregado el parámetro `--load-balancer-sku` al comando `aks create`, lo que permite crear un clúster de AKS con SLB.</span><span class="sxs-lookup"><span data-stu-id="3707c-145">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="3707c-146">Se han agregado los parámetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` y `--load-balancer-outbound-ip-prefixes` a los comandos `aks [create|update]`, lo que permite actualizar el perfil del equilibrador de carga de un clúster de AKS con SLB.</span><span class="sxs-lookup"><span data-stu-id="3707c-146">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="3707c-147">Se ha agregado el parámetro `--vm-set-type` al comando `aks create`, lo que permite especificar los tipos de máquina virtual de un clúster de AKS (vmas o vmss).</span><span class="sxs-lookup"><span data-stu-id="3707c-147">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="3707c-148">ARM</span><span class="sxs-lookup"><span data-stu-id="3707c-148">ARM</span></span>

* <span data-ttu-id="3707c-149">Se ha agregado el parámetro `--handle-extended-json-format` al comando `group deployment create` para admitir varias líneas y comentarios en la plantilla JSON.</span><span class="sxs-lookup"><span data-stu-id="3707c-149">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="3707c-150">Proceso</span><span class="sxs-lookup"><span data-stu-id="3707c-150">Compute</span></span>

* <span data-ttu-id="3707c-151">Se ha agregado el parámetro `--terminate-notification-time` a los comandos `vmss [create|update]` para poder finalizar la capacidad de configurar eventos programados.</span><span class="sxs-lookup"><span data-stu-id="3707c-151">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="3707c-152">Se ha agregado el parámetro `--enable-terminate-notification` al comando `vmss update` para poder finalizar la capacidad de configurar eventos programados.</span><span class="sxs-lookup"><span data-stu-id="3707c-152">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="3707c-153">Se han agregado los parámetros `--priority,` `--eviction-policy,` `--max-billing` a los comandos `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-153">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="3707c-154">Se ha cambiado `disk create` para permitir especificar el tamaño exacto de la carga del disco.</span><span class="sxs-lookup"><span data-stu-id="3707c-154">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="3707c-155">Se ha agregado compatibilidad para instantáneas incrementales de discos administrados a `snapshot create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-155">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3707c-156">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3707c-156">Cosmos DB</span></span>

* <span data-ttu-id="3707c-157">Se ha agregado el parámetro `--type <key-type>` al comando `cosmosdb keys list` para mostrar la clave, las claves de solo lectura o las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="3707c-157">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="3707c-158">Se agregó el comando `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="3707c-158">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="3707c-159">[EN DESUSO] Se han dejado de usar los comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` y `cosmosdb list-read-only-keys`.</span><span class="sxs-lookup"><span data-stu-id="3707c-159">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3707c-160">EventGrid</span><span class="sxs-lookup"><span data-stu-id="3707c-160">EventGrid</span></span>

* <span data-ttu-id="3707c-161">Se ha corregido el texto de ayuda del punto de conexión para que haga referencia al parámetro correcto.</span><span class="sxs-lookup"><span data-stu-id="3707c-161">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="3707c-162">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3707c-162">Key Vault</span></span>

* <span data-ttu-id="3707c-163">Se ha corregido un problema por el que un inquilino (`login -t`) podía producir un error en `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-163">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-164">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-164">Monitor</span></span>

* <span data-ttu-id="3707c-165">Se ha corregido un problema por el que no se permitía el carácter `:` en el argumento `--condition` de `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-165">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="3707c-166">Directiva</span><span class="sxs-lookup"><span data-stu-id="3707c-166">Policy</span></span>

* <span data-ttu-id="3707c-167">Se ha agregado compatibilidad con la versión 2019-06-01 de Policy API.</span><span class="sxs-lookup"><span data-stu-id="3707c-167">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="3707c-168">Se ha agregado el parámetro `--enforcement-mode` al comando `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-168">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-169">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-169">Storage</span></span>

* <span data-ttu-id="3707c-170">Se ha agregado el parámetro `--blob-type` al comando `az storage copy`.</span><span class="sxs-lookup"><span data-stu-id="3707c-170">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="3707c-171">10 de septiembre de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-171">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-172">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-172">ACR</span></span>

* <span data-ttu-id="3707c-173">Se ha agregado el grupo de comandos `acr config retention` para configurar la directiva de retención.</span><span class="sxs-lookup"><span data-stu-id="3707c-173">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="3707c-174">AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-174">AKS</span></span>

* <span data-ttu-id="3707c-175">Se ha agregado compatibilidad para la integración de ACR con los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-175">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="3707c-176">Se ha agregado el parámetro `--attach-acr` a `aks [create|update]` para asociar un ACR a un clúster de AKS.</span><span class="sxs-lookup"><span data-stu-id="3707c-176">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="3707c-177">Se ha agregado el parámetro `--detach-acr` a `aks update` para desasociar un ACR de un clúster de AKS.</span><span class="sxs-lookup"><span data-stu-id="3707c-177">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="3707c-178">ARM</span><span class="sxs-lookup"><span data-stu-id="3707c-178">ARM</span></span>

* <span data-ttu-id="3707c-179">Se ha actualizado para usar la versión 2019-05-10 de la API.</span><span class="sxs-lookup"><span data-stu-id="3707c-179">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-180">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-180">Batch</span></span>

* <span data-ttu-id="3707c-181">Se han agregado nuevas opciones de configuración de JSON a `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="3707c-181">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="3707c-182">Se ha agregado `MountConfigurations` para montajes del sistema de archivos (consulte https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body para obtener más información).</span><span class="sxs-lookup"><span data-stu-id="3707c-182">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="3707c-183">Se ha agregado la propiedad `publicIPs` opcional en `NetworkConfiguration` para las direcciones IP públicas en grupos (consulte https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body para obtener más información).</span><span class="sxs-lookup"><span data-stu-id="3707c-183">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/en-us/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="3707c-184">Se ha agregado compatibilidad para la galería de imágenes compartidas a `--image`.</span><span class="sxs-lookup"><span data-stu-id="3707c-184">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="3707c-185">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--start-task-wait-for-success` en `batch pool create` a `true`.</span><span class="sxs-lookup"><span data-stu-id="3707c-185">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="3707c-186">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `Scope` en `AutoUserSpecification` para que siempre sea Pool (era `Task` en los nodos Windows, `Pool` en los nodos Linux).</span><span class="sxs-lookup"><span data-stu-id="3707c-186">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="3707c-187">Este argumento solo se puede establecer desde una configuración de JSON con `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="3707c-187">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-188">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-188">HDInsight</span></span>

* <span data-ttu-id="3707c-189">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="3707c-189">GA release</span></span>
* <span data-ttu-id="3707c-190">[CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--workernode-count/-c` de `az hdinsight resize` para que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="3707c-190">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="3707c-191">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3707c-191">Key Vault</span></span>

* <span data-ttu-id="3707c-192">Se ha corregido un problema por el que no se podían eliminar las subredes de las reglas de red.</span><span class="sxs-lookup"><span data-stu-id="3707c-192">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="3707c-193">Se ha corregido un problema por el que se podían agregar subredes y direcciones IP duplicadas a las reglas de red.</span><span class="sxs-lookup"><span data-stu-id="3707c-193">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="3707c-194">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-194">Network</span></span>

* <span data-ttu-id="3707c-195">Se ha agregado el parámetro `--interval` a `network watcher flow-log` para establecer el valor del intervalo de análisis del tráfico.</span><span class="sxs-lookup"><span data-stu-id="3707c-195">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="3707c-196">Se ha agregado `network application-gateway identity` para administrar la identidad de puerta de enlace.</span><span class="sxs-lookup"><span data-stu-id="3707c-196">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="3707c-197">Se ha agregado compatibilidad para establecer el identificador del almacén de claves en `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="3707c-197">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="3707c-198">Se agregó `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-198">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="3707c-199">Directiva</span><span class="sxs-lookup"><span data-stu-id="3707c-199">Policy</span></span>

* <span data-ttu-id="3707c-200">Se ha actualizado para usar la versión 2019-01-01 de la API.</span><span class="sxs-lookup"><span data-stu-id="3707c-200">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="3707c-201">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-201">August 27, 2019</span></span>

<span data-ttu-id="3707c-202">Versión 2.0.72</span><span class="sxs-lookup"><span data-stu-id="3707c-202">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-203">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-203">ACR</span></span>

* <span data-ttu-id="3707c-204">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para la SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="3707c-204">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="3707c-205">API Management</span><span class="sxs-lookup"><span data-stu-id="3707c-205">API Management</span></span>

* <span data-ttu-id="3707c-206">[VERSIÓN PRELIMINAR] Se ha agregado el grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="3707c-206">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-207">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-207">AppService</span></span>

* <span data-ttu-id="3707c-208">Se ha corregido un problema con el comando `webapp webjob continuous start` al especificar una ranura</span><span class="sxs-lookup"><span data-stu-id="3707c-208">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="3707c-209">Se ha cambiado `webapp up` para detectar la carpeta `env` y quitarla del archivo usado para la implementación</span><span class="sxs-lookup"><span data-stu-id="3707c-209">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-210">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3707c-210">Keyvault</span></span>

* <span data-ttu-id="3707c-211">Se ha corregido un error en `keyvault secret set` que hacía que se ignorara el argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="3707c-211">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="3707c-212">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-212">Network</span></span>

* <span data-ttu-id="3707c-213">Se ha agregado compatibilidad para las direcciones IPv6 con argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="3707c-213">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="3707c-214">Se han agregado nuevos comandos `network private-endpoint [create|update|list-types]` para la administración de un punto de conexión privado</span><span class="sxs-lookup"><span data-stu-id="3707c-214">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="3707c-215">Se ha agregado el grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="3707c-215">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="3707c-216">Se agregaron los argumentos `--private-endpoint-network-policies` y `--private-link-service-network-policies` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="3707c-216">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="3707c-217">RBAC</span><span class="sxs-lookup"><span data-stu-id="3707c-217">RBAC</span></span>

* <span data-ttu-id="3707c-218">Se ha corregido el problema con `ad app update --homepage` por el cual la página principal no se actualizaba</span><span class="sxs-lookup"><span data-stu-id="3707c-218">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="3707c-219">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3707c-219">ServiceFabric</span></span>

* <span data-ttu-id="3707c-220">Se ha agregado compatibilidad con los nombres de Key Vault que combinan mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="3707c-220">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="3707c-221">Se ha solucionado el problema que se producía al usar certificados en Key Vault</span><span class="sxs-lookup"><span data-stu-id="3707c-221">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="3707c-222">Se ha solucionado el problema con el uso de archivos de certificado de PFX</span><span class="sxs-lookup"><span data-stu-id="3707c-222">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="3707c-223">Se ha solucionado el problema con `sf cluster certificate add` que se producía cuando no se especificaba el grupo de recursos de Key Vault</span><span class="sxs-lookup"><span data-stu-id="3707c-223">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="3707c-224">Se ha corregido el problema con `sf cluster set` que no funcionaba</span><span class="sxs-lookup"><span data-stu-id="3707c-224">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="3707c-225">SignalR</span><span class="sxs-lookup"><span data-stu-id="3707c-225">SignalR</span></span>

* <span data-ttu-id="3707c-226">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-226">Added new commands:</span></span>
  * <span data-ttu-id="3707c-227">`signalr cors`: Administración de SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="3707c-227">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="3707c-228">`signalr restart`: Reinicio de una instancia de SignalR Service</span><span class="sxs-lookup"><span data-stu-id="3707c-228">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="3707c-229">`signalr update`: Actualización de una instancia de SignalR Service</span><span class="sxs-lookup"><span data-stu-id="3707c-229">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="3707c-230">Se agregó el argumento `--service-mode` a `signalr create`</span><span class="sxs-lookup"><span data-stu-id="3707c-230">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-231">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-231">Storage</span></span>

* <span data-ttu-id="3707c-232">Se agregó el comando `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="3707c-232">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="3707c-233">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-233">August 13, 2019</span></span>

<span data-ttu-id="3707c-234">Versión 2.0.71</span><span class="sxs-lookup"><span data-stu-id="3707c-234">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-235">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-235">AppService</span></span>

* <span data-ttu-id="3707c-236">Se ha corregido un problema por el que se producían errores con los comandos `webapp webjob continuous` en los espacios</span><span class="sxs-lookup"><span data-stu-id="3707c-236">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-237">BotService</span><span class="sxs-lookup"><span data-stu-id="3707c-237">BotService</span></span>

* <span data-ttu-id="3707c-238">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para crear bots con el SDK v3.</span><span class="sxs-lookup"><span data-stu-id="3707c-238">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="3707c-239">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="3707c-239">CognitiveServices</span></span>

* <span data-ttu-id="3707c-240">Se agregaron los comandos `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-240">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3707c-241">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3707c-241">Cosmos DB</span></span>

* <span data-ttu-id="3707c-242">Se ha quitado la advertencia al actualizar varias ubicaciones de escritura.</span><span class="sxs-lookup"><span data-stu-id="3707c-242">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="3707c-243">Se han agregado comandos CRUD para recursos de CosmosDB SQL, MongoDB, Cassandra, Gremlin y Table, así como capacidad de proceso para los recursos.</span><span class="sxs-lookup"><span data-stu-id="3707c-243">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-244">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-244">HDInsight</span></span>

<span data-ttu-id="3707c-245">Esta versión contiene un gran número de cambios importantes.</span><span class="sxs-lookup"><span data-stu-id="3707c-245">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="3707c-246">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="3707c-246">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="3707c-247">Se cambió el nombre de `--storage-default-container` a `--storage-container`.</span><span class="sxs-lookup"><span data-stu-id="3707c-247">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="3707c-248">Se cambió el nombre de `--storage-default-filesystem` a `--storage-filesystem`.</span><span class="sxs-lookup"><span data-stu-id="3707c-248">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="3707c-249">[CAMBIO IMPORTANTE] Se ha cambiado el argumento `--name` de `application create` para que represente el nombre de la aplicación en lugar del nombre del clúster.</span><span class="sxs-lookup"><span data-stu-id="3707c-249">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="3707c-250">Se ha agregado el argumento `--cluster-name` a `application create` para reemplazar la funcionalidad de `--name` antigua.</span><span class="sxs-lookup"><span data-stu-id="3707c-250">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="3707c-251">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `application create`:</span><span class="sxs-lookup"><span data-stu-id="3707c-251">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="3707c-252">Se cambió el nombre de `--application-type` a `--type`.</span><span class="sxs-lookup"><span data-stu-id="3707c-252">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="3707c-253">Se cambió el nombre de `--marketplace-identifier` a `--marketplace-id`.</span><span class="sxs-lookup"><span data-stu-id="3707c-253">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="3707c-254">Se cambió el nombre de `--https-endpoint-access-mode` a `--access-mode`.</span><span class="sxs-lookup"><span data-stu-id="3707c-254">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="3707c-255">Se cambió el nombre de `--https-endpoint-destination-port` a `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="3707c-255">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="3707c-256">[CAMBIO IMPORTANTE] Se han quitado los parámetros de `application create`:</span><span class="sxs-lookup"><span data-stu-id="3707c-256">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="3707c-257">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--target-instance-count` a `--workernode-count` para `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="3707c-257">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="3707c-258">[CAMBIO IMPORTANTE] Se han cambiado todos los comandos del grupo `hdinsight script-action` para que usen el parámetro `--name` como nombre de la acción de script.</span><span class="sxs-lookup"><span data-stu-id="3707c-258">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="3707c-259">Se ha agregado el argumento `--cluster-name` a todos los comandos `hdinsight script-action` para reemplazar la funcionalidad de `--name` antigua.</span><span class="sxs-lookup"><span data-stu-id="3707c-259">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="3707c-260">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--script-execution-id` a `--execution-id` para todos los comandos `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="3707c-260">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="3707c-261">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `hdinsight script-action show` a `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="3707c-261">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="3707c-262">[CAMBIO IMPORTANTE] Se han cambiado los parámetros a `hdinsight script-action execute --roles` para que estén separados por espacios en lugar de por comas.</span><span class="sxs-lookup"><span data-stu-id="3707c-262">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="3707c-263">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--persisted` de `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="3707c-263">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="3707c-264">Se ha cambiado el parámetro `hdinsight create --cluster-configurations` para aceptar una ruta a un archivo JSON local o una cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="3707c-264">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="3707c-265">Se ha agregado el comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="3707c-265">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="3707c-266">Se ha cambiado `hdinsight monitor enable --workspace` para aceptar un identificador o un nombre de área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="3707c-266">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="3707c-267">Se ha agregado el argumento `hdinsight monitor enable --primary-key`, que es necesario si se proporciona un identificador de área de trabajo como parámetro.</span><span class="sxs-lookup"><span data-stu-id="3707c-267">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="3707c-268">Se han agregado más ejemplos y se han actualizado las descripciones para los mensajes de ayuda.</span><span class="sxs-lookup"><span data-stu-id="3707c-268">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-269">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-269">Interactive</span></span>

* <span data-ttu-id="3707c-270">Se ha corregido un error de carga.</span><span class="sxs-lookup"><span data-stu-id="3707c-270">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="3707c-271">kubernetes</span><span class="sxs-lookup"><span data-stu-id="3707c-271">Kubernetes</span></span>

* <span data-ttu-id="3707c-272">Se ha cambiado para usar `https` si el puerto del contenedor del panel usa `https`.</span><span class="sxs-lookup"><span data-stu-id="3707c-272">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-273">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-273">Network</span></span>

* <span data-ttu-id="3707c-274">Se ha agregado el argumento `network dns record-set cname delete` a `--yes`.</span><span class="sxs-lookup"><span data-stu-id="3707c-274">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-275">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-275">Profile</span></span>

* <span data-ttu-id="3707c-276">Se ha agregado el argumento `--resource-type` a `account get-access-token` para obtener los tokens de acceso a recursos.</span><span class="sxs-lookup"><span data-stu-id="3707c-276">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="3707c-277">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3707c-277">ServiceFabric</span></span>

* <span data-ttu-id="3707c-278">Se han agregado todas las versiones del sistema operativo compatible para la creación de clústeres SF.</span><span class="sxs-lookup"><span data-stu-id="3707c-278">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="3707c-279">Se ha corregido el error de validación de certificado principal.</span><span class="sxs-lookup"><span data-stu-id="3707c-279">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-280">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-280">Storage</span></span>

* <span data-ttu-id="3707c-281">Se ha agregado el comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="3707c-281">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="3707c-282">30 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-282">July 30, 2019</span></span>

<span data-ttu-id="3707c-283">Versión 2.0.70</span><span class="sxs-lookup"><span data-stu-id="3707c-283">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-284">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-284">ACR</span></span>

* <span data-ttu-id="3707c-285">Se ha corregido el problema 9952 (una regresión en el comando `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="3707c-285">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="3707c-286">Se ha quitado el nombre predeterminado de la imagen del generador en `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="3707c-286">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-287">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-287">Appservice</span></span>

* <span data-ttu-id="3707c-288">Se ha cambiado `webapp config ssl` para que muestre un mensaje si no se encuentra un recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-288">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="3707c-289">Se ha corregido un problema por el que `functionapp create` no acepta el tipo de cuenta de almacenamiento `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="3707c-289">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="3707c-290">Se ha corregido un problema por el que `webapp up` producía un error si se ejecutaba con versiones anteriores de Python.</span><span class="sxs-lookup"><span data-stu-id="3707c-290">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="3707c-291">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-291">Network</span></span>

* <span data-ttu-id="3707c-292">Se ha quitado un parámetro no válido `--ids` de `network nic ip-config add` (corrige el problema 9861).</span><span class="sxs-lookup"><span data-stu-id="3707c-292">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="3707c-293">Corrige el problema 9604.</span><span class="sxs-lookup"><span data-stu-id="3707c-293">Fixes #9604.</span></span> <span data-ttu-id="3707c-294">Se ha agregado el parámetro `--root-certs` a `network application-gateway http-settings [create|update]` para admitir los certificados raíz de confianza de los usuarios asociados.</span><span class="sxs-lookup"><span data-stu-id="3707c-294">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="3707c-295">Se ha corregido el argumento `--subscription` para `network dns record-set ns create` (9965).</span><span class="sxs-lookup"><span data-stu-id="3707c-295">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="3707c-296">RBAC</span><span class="sxs-lookup"><span data-stu-id="3707c-296">RBAC</span></span>

* <span data-ttu-id="3707c-297">Se agregó el comando `user update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-297">Added `user update` command</span></span>
* <span data-ttu-id="3707c-298">[EN DESUSO] Se ha dejado de usar `--upn-or-object-id` en los comandos relacionados con el usuario.</span><span class="sxs-lookup"><span data-stu-id="3707c-298">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="3707c-299">Use el nuevo argumento `--id`.</span><span class="sxs-lookup"><span data-stu-id="3707c-299">Use replacement argument `--id`</span></span>
* <span data-ttu-id="3707c-300">Se ha agregado el argumento `--id` a los comandos relacionados con el usuario.</span><span class="sxs-lookup"><span data-stu-id="3707c-300">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-301">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-301">SQL</span></span>

* <span data-ttu-id="3707c-302">Se han agregado comandos de administración para claves de instancia administrada y protector de TDE.</span><span class="sxs-lookup"><span data-stu-id="3707c-302">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-303">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-303">Storage</span></span>

* <span data-ttu-id="3707c-304">Se agregó el comando `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="3707c-304">Added `storage remove` command</span></span>
* <span data-ttu-id="3707c-305">Se ha corregido un error con `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-305">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-306">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-306">VM</span></span>

* <span data-ttu-id="3707c-307">Se ha cambiado `list-skus` para que use la versión más reciente de la API para generar los detalles de la zona.</span><span class="sxs-lookup"><span data-stu-id="3707c-307">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="3707c-308">Se ha cambiado el valor predeterminado de `--single-placement-group` a `false` para `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-308">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="3707c-309">Se ha agregado la posibilidad de seleccionar SKU de almacenamiento ZRS para `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-309">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="3707c-310">Se ha agregado un nuevo grupo de comandos `vm host` para admitir hosts dedicados.</span><span class="sxs-lookup"><span data-stu-id="3707c-310">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="3707c-311">Se han agregado los parámetros `--host` y `--host-group` en `vm create` para establecer un host dedicado de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="3707c-311">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="3707c-312">16 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-312">July 16, 2019</span></span>

<span data-ttu-id="3707c-313">Versión 2.0.69</span><span class="sxs-lookup"><span data-stu-id="3707c-313">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-314">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-314">Appservice</span></span>

* <span data-ttu-id="3707c-315">Se han cambiado los comandos de `webapp identity` para devolver un mensaje de error adecuado si el nombre del grupo de recursos o la aplicación no es válido.</span><span class="sxs-lookup"><span data-stu-id="3707c-315">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="3707c-316">Se ha corregido `webapp list` para devolver el valor correcto de numberOfSites si no se ha proporcionado ningún grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="3707c-316">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="3707c-317">Se han corregido los efectos secundarios de `appservice plan create` y `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-317">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="3707c-318">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-318">Core</span></span>

* <span data-ttu-id="3707c-319">Se ha corregido el problema por el que `--subscription` aparecía a pesar de no ser aplicable.</span><span class="sxs-lookup"><span data-stu-id="3707c-319">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-320">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-320">Batch</span></span>

* <span data-ttu-id="3707c-321">[CAMBIO IMPORTANTE] Se ha reemplazado `batch pool node-agent-skus list` por `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="3707c-321">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="3707c-322">Se ha agregado compatibilidad con las reglas de seguridad que bloquea el acceso de red a un grupo basado en el puerto de origen del tráfico cuando se usa la opción `--json-file` de `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="3707c-322">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="3707c-323">Agrega compatibilidad para ejecutar la tarea en el directorio de trabajo del contenedor o en el directorio de trabajo de la tarea por lotes cuando se usa la opción `--json-file` de `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-323">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="3707c-324">Se ha corregido el error en la opción `--application-package-references` de `batch pool create` por el que solo funcionaba con los valores predeterminados.</span><span class="sxs-lookup"><span data-stu-id="3707c-324">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="3707c-325">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="3707c-325">Eventhubs</span></span>

* <span data-ttu-id="3707c-326">Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-326">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-327">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-327">RDBMS</span></span>

* <span data-ttu-id="3707c-328">Se ha agregado un parámetro opcional para especificar la SKU de réplica para crear comandos de réplica.</span><span class="sxs-lookup"><span data-stu-id="3707c-328">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="3707c-329">Se ha corregido el problema con el error de prueba de CI al crear la réplica de MySQL.</span><span class="sxs-lookup"><span data-stu-id="3707c-329">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="3707c-330">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="3707c-330">Relay</span></span>

* <span data-ttu-id="3707c-331">Se ha corregido el problema con la conexión híbrida cuando la autorización del cliente está deshabilitada [n.º 8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="3707c-331">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="3707c-332">Se ha agregado el parámetro `--requires-transport-security` a `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-332">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="3707c-333">Servicebus</span><span class="sxs-lookup"><span data-stu-id="3707c-333">Servicebus</span></span>

* <span data-ttu-id="3707c-334">Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-334">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-335">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-335">Storage</span></span>

* <span data-ttu-id="3707c-336">Habilitar archivos AADDS para la actualización de la cuenta de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="3707c-336">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="3707c-337">Se ha corregido el problema `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="3707c-337">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="3707c-338">2 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-338">July 2, 2019</span></span>

<span data-ttu-id="3707c-339">Versión 2.0.68</span><span class="sxs-lookup"><span data-stu-id="3707c-339">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="3707c-340">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-340">Core</span></span>

* <span data-ttu-id="3707c-341">Los módulos de comandos ahora se consolidan en un único paquete distribuible de Python.</span><span class="sxs-lookup"><span data-stu-id="3707c-341">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="3707c-342">Esto reemplaza el uso directo de muchos paquetes `azure-cli-` en PyPI.</span><span class="sxs-lookup"><span data-stu-id="3707c-342">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="3707c-343">Esto reducirá el tamaño de la instalación y solo afecta a los usuarios que hayan instalado directamente mediante `pip`.</span><span class="sxs-lookup"><span data-stu-id="3707c-343">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-344">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-344">ACR</span></span>

* <span data-ttu-id="3707c-345">Se ha agregado compatibilidad para los desencadenadores de temporizador para las tareas.</span><span class="sxs-lookup"><span data-stu-id="3707c-345">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-346">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-346">Appservice</span></span>

* <span data-ttu-id="3707c-347">Se ha cambiado `functionapp create` para habilitar Application Insights de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3707c-347">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="3707c-348">[CAMBIO IMPORTANTE] Se ha dejado de utilizar el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="3707c-348">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="3707c-349">Use el nuevo comando `az functionapp devops-pipeline` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="3707c-349">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="3707c-350">Se ha agregado compatibilidad con el plan de aplicación de funciones Consumo para Linux a `functionapp deployment config-zip`.</span><span class="sxs-lookup"><span data-stu-id="3707c-350">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3707c-351">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3707c-351">Cosmos DB</span></span>

* <span data-ttu-id="3707c-352">Se ha agregado compatibilidad para deshabilitar TTL.</span><span class="sxs-lookup"><span data-stu-id="3707c-352">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="3707c-353">DLS</span><span class="sxs-lookup"><span data-stu-id="3707c-353">DLS</span></span>

* <span data-ttu-id="3707c-354">Se ha actualizado la versión de ADLS (0.0.45).</span><span class="sxs-lookup"><span data-stu-id="3707c-354">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="3707c-355">Comentarios</span><span class="sxs-lookup"><span data-stu-id="3707c-355">Feedback</span></span>

* <span data-ttu-id="3707c-356">Al informar de un error de comando de extensión, `az feedback` ahora intenta abrir el explorador en la dirección URL del repositorio del proyecto de la extensión desde el índice.</span><span class="sxs-lookup"><span data-stu-id="3707c-356">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-357">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-357">HDInsight</span></span>

* <span data-ttu-id="3707c-358">[CAMBIO IMPORTANTE] Se ha cambiado el nombre del grupo de comandos `oms` por `monitor`.</span><span class="sxs-lookup"><span data-stu-id="3707c-358">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="3707c-359">[CAMBIO IMPORTANTE] Ahora `--http-password/-p` es un parámetro necesario.</span><span class="sxs-lookup"><span data-stu-id="3707c-359">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="3707c-360">Se han agregado completadores para los parámetros `--cluster-admin-account` y `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="3707c-360">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="3707c-361">Se ha cambiado el parámetro `cluster-users-group-dns` para que sea necesario cuando `—esp` está presente.</span><span class="sxs-lookup"><span data-stu-id="3707c-361">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="3707c-362">Se ha agregado un tiempo de espera para todos los autocompletadores de argumentos existentes.</span><span class="sxs-lookup"><span data-stu-id="3707c-362">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="3707c-363">Se ha agregado un tiempo de espera para transformar el nombre de recurso en un identificador de recurso.</span><span class="sxs-lookup"><span data-stu-id="3707c-363">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="3707c-364">Se han cambiado los autocompletadores para seleccionar recursos de cualquier grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="3707c-364">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="3707c-365">Puede ser un grupo de recursos diferente a que se especifica con `-g`.</span><span class="sxs-lookup"><span data-stu-id="3707c-365">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="3707c-366">Se ha agregado compatibilidad con los parámetros `--sub-domain-suffix` y `--disable_gateway_auth` en el comando `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-366">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="3707c-367">Servicios administrados</span><span class="sxs-lookup"><span data-stu-id="3707c-367">Managed Services</span></span>

* <span data-ttu-id="3707c-368">Se ha introducido un módulo de comandos de servicios administrados en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="3707c-368">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-369">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-369">Profile</span></span>
* <span data-ttu-id="3707c-370">Se ha suprimido el argumento `--subscription` del comando de cierre de sesión.</span><span class="sxs-lookup"><span data-stu-id="3707c-370">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="3707c-371">RBAC</span><span class="sxs-lookup"><span data-stu-id="3707c-371">RBAC</span></span>

* <span data-ttu-id="3707c-372">[CAMBIO IMPORTANTE] Se ha quitado el argumento `--password` de `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="3707c-372">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="3707c-373">Se ha agregado el parámetro `--assignee-principal-type` al comando `create` para evitar errores intermitentes causados por la latencia de replicación del servidor de grafos de AAD.</span><span class="sxs-lookup"><span data-stu-id="3707c-373">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="3707c-374">Se ha corregido un bloqueo en `ad signed-in-user` al enumerar los objetos que posee.</span><span class="sxs-lookup"><span data-stu-id="3707c-374">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="3707c-375">Se ha corregido el problema por el que `ad sp` no encontraba la aplicación correcta en una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="3707c-375">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-376">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-376">RDBMS</span></span>

* <span data-ttu-id="3707c-377">Se ha agregado compatibilidad para la replicación a MariaDB.</span><span class="sxs-lookup"><span data-stu-id="3707c-377">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-378">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-378">SQL</span></span>

* <span data-ttu-id="3707c-379">Se han documentado los valores permitidos para `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="3707c-379">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-380">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-380">Storage</span></span>

* <span data-ttu-id="3707c-381">Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="3707c-381">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="3707c-382">Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="3707c-382">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="3707c-383">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-383">VM</span></span>

* <span data-ttu-id="3707c-384">Se ha corregido un error por el que `vmss create` devuelve un mensaje de error cuando se ejecuta con `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-384">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="3707c-385">Se ha quitado la validación del lado cliente para `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="3707c-385">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="3707c-386">No genera ningún error si `--single-placement-group` está establecido en `true` y `--instance-count` es mayor que 100 o se especifican zonas de disponibilidad, y deja esta validación al servicio de proceso.</span><span class="sxs-lookup"><span data-stu-id="3707c-386">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="3707c-387">Se ha corregido el error por el que `[vm|vmss] extension image list` produce un error cuando se usa con `--latest`.</span><span class="sxs-lookup"><span data-stu-id="3707c-387">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="3707c-388">18 de junio de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-388">June 18, 2019</span></span>

<span data-ttu-id="3707c-389">Versión 2.0.67</span><span class="sxs-lookup"><span data-stu-id="3707c-389">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="3707c-390">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-390">Core</span></span>

<span data-ttu-id="3707c-391">Esta versión introduce una nueva etiqueta [Preview] para indicar con mayor claridad a los clientes si un grupo de comandos, un comando o un argumento está en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="3707c-391">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="3707c-392">Antes esto se comunicaba en el texto de ayuda o se indicaba explícitamente en el número de versión del módulo de comandos.</span><span class="sxs-lookup"><span data-stu-id="3707c-392">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="3707c-393">La CLI eliminará los números de versión de los paquetes individuales en el futuro.</span><span class="sxs-lookup"><span data-stu-id="3707c-393">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="3707c-394">Si un comando está en versión preliminar, todos sus argumentos también lo están.</span><span class="sxs-lookup"><span data-stu-id="3707c-394">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="3707c-395">Si un grupo de comandos está etiquetado como versión preliminar, se consideran que todos los comandos y argumentos también están en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="3707c-395">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="3707c-396">Como resultado de este cambio, pueden parecer que varios grupos de comandos están "repentinamente" en versión preliminar con esta versión.</span><span class="sxs-lookup"><span data-stu-id="3707c-396">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="3707c-397">Lo que realmente ha sucede es que la mayoría de los paquetes estaban en versión preliminar, pero se considera que están disponibles con carácter general con esta versión.</span><span class="sxs-lookup"><span data-stu-id="3707c-397">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-398">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-398">ACR</span></span>
* <span data-ttu-id="3707c-399">Se ha agregado el comando "acr check-health".</span><span class="sxs-lookup"><span data-stu-id="3707c-399">Added 'acr check-health' command</span></span>
* <span data-ttu-id="3707c-400">Mejor control de los errores para los tokens AAD y para recuperar los comandos externos.</span><span class="sxs-lookup"><span data-stu-id="3707c-400">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-401">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-401">ACS</span></span>
* <span data-ttu-id="3707c-402">Los comandos en desuso de ACS ya no se muestran en la vista de la ayuda.</span><span class="sxs-lookup"><span data-stu-id="3707c-402">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-403">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-403">AMS</span></span>
* <span data-ttu-id="3707c-404">[CAMBIO IMPORTANTE] Las cadenas de hora ISO 8601 se han cambiado para volver a archive-window-length y key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="3707c-404">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-405">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-405">AppService</span></span>
* <span data-ttu-id="3707c-406">Se ha agregado el enrutamiento basado en la ubicación para `webapp deleted list` y `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="3707c-406">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="3707c-407">Se ha corregido el problema por el que no se podía hacer clic la dirección URL de destino registrada de la aplicación web ("Puede iniciar la aplicación en...") en Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="3707c-407">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="3707c-408">Se ha corregido el problema por el que, al crear aplicaciones con algunas SKU, se producía un error de AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="3707c-408">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="3707c-409">Se ha agregado validación previa a `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-409">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="3707c-410">Se ha corregido `[webapp|functionapp] traffic-routing` para usar el valor correcto de actionHostName.</span><span class="sxs-lookup"><span data-stu-id="3707c-410">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="3707c-411">Se ha agregado compatibilidad con ranuras a los comandos `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="3707c-411">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-412">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-412">Batch</span></span>
* <span data-ttu-id="3707c-413">Se ha corregido la regresión de autenticación de AAD causada por una notificación demasiado agresiva de errores de autenticación de clave compartida.</span><span class="sxs-lookup"><span data-stu-id="3707c-413">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="3707c-414">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3707c-414">BatchAI</span></span>
* <span data-ttu-id="3707c-415">Los comandos de BatchAI han dejado de usarse y están ocultos.</span><span class="sxs-lookup"><span data-stu-id="3707c-415">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-416">BotService</span><span class="sxs-lookup"><span data-stu-id="3707c-416">BotService</span></span>
* <span data-ttu-id="3707c-417">Se ha agregado un aviso de advertencia "compatibilidad descontinuada" o "modo de mantenimiento" a los comandos que admiten el SDK v3.</span><span class="sxs-lookup"><span data-stu-id="3707c-417">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-418">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-418">CosmosDB</span></span>
* <span data-ttu-id="3707c-419">[EN DESUSO] Se ha dejado de usar el comando `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="3707c-419">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="3707c-420">Se ha agregado el comando `cosmosdb keys list`, que reemplaza a `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="3707c-420">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="3707c-421">`cosmsodb create/update`: Se ha agregado el nuevo formato a --location para poder establecer la propiedad "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="3707c-421">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="3707c-422">Formato antiguo en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-422">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3707c-423">EventGrid</span><span class="sxs-lookup"><span data-stu-id="3707c-423">EventGrid</span></span>
* <span data-ttu-id="3707c-424">Se han agregado comandos `eventgrid domain` para las operaciones CRUD de dominios.</span><span class="sxs-lookup"><span data-stu-id="3707c-424">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="3707c-425">Se han agregado comandos `eventgrid domain topic` para las operaciones CRUD de temas de dominio.</span><span class="sxs-lookup"><span data-stu-id="3707c-425">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="3707c-426">Se ha agregado el argumento `--odata-query` a `eventgrid [topic|event-subscription] list` para filtrar los resultados mediante la sintaxis de OData.</span><span class="sxs-lookup"><span data-stu-id="3707c-426">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="3707c-427">`event-subscription create/update`: Se ha agregado servicebusqueue como nuevos valores para el parámetro `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="3707c-427">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="3707c-428">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para `--included-event-types All` con `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-428">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-429">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-429">HDInsight</span></span>
* <span data-ttu-id="3707c-430">Se ha agregado compatibilidad con el parámetro `--ssh-public-key` al comando `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-430">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-431">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-431">IoT</span></span>
* <span data-ttu-id="3707c-432">Se ha agregado compatibilidad para volver a generar las claves de directiva de autorización.</span><span class="sxs-lookup"><span data-stu-id="3707c-432">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="3707c-433">Se ha agregado un SDK y compatibilidad con el servicio de aprovisionamiento de repositorio de DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="3707c-433">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="3707c-434">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-434">Network</span></span>
* <span data-ttu-id="3707c-435">Se ha agregado compatibilidad de las zonas con puertas de enlace NAT.</span><span class="sxs-lookup"><span data-stu-id="3707c-435">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="3707c-436">Se ha agregado el comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="3707c-436">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="3707c-437">Se ha corregido el problema con `dns zone import` por el que los usuarios no podían importar registros A con caracteres comodín.</span><span class="sxs-lookup"><span data-stu-id="3707c-437">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="3707c-438">Se ha corregido el problema con `watcher flow-log configure` por el que no se podía habilitar el registro de flujos en determinadas regiones.</span><span class="sxs-lookup"><span data-stu-id="3707c-438">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-439">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-439">Resource</span></span>
* <span data-ttu-id="3707c-440">Se ha agregado el comando `az rest` para hacer llamadas de REST.</span><span class="sxs-lookup"><span data-stu-id="3707c-440">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="3707c-441">Se ha corregido el error al usar `policy assignment list` con un grupo de recursos o un nivel de suscripción `--scope`.</span><span class="sxs-lookup"><span data-stu-id="3707c-441">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="3707c-442">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="3707c-442">ServiceBus</span></span>
* <span data-ttu-id="3707c-443">Se ha corregido el error con `servicebus topic create --max-size` [n.º 9319](https://github.com/azure/azure-cli/issues/9319)</span><span class="sxs-lookup"><span data-stu-id="3707c-443">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-444">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-444">SQL</span></span>
* <span data-ttu-id="3707c-445">Se ha cambiado `--location` para que sea opcionalpara `sql [server|mi] create`; usa la ubicación del grupo de recursos si no se especifica.</span><span class="sxs-lookup"><span data-stu-id="3707c-445">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="3707c-446">Se ha corregido el error "No se puede iterar en el objeto NoneType" para `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="3707c-446">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="3707c-447">SQLVm</span><span class="sxs-lookup"><span data-stu-id="3707c-447">SQLVm</span></span>
* <span data-ttu-id="3707c-448">[CAMBIO IMPORTANTE] Se ha cambiado `sql vm create` para requerir el parámetro `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="3707c-448">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="3707c-449">Se ha cambiado para poder establecer el SKU de la imagen de SQL al crear o actualizar una máquina virtual de SQL.</span><span class="sxs-lookup"><span data-stu-id="3707c-449">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-450">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-450">Storage</span></span>
* <span data-ttu-id="3707c-451">Se ha corregido un problema con una clave de cuenta que falta para `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="3707c-451">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="3707c-452">Se ha corregido un problema con `storage blob sync` en Linux.</span><span class="sxs-lookup"><span data-stu-id="3707c-452">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-453">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-453">VM</span></span>
* <span data-ttu-id="3707c-454">[VERSIÓN PRELIMINAR] Se han agregado los comandos `vm image template` para compilar imágenes de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="3707c-454">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="3707c-455">4 de junio de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-455">June 4, 2019</span></span>

<span data-ttu-id="3707c-456">Versión 2.0.66</span><span class="sxs-lookup"><span data-stu-id="3707c-456">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="3707c-457">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-457">Core</span></span>
* <span data-ttu-id="3707c-458">Se ha corregido el problema por el que los comandos generan un error si `--output yaml` se usa con `--query`.</span><span class="sxs-lookup"><span data-stu-id="3707c-458">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-459">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-459">ACR</span></span>
* <span data-ttu-id="3707c-460">Se ha agregado el grupo de comandos "acr pack" para crear tareas de compilación rápida mediante Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="3707c-460">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-461">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-461">ACS</span></span>
* <span data-ttu-id="3707c-462">Se permite habilitar o deshabilitar el complemento kube-dashboard de AKS.</span><span class="sxs-lookup"><span data-stu-id="3707c-462">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="3707c-463">Se imprime un mensaje descriptivo cuando la suscripción no está en la lista de permitidos para usar Azure Red Hat OpenShift.</span><span class="sxs-lookup"><span data-stu-id="3707c-463">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-464">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-464">Batch</span></span>
* <span data-ttu-id="3707c-465">Se ha mejorado el control de errores cuando no se ha iniciado sesión en una cuenta \[ [9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="3707c-465">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-466">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-466">IoT</span></span>
* <span data-ttu-id="3707c-467">Se ha agregado compatibilidad para la conmutación por error manual.</span><span class="sxs-lookup"><span data-stu-id="3707c-467">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="3707c-468">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-468">Network</span></span>
* <span data-ttu-id="3707c-469">Se han agregado comandos `network application-gateway waf-policy` para admitir reglas personalizadas de WAF.</span><span class="sxs-lookup"><span data-stu-id="3707c-469">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="3707c-470">Se agregaron los argumentos `--waf-policy` y `--max-capacity` a `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-470">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="3707c-471">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-471">Resource</span></span>
* <span data-ttu-id="3707c-472">Se ha mejorado el mensaje de error de `deployment create` cuando TTY no está disponible.</span><span class="sxs-lookup"><span data-stu-id="3707c-472">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="3707c-473">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-473">Role</span></span>
* <span data-ttu-id="3707c-474">Texto de ayuda actualizado.</span><span class="sxs-lookup"><span data-stu-id="3707c-474">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="3707c-475">Proceso</span><span class="sxs-lookup"><span data-stu-id="3707c-475">Compute</span></span>
* <span data-ttu-id="3707c-476">Se ha agregado compatibilidad a `vm create` para máquinas virtuales desde una imagen administrada con LUN de discos de datos que no comienzan en 0 o que omiten los números.</span><span class="sxs-lookup"><span data-stu-id="3707c-476">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="3707c-477">21 de mayo de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-477">May 21, 2019</span></span>

<span data-ttu-id="3707c-478">Versión 2.0.65</span><span class="sxs-lookup"><span data-stu-id="3707c-478">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="3707c-479">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-479">Core</span></span>
* <span data-ttu-id="3707c-480">Se han agregado mejores comentarios para los errores de autenticación.</span><span class="sxs-lookup"><span data-stu-id="3707c-480">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="3707c-481">Se ha corregido un problema por el que la CLI cargaba extensiones que no eran compatibles con su versión principal.</span><span class="sxs-lookup"><span data-stu-id="3707c-481">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="3707c-482">Se ha corregido un problema con el inicio cuando `clouds.config` estaba dañado.</span><span class="sxs-lookup"><span data-stu-id="3707c-482">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-483">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-483">ACR</span></span>
* <span data-ttu-id="3707c-484">Se ha agregado compatibilidad para identidades administradas a Tareas.</span><span class="sxs-lookup"><span data-stu-id="3707c-484">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-485">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-485">ACS</span></span>
* <span data-ttu-id="3707c-486">Se ha corregido el comando `openshift create` cuando se usa con el cliente AAD.</span><span class="sxs-lookup"><span data-stu-id="3707c-486">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-487">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-487">AppService</span></span>
* <span data-ttu-id="3707c-488">[EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`; se quitará en la próxima versión.</span><span class="sxs-lookup"><span data-stu-id="3707c-488">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="3707c-489">Se ha cambiado `functionapp devops-pipeline` para recopilar el registro de compilación de Azure DevOps en modo detallado.</span><span class="sxs-lookup"><span data-stu-id="3707c-489">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="3707c-490">[CAMBIO IMPORTANTE] Se ha eliminado la marca `--use_local_settings` del comando `functionapp devops-pipeline`; no era operativa.</span><span class="sxs-lookup"><span data-stu-id="3707c-490">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="3707c-491">Se ha cambiado `webapp up` para que devuelva la salida JSON si no se usa `--logs`.</span><span class="sxs-lookup"><span data-stu-id="3707c-491">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="3707c-492">Se ha agregado compatibilidad para escribir los recursos predeterminados en la configuración local para `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="3707c-492">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="3707c-493">Se ha agregado compatibilidad para `webapp up` para volver a implementar una aplicación sin usar el argumento `--location`.</span><span class="sxs-lookup"><span data-stu-id="3707c-493">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="3707c-494">Se ha corregido un problema por el que, al crear un ASP en la SKU gratuita de Linux, el valor de SKU "Fee" no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="3707c-494">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-495">BotService</span><span class="sxs-lookup"><span data-stu-id="3707c-495">BotService</span></span>
* <span data-ttu-id="3707c-496">Se ha cambiado para permitir las mayúsculas y minúsculas para los parámetros `--lang` de los comandos.</span><span class="sxs-lookup"><span data-stu-id="3707c-496">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="3707c-497">Se ha actualizado la descripción para el módulo de comandos.</span><span class="sxs-lookup"><span data-stu-id="3707c-497">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="3707c-498">Consumo</span><span class="sxs-lookup"><span data-stu-id="3707c-498">Consumption</span></span>
* <span data-ttu-id="3707c-499">Se ha agregado un parámetro obligatorio que faltaba al ejecutar `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="3707c-499">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-500">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-500">IoT</span></span>
* <span data-ttu-id="3707c-501">Se ha agregado compatibilidad para enumerar todas las claves.</span><span class="sxs-lookup"><span data-stu-id="3707c-501">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="3707c-502">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-502">Network</span></span>
* [CAMBIO IMPORTANTE]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="3707c-504">Se ha agregado el argumento `--nat-gateway` a `network vnet subnet [create|update]` para adjuntar a una puerta de enlace NAT.</span><span class="sxs-lookup"><span data-stu-id="3707c-504">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="3707c-505">Se ha corregido el problema con `dns zone import` por el que los nombres de registro no encontraban un tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="3707c-505">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-506">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-506">RDBMS</span></span>
* <span data-ttu-id="3707c-507">Se ha agregado compatibilidad con replicación geográfica a mysql y postgres.</span><span class="sxs-lookup"><span data-stu-id="3707c-507">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="3707c-508">RBAC</span><span class="sxs-lookup"><span data-stu-id="3707c-508">RBAC</span></span>
* <span data-ttu-id="3707c-509">Se ha agregado compatibilidad para ámbitos de grupos de administración a `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="3707c-509">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-510">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-510">Storage</span></span>
* <span data-ttu-id="3707c-511">`storage blob sync`: se ha agregado el comando sync a Blob Storage.</span><span class="sxs-lookup"><span data-stu-id="3707c-511">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="3707c-512">Proceso</span><span class="sxs-lookup"><span data-stu-id="3707c-512">Compute</span></span>
* <span data-ttu-id="3707c-513">Se ha agregado `--computer-name` a `vm create` para establecer el nombre de equipo de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="3707c-513">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="3707c-514">Se ha cambiado el nombre de `--ssh-key-value` a `--ssh-key-values` para `[vm|vmss] create`; ahora pueden aceptar varios valores ssh de clave pública o rutas de acceso.</span><span class="sxs-lookup"><span data-stu-id="3707c-514">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="3707c-515">__Nota__: Este **no** es un cambio importante. `--ssh-key-value` se analizará correctamente porque solo coincide con `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="3707c-515">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="3707c-516">Se ha cambiado el argumento `--type` de `ppg create` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="3707c-516">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="3707c-517">6 de mayo de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-517">May 6, 2019</span></span>

<span data-ttu-id="3707c-518">Versión 2.0.64</span><span class="sxs-lookup"><span data-stu-id="3707c-518">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-519">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-519">ACS</span></span>
* <span data-ttu-id="3707c-520">[CAMBIO IMPORTANTE] Se ha eliminado la marca `--fqdn` de los comandos `openshift`.</span><span class="sxs-lookup"><span data-stu-id="3707c-520">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="3707c-521">Se ha cambiado para usar la versión GA de la API Openshift de Azure Red Hat.</span><span class="sxs-lookup"><span data-stu-id="3707c-521">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="3707c-522">Se ha agregado la marca `customer-admin-group-id` a `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-522">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="3707c-523">[GA] Se ha quitado `(PREVIEW)` de la opción `--network-policy` de `aks create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-523">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-524">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-524">Appservice</span></span>
* <span data-ttu-id="3707c-525">[EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="3707c-525">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="3707c-526">Se ha cambiado el nombre a `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="3707c-526">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="3707c-527">Se ha corregido un error por el que no se podía obtener el nombre de usuario correcto para cloudshell, lo que provocaba un error de `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="3707c-527">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="3707c-528">Se ha actualziado la documentación de `appservice plan --sku` para incluir la compatibilidad con appserviceplans.</span><span class="sxs-lookup"><span data-stu-id="3707c-528">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="3707c-529">Se han agregado argumentos opcionales para el grupo de recursos y el plan a `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="3707c-529">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="3707c-530">Se ha agregado compatibilidad a `webapp ssh` para respetar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="3707c-530">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="3707c-531">Se ha agregado compatibilidad a `appserviceplan create` con la SKU gratuita de Linux.</span><span class="sxs-lookup"><span data-stu-id="3707c-531">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="3707c-532">Se ha cambiado `webapp up` para que haya una suspensión de 30 segundos después de configurar la opción `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para controlar el inicio en frío de kudu.</span><span class="sxs-lookup"><span data-stu-id="3707c-532">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="3707c-533">Se ha agregado compatibilidad con el entorno de ejecución `powershell` a `functionapp create` en Windows.</span><span class="sxs-lookup"><span data-stu-id="3707c-533">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="3707c-534">Se agregó el comando `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="3707c-534">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-535">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-535">Batch</span></span>
* <span data-ttu-id="3707c-536">Se ha corregido un error en el validador para las opciones de `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="3707c-536">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-537">Botservice</span><span class="sxs-lookup"><span data-stu-id="3707c-537">Botservice</span></span>
* <span data-ttu-id="3707c-538">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para crear un bot de Web App vacío de forma predeterminada (es decir, el bot no se implementa en App Service).</span><span class="sxs-lookup"><span data-stu-id="3707c-538">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="3707c-539">Se ha agregado la marca `--echo` a `bot create` para usar el comportamiento anterior con `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="3707c-539">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="3707c-540">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--version` a `v4`.</span><span class="sxs-lookup"><span data-stu-id="3707c-540">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="3707c-541">__NOTA:__ `bot prepare-publish` sigue usando el valor predeterminado anterior.</span><span class="sxs-lookup"><span data-stu-id="3707c-541">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="3707c-542">[CAMBIO IMPORTANTE] Se ha cambiado `--lang` para que su valor predeterminado ya no sea `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="3707c-542">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="3707c-543">Si el comando requiere `--lang` y no se proporciona, ahora producirá un error.</span><span class="sxs-lookup"><span data-stu-id="3707c-543">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="3707c-544">[CAMBIO IMPORTANTE] Se han cambiado los argumentos `--appid` y `--password` de `bot create` para que sean necesarios y ahora se pueden crear mediante `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-544">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="3707c-545">Se ha agregado la validación de `--appid` y `--password`.</span><span class="sxs-lookup"><span data-stu-id="3707c-545">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="3707c-546">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4` para que no cree ni use una cuenta de almacenamiento ni Application Insights.</span><span class="sxs-lookup"><span data-stu-id="3707c-546">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="3707c-547">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v3` para que requiera una región donde esté disponible Application Insights.</span><span class="sxs-lookup"><span data-stu-id="3707c-547">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="3707c-548">[CAMBIO IMPORTANTE] Se ha cambiado `bot update` para que ahora afecte solo a determinadas propiedades de un bot.</span><span class="sxs-lookup"><span data-stu-id="3707c-548">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="3707c-549">[CAMBIO IMPORTANTE] Se han cambiado las marcas `--lang` para que acepten `Javascript` en lugar de `Node`.</span><span class="sxs-lookup"><span data-stu-id="3707c-549">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="3707c-550">[CAMBIO IMPORTANTE] Se ha quitado `Node` como valor de `--lang` permitido.</span><span class="sxs-lookup"><span data-stu-id="3707c-550">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="3707c-551">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para que no establezca `SCM_DO_BUILD_DURING_DEPLOYMENT` en true.</span><span class="sxs-lookup"><span data-stu-id="3707c-551">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="3707c-552">Todas las implementaciones a través de Kudu actuarán según su comportamiento predeterminado.</span><span class="sxs-lookup"><span data-stu-id="3707c-552">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="3707c-553">Se ha cambiado `bot download` para los bots sin archivos `.bot` para crear el archivo de configuración específico del idioma con los valores de Application Insights para el bot.</span><span class="sxs-lookup"><span data-stu-id="3707c-553">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="3707c-554">Se ha agregado compatibilidad de `Typescript` con `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="3707c-554">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="3707c-555">Se ha agregado un mensaje de advertencia a `bot prepare-deploy` para los bots `Javascript` y `Typescript` cuando `--code-dir` no contiene `package.json`.</span><span class="sxs-lookup"><span data-stu-id="3707c-555">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="3707c-556">Se ha cambiado `bot prepare-deploy` para que devuelva `true` si es correcto.</span><span class="sxs-lookup"><span data-stu-id="3707c-556">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="3707c-557">Se ha agregado el registro detallado a `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="3707c-557">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="3707c-558">Se han agregado regiones más disponibles de Application Insights a `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="3707c-558">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="3707c-559">Configuración</span><span class="sxs-lookup"><span data-stu-id="3707c-559">Configure</span></span>
* <span data-ttu-id="3707c-560">Se ha agregado compatibilidad para configuraciones de valores predeterminados de argumentos basadas en carpetas.</span><span class="sxs-lookup"><span data-stu-id="3707c-560">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="3707c-561">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="3707c-561">Eventhubs</span></span>
* <span data-ttu-id="3707c-562">Se agregaron los comandos `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-562">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="3707c-563">Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-563">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-564">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-564">Network</span></span>
* <span data-ttu-id="3707c-565">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--cache` con `--defer` para `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-565">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="3707c-566">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="3707c-566">Policy Insights</span></span>
* <span data-ttu-id="3707c-567">Se ha agregado compatibilidad a `--expand PolicyEvaluationDetails` para consultar detalles de evaluación de directivas en el recurso.</span><span class="sxs-lookup"><span data-stu-id="3707c-567">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="3707c-568">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-568">Role</span></span>
* <span data-ttu-id="3707c-569">[EN DESUSO] Se ha cambiado el argumento `create-for-rbac` hide '--password' y se dejará de dar soporte en mayo de 2019.</span><span class="sxs-lookup"><span data-stu-id="3707c-569">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="3707c-570">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="3707c-570">Service Bus</span></span>
* <span data-ttu-id="3707c-571">Se agregaron los comandos `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-571">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="3707c-572">Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-572">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="3707c-573">Se ha corregido `topic [create|update]` para que `--max-size` permita valores de 10, 20, 40 y 80 GB con SKU Premium.</span><span class="sxs-lookup"><span data-stu-id="3707c-573">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-574">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-574">SQL</span></span>
* <span data-ttu-id="3707c-575">Se agregaron los comandos `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-575">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-576">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-576">VM</span></span>
* <span data-ttu-id="3707c-577">Se ha agregado `--protect-from-scale-in` y `--protect-from-scale-set-actions` a `vmss update` para habilitar las actualizaciones a la directiva de protección de instancias de máquina virtual de VMSS.</span><span class="sxs-lookup"><span data-stu-id="3707c-577">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="3707c-578">Se ha agregado `--instance-id` a `vmss update` para habilitar la actualización genérica de instancias de máquina virtual de VMSS.</span><span class="sxs-lookup"><span data-stu-id="3707c-578">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="3707c-579">Se ha agregado `--instance-id` a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="3707c-579">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="3707c-580">Se ha agregado un nuevo grupo de comandos `ppg` para administrar grupos de ubicación de proximidad.</span><span class="sxs-lookup"><span data-stu-id="3707c-580">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="3707c-581">Se ha agregado `--ppg` a `[vm|vmss] create` y `vm availability-set create` para administrar grupos de ubicación de proximidad.</span><span class="sxs-lookup"><span data-stu-id="3707c-581">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="3707c-582">Se ha agregado el parámetro `--hyper-v-generation` a `image create`</span><span class="sxs-lookup"><span data-stu-id="3707c-582">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="3707c-583">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-583">April 23, 2019</span></span>

<span data-ttu-id="3707c-584">Versión 2.0.63</span><span class="sxs-lookup"><span data-stu-id="3707c-584">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-585">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-585">ACS</span></span>
* <span data-ttu-id="3707c-586">Se ha cambiado `aks get-credentials` para que pregunte si se desean sobrescribir los valores duplicados.</span><span class="sxs-lookup"><span data-stu-id="3707c-586">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="3707c-587">Se ha quitado `(PREVIEW)` de los comandos de DevSpaces "aks use-dev-spaces" y "aks remove-dev-spaces".</span><span class="sxs-lookup"><span data-stu-id="3707c-587">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-588">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-588">AMS</span></span>
* <span data-ttu-id="3707c-589">Se ha corregido un error con la actualización de los filtros de cuenta y recursos.</span><span class="sxs-lookup"><span data-stu-id="3707c-589">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-590">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-590">AppService</span></span>
* <span data-ttu-id="3707c-591">Se ha agregado compatibilidad para ASE y un tiempo de espera a `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="3707c-591">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="3707c-592">Se ha agregado compatibilidad para establecer la integración e implementación continuas a una canalización de Azure DevOps desde un repositorio de Github para aplicaciones de función.</span><span class="sxs-lookup"><span data-stu-id="3707c-592">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="3707c-593">Se ha agregado el argumento `--github-pat` a `functionapp devops-build create` para aceptar el token de acceso personal de Github.</span><span class="sxs-lookup"><span data-stu-id="3707c-593">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="3707c-594">Se ha agregado el argumento `--github-repository` a `functionapp devops-build create` para aceptar el repositorio de Github que contiene un código de origen de aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="3707c-594">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="3707c-595">Se ha corregido el problema por el que `az webapp up --logs` producía un error y actualizaba .NETCORE a la versión 2.1 de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3707c-595">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="3707c-596">Se han quitado las opciones de configuración de aplicaciones de función innecesarias a la hora de crear una aplicación de función con un plan de consumo.</span><span class="sxs-lookup"><span data-stu-id="3707c-596">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="3707c-597">Se ha cambiado `webapp up` para que la cadena asp predeterminada ahora anexe el número al final para crear un nuevo ASP según las opciones de SKU.</span><span class="sxs-lookup"><span data-stu-id="3707c-597">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="3707c-598">Se ha agregado `-b` como opción a `webapp up` para iniciar la aplicación en el explorador.</span><span class="sxs-lookup"><span data-stu-id="3707c-598">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="3707c-599">Se ha cambiado `webapp deployment source config zip` para controlar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="3707c-599">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="3707c-600">Administrador de implementaciones</span><span class="sxs-lookup"><span data-stu-id="3707c-600">Deployment Manager</span></span>
* <span data-ttu-id="3707c-601">[VERSIÓN PRELIMINAR] Creación y administración de artefactos que admiten lanzamientos.</span><span class="sxs-lookup"><span data-stu-id="3707c-601">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="3707c-602">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-602">Lab</span></span>
* <span data-ttu-id="3707c-603">Se ha corregido el error que provocaba una salida prematura.</span><span class="sxs-lookup"><span data-stu-id="3707c-603">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="3707c-604">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-604">Network</span></span>
* <span data-ttu-id="3707c-605">Se ha agregado la delegación de servidor nombre automática a `dns zone create` en la zona primaria durante la creación de una zona secundaria.</span><span class="sxs-lookup"><span data-stu-id="3707c-605">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-606">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-606">Resource</span></span>
* <span data-ttu-id="3707c-607">[EN DESUSO] Se han dejado de usar los argumentos `--link-id`, `--target-id` y `--filter-string` de `resource link`.</span><span class="sxs-lookup"><span data-stu-id="3707c-607">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="3707c-608">En su lugar, use los argumentos `--link`, `--target` y `--filter`.</span><span class="sxs-lookup"><span data-stu-id="3707c-608">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="3707c-609">Se ha corregido el problema por el que los comandos `resource link [create|update]` no funcionaban.</span><span class="sxs-lookup"><span data-stu-id="3707c-609">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="3707c-610">Se ha corregido un problema por el que se podía producir un problema al eliminar utilizando un identificador de recurso.</span><span class="sxs-lookup"><span data-stu-id="3707c-610">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-611">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-611">SQL</span></span>
* <span data-ttu-id="3707c-612">Se ha agregado compatibilidad para zonas horarias personalizadas en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="3707c-612">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="3707c-613">Se ha cambiado para poder usar un nombre de grupo elástico con `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-613">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="3707c-614">Se ha agregado compatibilidad de `--no-wait` con `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-614">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="3707c-615">Se ha agregado el comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="3707c-615">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-616">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-616">Storage</span></span>
* <span data-ttu-id="3707c-617">Se ha corregido un problema con los tokens de SAS de codificación doble en `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="3707c-617">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-618">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-618">VM</span></span>
* <span data-ttu-id="3707c-619">Se ha agregado la marca `--skip-shutdown` a `vm|vmss stop` para apagar las máquinas virtuales sin cerrarlas.</span><span class="sxs-lookup"><span data-stu-id="3707c-619">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="3707c-620">Se ha agregado el argumento `--storage-account-type` a `sig image-version create` para establecer el tipo de cuenta del perfil de publicación.</span><span class="sxs-lookup"><span data-stu-id="3707c-620">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="3707c-621">Se ha agregado el argumento `--target-regions` a `sig image-version create` para permitir tipos de cuenta de almacenamiento específicos de la región.</span><span class="sxs-lookup"><span data-stu-id="3707c-621">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="3707c-622">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-622">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="3707c-623">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-623">Core</span></span>
* <span data-ttu-id="3707c-624">Se ha corregido el problema por el que algunas extensiones mostraban una versión `Unknown` y no se podían actualizar.</span><span class="sxs-lookup"><span data-stu-id="3707c-624">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-625">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-625">ACR</span></span>
* <span data-ttu-id="3707c-626">Se ha agregado compatibilidad con la ejecución de una imagen sin contexto.</span><span class="sxs-lookup"><span data-stu-id="3707c-626">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-627">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-627">AMS</span></span>
* [EN DESUSO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CAMBIO IMPORTANTE]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="3707c-630">Se ha agregado compatibilidad con nuevos parámetros de cifrado a `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-630">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="3707c-631">Se ha agregado un nuevo parámetro `--filters` a `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-631">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-632">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-632">AppService</span></span>
* <span data-ttu-id="3707c-633">Se ha agregado compatibilidad de `--logs` con `webapp up`</span><span class="sxs-lookup"><span data-stu-id="3707c-633">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="3707c-634">En el comando `functionapp devops-build create`, se han corregido los problemas de generación de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="3707c-634">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="3707c-635">Se ha mejorado el control de errores y los indicadores de `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="3707c-635">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="3707c-636">[CAMBIO IMPORTANTE] Se ha quitado la marca `--local-git` del comando `devops-build`; la detección y administración del repositorio git local son obligatorias para crear canalizaciones de Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="3707c-636">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="3707c-637">Se ha agregado compatibilidad para crear planes de funciones Linux</span><span class="sxs-lookup"><span data-stu-id="3707c-637">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="3707c-638">Se ha agregado la posibilidad de cambiar el plan de una aplicación de función mediante `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="3707c-638">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="3707c-639">Se ha agregado compatibilidad para las opciones de escalado horizontal del plan Premium de Azure Functions</span><span class="sxs-lookup"><span data-stu-id="3707c-639">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="3707c-640">CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-640">CDN</span></span>
* <span data-ttu-id="3707c-641">Se ha agregado compatibilidad para `Microsoft_Standard` y `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="3707c-641">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="3707c-642">Comentarios</span><span class="sxs-lookup"><span data-stu-id="3707c-642">Feedback</span></span>
* <span data-ttu-id="3707c-643">Se ha cambiado `feedback` para mostrar los metadatos de los comandos ejecutados recientemente</span><span class="sxs-lookup"><span data-stu-id="3707c-643">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="3707c-644">Se ha cambiado `feedback` para pedir al usuario que abra un explorador y use una plantilla de incidencia para ayudar en el proceso de creación de la incidencia</span><span class="sxs-lookup"><span data-stu-id="3707c-644">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="3707c-645">Se ha cambiado `feedback` para imprimir el cuerpo de la incidencia cuando se ejecuta con "--verbose"</span><span class="sxs-lookup"><span data-stu-id="3707c-645">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-646">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-646">Monitor</span></span>
* <span data-ttu-id="3707c-647">Se ha corregido un problema por "count" no era un valor permitido en `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-647">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="3707c-648">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-648">Network</span></span>
* <span data-ttu-id="3707c-649">Se ha corregido el formato de tabla que no se mostraba con `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="3707c-649">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="3707c-650">Se han agregado los comandos `list-request-headers` y `list-response-headers` a `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-650">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="3707c-651">Se ha agregado el comando `list-server-variables` a `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="3707c-651">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="3707c-652">Se ha corregido un problema por el que actualización del estado de un vínculo en un puerto de express-route generaba una excepción de atributo desconocido `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-652">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="3707c-653">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="3707c-653">PrivateDNS</span></span>
* <span data-ttu-id="3707c-654">Se ha agregado `network private-dns` para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="3707c-654">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-655">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-655">Resource</span></span>
* <span data-ttu-id="3707c-656">Se ha corregido el problema con `deployment create` y `group deployment create` por el que no funcionaba un archivo de parámetros con un conjunto de parámetros vacío</span><span class="sxs-lookup"><span data-stu-id="3707c-656">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="3707c-657">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-657">Role</span></span>
* <span data-ttu-id="3707c-658">Se ha corregido `create-for-rbac` para que trate `--years` correctamente</span><span class="sxs-lookup"><span data-stu-id="3707c-658">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="3707c-659">[CAMBIO IMPORTANTE] Se ha cambiado `role assignment delete` para preguntar cuando se eliminan todas las asignaciones de la suscripción de forma incondicional</span><span class="sxs-lookup"><span data-stu-id="3707c-659">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-660">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-660">SQL</span></span>
* <span data-ttu-id="3707c-661">Se ha actualizado `sql mi [create|update]` con las propiedades proxyOverride y publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="3707c-661">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-662">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-662">Storage</span></span>
* <span data-ttu-id="3707c-663">[CAMBIO IMPORTANTE] Se ha quitado el resultado de `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="3707c-663">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="3707c-664">Se ha agregado `--full-uri` a `storage blob generate-sas` para crear el URI completo para el blob con SAS</span><span class="sxs-lookup"><span data-stu-id="3707c-664">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="3707c-665">Se ha agregado `--file-snapshot` a `storage file copy start` para copiar el archivo desde la instantánea</span><span class="sxs-lookup"><span data-stu-id="3707c-665">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="3707c-666">Se ha cambiado `storage blob copy cancel` para mostrar solo el error en lugar de la excepción para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="3707c-666">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="3707c-667">26 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-667">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="3707c-668">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-668">Core</span></span>
* <span data-ttu-id="3707c-669">Se han corregido problemas con la incompatibilidad de la extensión de desarrollo.</span><span class="sxs-lookup"><span data-stu-id="3707c-669">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="3707c-670">El control de errores ahora dirige a los clientes a la página de problemas.</span><span class="sxs-lookup"><span data-stu-id="3707c-670">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="3707c-671">Nube</span><span class="sxs-lookup"><span data-stu-id="3707c-671">Cloud</span></span>
* <span data-ttu-id="3707c-672">Se ha corregido un error de "suscripción no encontrada" en `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="3707c-672">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-673">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-673">ACR</span></span>
* <span data-ttu-id="3707c-674">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="3707c-674">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="3707c-675">Se ha agregado `--auth-mode` a los comandos `acr build`, `acr run`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-675">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="3707c-676">Se ha agregado el grupo de comandos "acr task credential" para administrar las credenciales de una tarea.</span><span class="sxs-lookup"><span data-stu-id="3707c-676">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="3707c-677">Se ha agregado "--no-wait" al comando `acr build`.</span><span class="sxs-lookup"><span data-stu-id="3707c-677">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-678">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-678">AppService</span></span>
* <span data-ttu-id="3707c-679">Se ha corregido el error por el que `webapp up` no controlaba correctamente los escenarios de ejecución desde un directorio o de código desconocido.</span><span class="sxs-lookup"><span data-stu-id="3707c-679">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="3707c-680">Se ha corregido el error por el que los espacios no funcionaban para `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="3707c-680">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="3707c-681">Servicio BOT</span><span class="sxs-lookup"><span data-stu-id="3707c-681">BOT Service</span></span>
* <span data-ttu-id="3707c-682">Se ha agregado `bot prepare-deploy` para preparar la implementación de bots mediante `webapp`.</span><span class="sxs-lookup"><span data-stu-id="3707c-682">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="3707c-683">Se ha cambiado `bot create --kind registration` para que muestre la contraseña si no se proporciona una.</span><span class="sxs-lookup"><span data-stu-id="3707c-683">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="3707c-684">[CAMBIO IMPORTANTE] Se ha cambiado `--endpoint` en `bot create --kind registration` a que sea una cadena vacía de forma predeterminada en lugar de que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="3707c-684">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="3707c-685">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="3707c-685">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="3707c-686">CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-686">CDN</span></span>
* <span data-ttu-id="3707c-687">Se agregó compatibilidad para `--no-wait` a `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-687">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="3707c-688">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento de almacenamiento de cadenas de consulta en caché predeterminado de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-688">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="3707c-689">El valor predeterminado ya no es "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="3707c-689">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="3707c-690">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="3707c-690">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-691">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="3707c-691">Cosmosdb</span></span>
* <span data-ttu-id="3707c-692">Se ha agregado compatibilidad con `--enable-multiple-write-locations` al actualizar la cuenta.</span><span class="sxs-lookup"><span data-stu-id="3707c-692">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="3707c-693">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="3707c-693">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-694">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-694">Interactive</span></span>
* <span data-ttu-id="3707c-695">Se ha corregido la incompatibilidad con la extensión interactiva instalada mediante azdev.</span><span class="sxs-lookup"><span data-stu-id="3707c-695">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-696">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-696">Monitor</span></span>
* <span data-ttu-id="3707c-697">Se ha cambiado para permitir el valor de dimensión `*` para `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-697">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-698">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-698">Network</span></span>
* <span data-ttu-id="3707c-699">Se ha agregado el grupo de comandos `rewrite-rule` a `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="3707c-699">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-700">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-700">Profile</span></span>
* <span data-ttu-id="3707c-701">Se ha agregado a `login` compatibilidad de la cuenta en el nivel de inquilino para la identidad de servicio administrada.</span><span class="sxs-lookup"><span data-stu-id="3707c-701">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="3707c-702">Postgres</span><span class="sxs-lookup"><span data-stu-id="3707c-702">Postgres</span></span> 
* <span data-ttu-id="3707c-703">Se han agregado los comandos postgresql `replica` y el comando `restart server`.</span><span class="sxs-lookup"><span data-stu-id="3707c-703">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="3707c-704">Se ha cambiado para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="3707c-704">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-705">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-705">Resource</span></span>
* <span data-ttu-id="3707c-706">Se ha mejorado la salida de tabla de `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-706">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="3707c-707">Se ha corregido el problema con `deployment [create|validate]` por el que no reconocía el tipo secureObject.</span><span class="sxs-lookup"><span data-stu-id="3707c-707">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="3707c-708">Grafo</span><span class="sxs-lookup"><span data-stu-id="3707c-708">Graph</span></span>
* <span data-ttu-id="3707c-709">Se agregó compatibilidad para `--end-date` a `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="3707c-709">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="3707c-710">Se ha agregado compatibilidad para agregar permisos con `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="3707c-710">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="3707c-711">Se ha corregido un error con `ad app permission list` cuando no había ningún permiso.</span><span class="sxs-lookup"><span data-stu-id="3707c-711">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="3707c-712">Se ha cambiado `ad sp delete` para omitir la eliminación de la asignación de roles si la cuenta actual no tiene ninguna suscripción.</span><span class="sxs-lookup"><span data-stu-id="3707c-712">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="3707c-713">Se ha cambiado `ad app create` para que `--identifier-uris` sea una lista vacía de forma predeterminada si no se proporciona.</span><span class="sxs-lookup"><span data-stu-id="3707c-713">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-714">storage</span><span class="sxs-lookup"><span data-stu-id="3707c-714">storage</span></span>
* <span data-ttu-id="3707c-715">Se ha agregado `--snapshot` a `storage file download-batch` para descargar desde una instantánea de recurso compartido.</span><span class="sxs-lookup"><span data-stu-id="3707c-715">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="3707c-716">Se ha cambiado la barra de progreso `storage blob [download-batch|upload-batch]` para que sea menos detallada y que indique el blob actual.</span><span class="sxs-lookup"><span data-stu-id="3707c-716">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="3707c-717">Se ha corregido el problema con `storage account update` al actualizar los parámetros de cifrado.</span><span class="sxs-lookup"><span data-stu-id="3707c-717">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="3707c-718">Se ha corregido el problema por el que `storage blob show` producía un error al usar oauth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="3707c-718">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-719">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-719">VM</span></span>
* <span data-ttu-id="3707c-720">Se agregó el comando `image update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-720">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="3707c-721">12 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-721">March 12, 2019</span></span>

<span data-ttu-id="3707c-722">Versión 2.0.60</span><span class="sxs-lookup"><span data-stu-id="3707c-722">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="3707c-723">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-723">Core</span></span>

* <span data-ttu-id="3707c-724">Se ha corregido un error incorrecto en `cloud set` sobre la suscripción no encontrada.</span><span class="sxs-lookup"><span data-stu-id="3707c-724">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-725">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-725">ACR</span></span>

* <span data-ttu-id="3707c-726">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="3707c-726">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-727">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-727">ACS</span></span>

* <span data-ttu-id="3707c-728">Ahora, se omite el parámetro `--listen-address` de `aks browse` si kubectl no lo admite</span><span class="sxs-lookup"><span data-stu-id="3707c-728">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="3707c-729">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-729">AppService</span></span>

* <span data-ttu-id="3707c-730">Se ha agregado `[webapp|functionapp] deployment list-publishing-credentials` para obtener la dirección URL y sus credenciales de publicación de Kudu.</span><span class="sxs-lookup"><span data-stu-id="3707c-730">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="3707c-731">Se ha quitado la instrucción de impresión errónea para `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-731">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="3707c-732">Se ha corregido `functionapp` para establecer la imagen correcta en el entorno de ejecución en los planes de App Service de Linux</span><span class="sxs-lookup"><span data-stu-id="3707c-732">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="3707c-733">Se ha quitado la etiqueta de versión preliminar para `webapp up` y se han agregado mejoras al comando.</span><span class="sxs-lookup"><span data-stu-id="3707c-733">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-734">Botservice</span><span class="sxs-lookup"><span data-stu-id="3707c-734">Botservice</span></span>

* <span data-ttu-id="3707c-735">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="3707c-735">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="3707c-736">Se han agregado `Microsoft-BotFramework-AppId` y `Microsoft-BotFramework-AppPassword` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web</span><span class="sxs-lookup"><span data-stu-id="3707c-736">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="3707c-737">Se han quitado las comillas simples de la salida del comando `bot publish` al final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-737">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="3707c-738">Se ha cambiado `bot publish` para que sea asincrónico.</span><span class="sxs-lookup"><span data-stu-id="3707c-738">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="3707c-739">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-739">Container</span></span>

* <span data-ttu-id="3707c-740">Se agregó el argumento `--no-wait` a `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="3707c-740">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="3707c-741">EventHub</span><span class="sxs-lookup"><span data-stu-id="3707c-741">EventHub</span></span>

* <span data-ttu-id="3707c-742">Se ha agregado la marca `--skip-empty-archives` a `eventhub create|update` para admitir archivos vacíos en la captura.</span><span class="sxs-lookup"><span data-stu-id="3707c-742">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="3707c-743">Buscar</span><span class="sxs-lookup"><span data-stu-id="3707c-743">Find</span></span>

* <span data-ttu-id="3707c-744">Actualización de la funcionalidad principal</span><span class="sxs-lookup"><span data-stu-id="3707c-744">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-745">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-745">HDInsight</span></span>

* <span data-ttu-id="3707c-746">Se ha agregado el parámetro `--storage-account-managed-identity` a `hdinsight create` para admitir MSI de ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="3707c-746">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="3707c-747">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-747">Network</span></span>

* <span data-ttu-id="3707c-748">Se ha corregido un problema con `vpn-connection update` por el que no se podía actualizar una conexión VPN entre pasarelas de diferentes suscripciones.</span><span class="sxs-lookup"><span data-stu-id="3707c-748">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-749">Rdbms</span><span class="sxs-lookup"><span data-stu-id="3707c-749">Rdbms</span></span>

* <span data-ttu-id="3707c-750">Correcciones menores para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="3707c-750">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="3707c-751">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-751">Role</span></span>

* <span data-ttu-id="3707c-752">Se ha corregido `role definition update` para usar el identificador para resolver la definición correctamente.</span><span class="sxs-lookup"><span data-stu-id="3707c-752">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="3707c-753">Se ha cambiado `ad app credential reset` para eliminar la suposición de que la entidad de servicio de la aplicación siempre existe.</span><span class="sxs-lookup"><span data-stu-id="3707c-753">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3707c-754">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3707c-754">Service Fabric</span></span>

* <span data-ttu-id="3707c-755">Se ha corregido un problema con `sf cluster list` que no se podía iterar.</span><span class="sxs-lookup"><span data-stu-id="3707c-755">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="3707c-756">26 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-756">February 26, 2019</span></span>

<span data-ttu-id="3707c-757">Versión 2.0.59</span><span class="sxs-lookup"><span data-stu-id="3707c-757">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="3707c-758">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-758">Core</span></span>

* <span data-ttu-id="3707c-759">Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.</span><span class="sxs-lookup"><span data-stu-id="3707c-759">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-760">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-760">ACR</span></span>

* <span data-ttu-id="3707c-761">Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-761">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="3707c-762">Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.</span><span class="sxs-lookup"><span data-stu-id="3707c-762">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-763">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-763">ACS</span></span>

* <span data-ttu-id="3707c-764">Se agregó la opción `--listen-address` a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="3707c-764">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-765">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-765">AppService</span></span>

* <span data-ttu-id="3707c-766">Se agregó el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="3707c-766">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-767">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-767">Batch</span></span>
* <span data-ttu-id="3707c-768">[CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="3707c-768">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="3707c-769">[CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.</span><span class="sxs-lookup"><span data-stu-id="3707c-769">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="3707c-770">Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="3707c-770">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="3707c-771">[CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`.</span><span class="sxs-lookup"><span data-stu-id="3707c-771">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="3707c-772">Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.</span><span class="sxs-lookup"><span data-stu-id="3707c-772">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="3707c-773">Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.</span><span class="sxs-lookup"><span data-stu-id="3707c-773">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-774">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-774">CosmosDB</span></span>

* <span data-ttu-id="3707c-775">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="3707c-775">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="3707c-776">Kusto</span><span class="sxs-lookup"><span data-stu-id="3707c-776">Kusto</span></span>

* <span data-ttu-id="3707c-777">[CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.</span><span class="sxs-lookup"><span data-stu-id="3707c-777">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="3707c-778">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-778">Network</span></span>

* <span data-ttu-id="3707c-779">Se agregó el argumento `--express-route-gateway-bypass` a `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-779">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="3707c-780">Se han agregado grupos de comandos desde extensiones `express-route`.</span><span class="sxs-lookup"><span data-stu-id="3707c-780">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="3707c-781">Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="3707c-781">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="3707c-782">Se agregó el argumento `--legacy-mode` a `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-782">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="3707c-783">Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-783">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="3707c-784">Se agregó el argumento `--gateway-default-site` a `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-784">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="3707c-785">Se han agregado comandos `ipsec-policy` a `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="3707c-785">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-786">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-786">Resource</span></span>

* <span data-ttu-id="3707c-787">Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="3707c-787">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="3707c-788">Se ha agregado compatibilidad para el archivo de parámetros basado en URI a `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-788">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="3707c-789">Se ha agregado compatibilidad para definiciones y parámetros basados en URI para `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-789">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="3707c-790">Se ha corregido el control de parámetros y reglas para `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-790">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="3707c-791">Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.</span><span class="sxs-lookup"><span data-stu-id="3707c-791">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="3707c-792">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-792">Role</span></span>

* <span data-ttu-id="3707c-793">Se ha agregado compatibilidad con roles de aplicación a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-793">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-794">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-794">VM</span></span>

* <span data-ttu-id="3707c-795">Se ha corregido un problema con `vm create where `--acelerated-networking\` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="3707c-795">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="3707c-796">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-796">February 12, 2019</span></span>

<span data-ttu-id="3707c-797">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="3707c-797">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="3707c-798">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-798">Core</span></span>

* <span data-ttu-id="3707c-799">`az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="3707c-799">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="3707c-800">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="3707c-800">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-801">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-801">ACR</span></span>
* <span data-ttu-id="3707c-802">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="3707c-802">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="3707c-803">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.</span><span class="sxs-lookup"><span data-stu-id="3707c-803">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-804">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-804">ACS</span></span>
* <span data-ttu-id="3707c-805">Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.</span><span class="sxs-lookup"><span data-stu-id="3707c-805">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="3707c-806">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="3707c-806">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="3707c-807">Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="3707c-807">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-808">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-808">AMS</span></span>
* <span data-ttu-id="3707c-809">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-809">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="3707c-810">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-810">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-811">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-811">Appservice</span></span>
* <span data-ttu-id="3707c-812">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="3707c-812">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="3707c-813">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="3707c-813">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="3707c-814">Se ha mejorado la ayuda de `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-814">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="3707c-815">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="3707c-815">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="3707c-816">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="3707c-816">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-817">Botservice</span><span class="sxs-lookup"><span data-stu-id="3707c-817">Botservice</span></span>
* <span data-ttu-id="3707c-818">Se ha mejorado la experiencia de usuario de `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="3707c-818">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="3707c-819">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="3707c-819">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="3707c-820">Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-820">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="3707c-821">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="3707c-821">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="3707c-822">[EN DESUSO] Se ha dejado de utilizar el argumento `--proj-name` en favor de `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="3707c-822">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="3707c-823">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="3707c-823">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="3707c-824">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="3707c-824">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="3707c-825">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="3707c-825">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="3707c-826">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="3707c-826">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="3707c-827">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="3707c-827">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="3707c-828">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3707c-828">Key Vault</span></span>
* <span data-ttu-id="3707c-829">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.</span><span class="sxs-lookup"><span data-stu-id="3707c-829">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-830">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-830">Monitor</span></span>
* <span data-ttu-id="3707c-831">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.</span><span class="sxs-lookup"><span data-stu-id="3707c-831">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-832">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-832">Network</span></span>
* <span data-ttu-id="3707c-833">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="3707c-833">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="3707c-834">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="3707c-834">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="3707c-835">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="3707c-835">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="3707c-836">Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-836">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="3707c-837">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="3707c-837">Policy Insights</span></span>
* <span data-ttu-id="3707c-838">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="3707c-838">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-839">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-839">RDBMS</span></span>
* <span data-ttu-id="3707c-840">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="3707c-840">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="3707c-841">Redis</span><span class="sxs-lookup"><span data-stu-id="3707c-841">Redis</span></span>
* <span data-ttu-id="3707c-842">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="3707c-842">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="3707c-843">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="3707c-843">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="3707c-844">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="3707c-844">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="3707c-845">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="3707c-845">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="3707c-846">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="3707c-846">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="3707c-847">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="3707c-847">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="3707c-848">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="3707c-848">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="3707c-849">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-849">Role</span></span>
* <span data-ttu-id="3707c-850">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="3707c-850">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="3707c-851">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-851">SQL VM</span></span>
* <span data-ttu-id="3707c-852">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="3707c-852">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-853">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-853">VM</span></span>
* <span data-ttu-id="3707c-854">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.</span><span class="sxs-lookup"><span data-stu-id="3707c-854">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="3707c-855">Se agregó `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-855">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="3707c-856">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="3707c-856">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="3707c-857">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="3707c-857">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="3707c-858">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-858">January 31, 2019</span></span>

<span data-ttu-id="3707c-859">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="3707c-859">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="3707c-860">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-860">Core</span></span>

* <span data-ttu-id="3707c-861">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="3707c-861">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="3707c-862">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-862">January 28, 2019</span></span>

<span data-ttu-id="3707c-863">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="3707c-863">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-864">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-864">ACR</span></span>
* <span data-ttu-id="3707c-865">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="3707c-865">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-866">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-866">ACS</span></span>
* <span data-ttu-id="3707c-867">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="3707c-867">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="3707c-868">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="3707c-868">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="3707c-869">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="3707c-869">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-870">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-870">AMS</span></span>
* <span data-ttu-id="3707c-871">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="3707c-871">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="3707c-872">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="3707c-872">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-873">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-873">Appservice</span></span>
* <span data-ttu-id="3707c-874">Se ha agregado compatibilidad para App Insights en `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-874">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="3707c-875">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="3707c-875">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="3707c-876">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="3707c-876">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="3707c-877">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-877">Container</span></span>
* <span data-ttu-id="3707c-878">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="3707c-878">Added `container start` command</span></span>
* <span data-ttu-id="3707c-879">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="3707c-879">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3707c-880">EventGrid</span><span class="sxs-lookup"><span data-stu-id="3707c-880">EventGrid</span></span>
* <span data-ttu-id="3707c-881">Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-881">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="3707c-882">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="3707c-882">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="3707c-883">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="3707c-883">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="3707c-884">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="3707c-884">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="3707c-885">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="3707c-885">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-886">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-886">HDInsight</span></span>
* <span data-ttu-id="3707c-887">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-887">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="3707c-888">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="3707c-888">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="3707c-889">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-889">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="3707c-890">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-890">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="3707c-891">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="3707c-891">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="3707c-892">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-892">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-893">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-893">IoT</span></span>
* <span data-ttu-id="3707c-894">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="3707c-894">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="3707c-895">Kusto</span><span class="sxs-lookup"><span data-stu-id="3707c-895">Kusto</span></span>
* <span data-ttu-id="3707c-896">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-896">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-897">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-897">Monitor</span></span>
* <span data-ttu-id="3707c-898">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="3707c-898">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-899">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-899">Profile</span></span>
* <span data-ttu-id="3707c-900">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.</span><span class="sxs-lookup"><span data-stu-id="3707c-900">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-901">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-901">Network</span></span>
* <span data-ttu-id="3707c-902">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="3707c-902">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="3707c-903">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="3707c-903">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-904">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-904">Resource</span></span>
* <span data-ttu-id="3707c-905">Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-905">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="3707c-906">Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-906">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="3707c-907">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-907">SQL Virtual Machine</span></span>
* <span data-ttu-id="3707c-908">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-908">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-909">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-909">Storage</span></span>
* <span data-ttu-id="3707c-910">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="3707c-910">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="3707c-911">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="3707c-911">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-912">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-912">VM</span></span>
* <span data-ttu-id="3707c-913">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="3707c-913">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="3707c-914">Se ha agregado la marca `--force` a `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="3707c-914">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="3707c-915">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="3707c-915">January 15, 2019</span></span>

<span data-ttu-id="3707c-916">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="3707c-916">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-917">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-917">ACR</span></span>
* <span data-ttu-id="3707c-918">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="3707c-918">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="3707c-919">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="3707c-919">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="3707c-920">[EN DESUSO] Se ha dejado de usar el parámetro `--resource-group` en los comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-920">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="3707c-921">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-921">ACS</span></span>
* <span data-ttu-id="3707c-922">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="3707c-922">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-923">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-923">Appservice</span></span>
* <span data-ttu-id="3707c-924">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="3707c-924">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="3707c-925">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="3707c-925">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="3707c-926">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="3707c-926">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="3707c-927">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="3707c-927">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-928">Botservice</span><span class="sxs-lookup"><span data-stu-id="3707c-928">Botservice</span></span>
* <span data-ttu-id="3707c-929">Se han agregado actualizaciones al estado de implementación a `bot create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-929">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="3707c-930">Configuración</span><span class="sxs-lookup"><span data-stu-id="3707c-930">Configure</span></span>
* <span data-ttu-id="3707c-931">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="3707c-931">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-932">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-932">CosmosDB</span></span>
* <span data-ttu-id="3707c-933">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="3707c-933">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-934">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-934">HDInsight</span></span>
* <span data-ttu-id="3707c-935">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="3707c-935">Added commands for managing applications</span></span>
* <span data-ttu-id="3707c-936">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="3707c-936">Added commands for managing script actions</span></span>
* <span data-ttu-id="3707c-937">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="3707c-937">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="3707c-938">Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="3707c-938">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="3707c-939">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-939">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-940">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-940">Network</span></span>
* <span data-ttu-id="3707c-941">Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-941">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="3707c-942">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="3707c-942">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="3707c-943">Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-943">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="3707c-944">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-944">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="3707c-945">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-945">Role</span></span>
* <span data-ttu-id="3707c-946">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="3707c-946">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="3707c-947">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="3707c-947">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="3707c-948">Seguridad</span><span class="sxs-lookup"><span data-stu-id="3707c-948">Security</span></span>
* <span data-ttu-id="3707c-949">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="3707c-949">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-950">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-950">Storage</span></span>
* <span data-ttu-id="3707c-951">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="3707c-951">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="3707c-952">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="3707c-952">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="3707c-953">Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="3707c-953">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="3707c-954">Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="3707c-954">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="3707c-955">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="3707c-955">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-956">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-956">VM</span></span>
* <span data-ttu-id="3707c-957">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="3707c-957">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="3707c-958">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-958">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="3707c-959">Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="3707c-959">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="3707c-960">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="3707c-960">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="3707c-961">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="3707c-961">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="3707c-962">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="3707c-962">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="3707c-963">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-963">December 20, 2018</span></span>

<span data-ttu-id="3707c-964">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="3707c-964">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="3707c-965">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-965">Appservice</span></span>
* <span data-ttu-id="3707c-966">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="3707c-966">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="3707c-967">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="3707c-967">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="3707c-968">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="3707c-968">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="3707c-969">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="3707c-969">IoTCentral</span></span>
* <span data-ttu-id="3707c-970">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="3707c-970">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="3707c-971">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-971">Role</span></span>
* <span data-ttu-id="3707c-972">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3707c-972">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-973">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-973">SQL</span></span>
* <span data-ttu-id="3707c-974">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="3707c-974">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-975">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-975">VM</span></span>
* <span data-ttu-id="3707c-976">Se ha agregado el parámetro `---os-type` a `disk create`</span><span class="sxs-lookup"><span data-stu-id="3707c-976">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="3707c-977">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-977">December 18, 2018</span></span>

<span data-ttu-id="3707c-978">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="3707c-978">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="3707c-979">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-979">ACR</span></span>
* <span data-ttu-id="3707c-980">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="3707c-980">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="3707c-981">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="3707c-981">Condensed the table layout for task list</span></span>
* <span data-ttu-id="3707c-982">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="3707c-982">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-983">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-983">ACS</span></span>
* <span data-ttu-id="3707c-984">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="3707c-984">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="3707c-985">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-985">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="3707c-986">[EN DESUSO] Se han dejado de usar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="3707c-986">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="3707c-987">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="3707c-987">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="3707c-988">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="3707c-988">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="3707c-989">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="3707c-989">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-990">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-990">Appservice</span></span>
* <span data-ttu-id="3707c-991">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="3707c-991">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="3707c-992">Botservice</span><span class="sxs-lookup"><span data-stu-id="3707c-992">Botservice</span></span>
* <span data-ttu-id="3707c-993">Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-993">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="3707c-994">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="3707c-994">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="3707c-995">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="3707c-995">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="3707c-996">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="3707c-996">Reduced Kudu network calls</span></span>
* <span data-ttu-id="3707c-997">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="3707c-997">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="3707c-998">Consumo</span><span class="sxs-lookup"><span data-stu-id="3707c-998">Consumption</span></span>
* <span data-ttu-id="3707c-999">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="3707c-999">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-1000">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-1000">CosmosDB</span></span>
* <span data-ttu-id="3707c-1001">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="3707c-1001">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="3707c-1002">Mapas</span><span class="sxs-lookup"><span data-stu-id="3707c-1002">Maps</span></span>
* <span data-ttu-id="3707c-1003">Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1003">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1004">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1004">Network</span></span>
* <span data-ttu-id="3707c-1005">Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="3707c-1005">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="3707c-1006">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="3707c-1006">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-1007">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1007">Resource</span></span>
* <span data-ttu-id="3707c-1008">Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1008">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="3707c-1009">Se ha agregado un nuevo comando `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1009">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1010">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1010">Storage</span></span>
*  <span data-ttu-id="3707c-1011">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1011">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1012">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1012">VM</span></span>
* <span data-ttu-id="3707c-1013">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="3707c-1013">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="3707c-1014">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1014">December 4, 2018</span></span>

<span data-ttu-id="3707c-1015">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="3707c-1015">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="3707c-1016">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1016">Core</span></span>
* <span data-ttu-id="3707c-1017">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="3707c-1017">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="3707c-1018">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="3707c-1018">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1019">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-1019">Appservice</span></span>
* <span data-ttu-id="3707c-1020">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="3707c-1020">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="3707c-1021">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="3707c-1021">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1022">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1022">Network</span></span>
* <span data-ttu-id="3707c-1023">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="3707c-1023">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1024">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1024">Role</span></span>
* <span data-ttu-id="3707c-1025">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="3707c-1025">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="3707c-1026">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1026">VM</span></span>
* <span data-ttu-id="3707c-1027">[EN DESUSO] Se ha dejado de usar el parámetro `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="3707c-1027">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="3707c-1028">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="3707c-1028">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="3707c-1029">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="3707c-1029">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="3707c-1030">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="3707c-1030">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="3707c-1031">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1031">November 20, 2018</span></span>

<span data-ttu-id="3707c-1032">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="3707c-1032">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="3707c-1033">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1033">Core</span></span>
* <span data-ttu-id="3707c-1034">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="3707c-1034">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1035">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1035">ACR</span></span>
* <span data-ttu-id="3707c-1036">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="3707c-1036">Added context token to task step</span></span>
* <span data-ttu-id="3707c-1037">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="3707c-1037">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="3707c-1038">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1038">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1039">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-1039">Appservice</span></span>
* <span data-ttu-id="3707c-1040">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="3707c-1040">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="3707c-1041">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1041">Updated the default `node_version`.</span></span> <span data-ttu-id="3707c-1042">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="3707c-1042">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="3707c-1043">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="3707c-1043">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="3707c-1044">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="3707c-1044">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="3707c-1045">IotCentral</span><span class="sxs-lookup"><span data-stu-id="3707c-1045">IotCentral</span></span>
* <span data-ttu-id="3707c-1046">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="3707c-1046">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-1047">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3707c-1047">KeyVault</span></span>
* <span data-ttu-id="3707c-1048">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="3707c-1048">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1049">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1049">Network</span></span>
* <span data-ttu-id="3707c-1050">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="3707c-1050">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="3707c-1051">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="3707c-1051">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="3707c-1052">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="3707c-1052">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="3707c-1053">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1053">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-1054">Rdbms</span><span class="sxs-lookup"><span data-stu-id="3707c-1054">Rdbms</span></span>
* <span data-ttu-id="3707c-1055">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="3707c-1055">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="3707c-1056">Rbac</span><span class="sxs-lookup"><span data-stu-id="3707c-1056">Rbac</span></span>
* <span data-ttu-id="3707c-1057">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1057">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="3707c-1058">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1058">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="3707c-1059">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1059">Storage</span></span>
* <span data-ttu-id="3707c-1060">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="3707c-1060">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="3707c-1061">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="3707c-1061">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="3707c-1062">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="3707c-1062">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="3707c-1063">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3707c-1063">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1064">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1064">VM</span></span>
* <span data-ttu-id="3707c-1065">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="3707c-1065">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="3707c-1066">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1066">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="3707c-1067">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1067">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="3707c-1068">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1068">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="3707c-1069">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1069">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="3707c-1070">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1070">Added `snapshot wait` command</span></span>
* <span data-ttu-id="3707c-1071">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1071">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="3707c-1072">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1072">November 6, 2018</span></span>

<span data-ttu-id="3707c-1073">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="3707c-1073">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1074">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1074">Core</span></span>
* <span data-ttu-id="3707c-1075">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="3707c-1075">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1076">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1076">ACR</span></span>
* <span data-ttu-id="3707c-1077">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="3707c-1077">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="3707c-1078">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="3707c-1078">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1079">ACS</span></span>
* <span data-ttu-id="3707c-1080">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="3707c-1080">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="3707c-1081">Advisor</span><span class="sxs-lookup"><span data-stu-id="3707c-1081">Advisor</span></span>
* <span data-ttu-id="3707c-1082">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="3707c-1082">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-1083">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1083">AMS</span></span>
* <span data-ttu-id="3707c-1084">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-1084">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="3707c-1085">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-1085">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="3707c-1086">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1086">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="3707c-1087">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-1087">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="3707c-1088">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="3707c-1088">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="3707c-1089">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="3707c-1089">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="3707c-1090">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="3707c-1090">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="3707c-1091">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="3707c-1091">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="3707c-1092">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="3707c-1092">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="3707c-1093">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="3707c-1093">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="3707c-1094">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="3707c-1094">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="3707c-1095">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1095">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="3707c-1096">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="3707c-1096">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="3707c-1097">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="3707c-1097">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="3707c-1098">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1098">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="3707c-1099">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="3707c-1099">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="3707c-1100">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="3707c-1100">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1101">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1101">AppService</span></span>
* <span data-ttu-id="3707c-1102">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="3707c-1102">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="3707c-1103">Configuración</span><span class="sxs-lookup"><span data-stu-id="3707c-1103">Configure</span></span>
* <span data-ttu-id="3707c-1104">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="3707c-1104">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1105">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1105">Container</span></span>
* <span data-ttu-id="3707c-1106">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="3707c-1106">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="3707c-1107">EventHub</span><span class="sxs-lookup"><span data-stu-id="3707c-1107">EventHub</span></span>
* <span data-ttu-id="3707c-1108">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1108">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1109">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1109">Interactive</span></span>
* <span data-ttu-id="3707c-1110">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="3707c-1110">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-1111">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-1111">Monitor</span></span>
* <span data-ttu-id="3707c-1112">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1112">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1113">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1113">Network</span></span>
* <span data-ttu-id="3707c-1114">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="3707c-1114">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="3707c-1115">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="3707c-1115">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="3707c-1116">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1116">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="3707c-1117">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-1117">Profile</span></span>
* <span data-ttu-id="3707c-1118">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="3707c-1118">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-1119">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1119">RDBMS</span></span>
* <span data-ttu-id="3707c-1120">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="3707c-1120">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-1121">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1121">Resource</span></span>
* <span data-ttu-id="3707c-1122">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="3707c-1122">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1123">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1123">Role</span></span>
* <span data-ttu-id="3707c-1124">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="3707c-1124">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="3707c-1125">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="3707c-1125">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="3707c-1126">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="3707c-1126">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1127">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1127">Storage</span></span>
* <span data-ttu-id="3707c-1128">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="3707c-1128">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1129">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1129">VM</span></span>
* <span data-ttu-id="3707c-1130">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="3707c-1130">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="3707c-1131">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="3707c-1131">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="3707c-1132">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="3707c-1132">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="3707c-1133">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="3707c-1133">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="3707c-1134">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="3707c-1134">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="3707c-1135">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="3707c-1135">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="3707c-1136">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1136">October 23, 2018</span></span>

<span data-ttu-id="3707c-1137">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="3707c-1137">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1138">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1138">Core</span></span>
* <span data-ttu-id="3707c-1139">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="3707c-1139">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="3707c-1140">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="3707c-1140">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1141">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1141">ACR</span></span>
* <span data-ttu-id="3707c-1142">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="3707c-1142">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="3707c-1143">CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-1143">CDN</span></span>
* <span data-ttu-id="3707c-1144">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="3707c-1144">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="3707c-1145">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="3707c-1145">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1146">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1146">Container</span></span>
* <span data-ttu-id="3707c-1147">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="3707c-1147">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="3707c-1148">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-1148">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="3707c-1149">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="3707c-1149">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="3707c-1150">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-1150">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="3707c-1151">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="3707c-1151">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="3707c-1152">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="3707c-1152">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="3707c-1153">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="3707c-1153">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-1154">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-1154">CosmosDB</span></span>
* <span data-ttu-id="3707c-1155">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1155">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1156">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1156">Interactive</span></span>
* <span data-ttu-id="3707c-1157">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="3707c-1157">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="3707c-1158">IoT Central</span><span class="sxs-lookup"><span data-stu-id="3707c-1158">IoT Central</span></span>
* <span data-ttu-id="3707c-1159">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="3707c-1159">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="3707c-1160">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="3707c-1160">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-1161">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-1161">Monitor</span></span>
* <span data-ttu-id="3707c-1162">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="3707c-1162">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="3707c-1163">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="3707c-1163">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="3707c-1164">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="3707c-1164">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="3707c-1165">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="3707c-1165">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="3707c-1166">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="3707c-1166">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="3707c-1167">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="3707c-1167">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="3707c-1168">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="3707c-1168">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="3707c-1169">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="3707c-1169">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="3707c-1170">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="3707c-1170">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="3707c-1171">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1171">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1172">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1172">Network</span></span>
* <span data-ttu-id="3707c-1173">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="3707c-1173">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="3707c-1174">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="3707c-1174">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="3707c-1175">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="3707c-1175">ServiceBus</span></span>
* <span data-ttu-id="3707c-1176">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="3707c-1176">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1177">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1177">SQL</span></span>
* <span data-ttu-id="3707c-1178">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="3707c-1178">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1179">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1179">Storage</span></span>
* <span data-ttu-id="3707c-1180">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="3707c-1180">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="3707c-1181">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="3707c-1181">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1182">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1182">VM</span></span>
* <span data-ttu-id="3707c-1183">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1183">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="3707c-1184">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1184">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="3707c-1185">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1185">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="3707c-1186">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1186">October 16, 2018</span></span>

<span data-ttu-id="3707c-1187">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="3707c-1187">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1188">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1188">VM</span></span>
* <span data-ttu-id="3707c-1189">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="3707c-1189">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="3707c-1190">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1190">October 9, 2018</span></span>

<span data-ttu-id="3707c-1191">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="3707c-1191">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1192">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1192">Core</span></span>
* <span data-ttu-id="3707c-1193">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="3707c-1193">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1194">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1194">ACR</span></span>
* <span data-ttu-id="3707c-1195">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="3707c-1195">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1196">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1196">ACS</span></span>
* <span data-ttu-id="3707c-1197">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="3707c-1197">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="3707c-1198">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="3707c-1198">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="3707c-1199">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="3707c-1199">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="3707c-1200">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="3707c-1200">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1201">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1201">Container</span></span>
* <span data-ttu-id="3707c-1202">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="3707c-1202">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="3707c-1203">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="3707c-1203">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="3707c-1204">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="3707c-1204">Event Hub</span></span>
* <span data-ttu-id="3707c-1205">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1205">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="3707c-1206">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="3707c-1206">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="3707c-1207">Extensiones</span><span class="sxs-lookup"><span data-stu-id="3707c-1207">Extensions</span></span>
* <span data-ttu-id="3707c-1208">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="3707c-1208">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="3707c-1209">HDInsight</span><span class="sxs-lookup"><span data-stu-id="3707c-1209">HDInsight</span></span>
* <span data-ttu-id="3707c-1210">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="3707c-1210">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-1211">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-1211">IoT</span></span>
* <span data-ttu-id="3707c-1212">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="3707c-1212">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-1213">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3707c-1213">KeyVault</span></span>
* <span data-ttu-id="3707c-1214">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="3707c-1214">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1215">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1215">Network</span></span>
* <span data-ttu-id="3707c-1216">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3707c-1216">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="3707c-1217">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="3707c-1217">See #6052</span></span>
* <span data-ttu-id="3707c-1218">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1218">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="3707c-1219">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="3707c-1219">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="3707c-1220">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="3707c-1220">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="3707c-1221">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="3707c-1221">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="3707c-1222">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="3707c-1222">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="3707c-1223">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1223">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1224">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1224">Role</span></span>
* <span data-ttu-id="3707c-1225">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="3707c-1225">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="3707c-1226">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="3707c-1226">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="3707c-1227">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="3707c-1227">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="3707c-1228">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="3707c-1228">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="3707c-1229">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="3707c-1229">Service Bus</span></span>
* <span data-ttu-id="3707c-1230">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="3707c-1230">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1231">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1231">VM</span></span>
* <span data-ttu-id="3707c-1232">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="3707c-1232">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="3707c-1233">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="3707c-1233">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="3707c-1234">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="3707c-1234">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="3707c-1235">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="3707c-1235">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="3707c-1236">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="3707c-1236">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="3707c-1237">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="3707c-1237">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="3707c-1238">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1238">September 21, 2018</span></span>

<span data-ttu-id="3707c-1239">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="3707c-1239">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1240">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1240">ACR</span></span>
* <span data-ttu-id="3707c-1241">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1241">Added ACR Task commands</span></span>
* <span data-ttu-id="3707c-1242">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="3707c-1242">Added quick run command</span></span>
* <span data-ttu-id="3707c-1243">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="3707c-1243">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="3707c-1244">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1244">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="3707c-1245">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="3707c-1245">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="3707c-1246">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="3707c-1246">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1247">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1247">ACS</span></span>
* <span data-ttu-id="3707c-1248">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-1248">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="3707c-1249">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="3707c-1249">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1250">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1250">AppService</span></span>

* <span data-ttu-id="3707c-1251">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="3707c-1251">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="3707c-1252">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="3707c-1252">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="3707c-1253">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="3707c-1253">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="3707c-1254">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="3707c-1254">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-1255">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-1255">Batch</span></span>
* <span data-ttu-id="3707c-1256">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="3707c-1256">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="3707c-1257">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="3707c-1257">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="3707c-1258">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1258">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="3707c-1259">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="3707c-1259">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3707c-1260">Batch AI</span><span class="sxs-lookup"><span data-stu-id="3707c-1260">Batch AI</span></span> 
* <span data-ttu-id="3707c-1261">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1261">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3707c-1262">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="3707c-1262">Cognitive Services</span></span>
* <span data-ttu-id="3707c-1263">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="3707c-1263">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="3707c-1264">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="3707c-1264">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="3707c-1265">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="3707c-1265">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="3707c-1266">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="3707c-1266">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="3707c-1267">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1267">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="3707c-1268">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="3707c-1268">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1269">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1269">Container</span></span>
* <span data-ttu-id="3707c-1270">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="3707c-1270">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="3707c-1271">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="3707c-1271">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="3707c-1272">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1272">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="3707c-1273">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-1273">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="3707c-1274">DataLake</span><span class="sxs-lookup"><span data-stu-id="3707c-1274">Datalake</span></span>
* <span data-ttu-id="3707c-1275">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1275">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="3707c-1276">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="3707c-1276">Interactive Shell</span></span>
* <span data-ttu-id="3707c-1277">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="3707c-1277">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="3707c-1278">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="3707c-1278">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-1279">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-1279">IoT</span></span>
* <span data-ttu-id="3707c-1280">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-1280">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="3707c-1281">Key Vault</span><span class="sxs-lookup"><span data-stu-id="3707c-1281">Key Vault</span></span>
* <span data-ttu-id="3707c-1282">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="3707c-1282">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1283">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1283">Network</span></span>
* <span data-ttu-id="3707c-1284">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="3707c-1284">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="3707c-1285">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="3707c-1285">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="3707c-1286">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="3707c-1286">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="3707c-1287">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="3707c-1287">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="3707c-1288">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1288">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="3707c-1289">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1289">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="3707c-1290">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="3707c-1290">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="3707c-1291">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="3707c-1291">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="3707c-1292">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="3707c-1292">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="3707c-1293">`network express-route create/update`: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="3707c-1293">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="3707c-1294">`network vnet subnet create/update`: Se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="3707c-1294">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="3707c-1295">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1295">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="3707c-1296">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="3707c-1296">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="3707c-1297">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="3707c-1297">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="3707c-1298">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="3707c-1298">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="3707c-1299">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="3707c-1299">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="3707c-1300">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="3707c-1300">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="3707c-1301">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="3707c-1301">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-1302">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1302">RDBMS</span></span>
* <span data-ttu-id="3707c-1303">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="3707c-1303">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="3707c-1304">Reserva</span><span class="sxs-lookup"><span data-stu-id="3707c-1304">Reservation</span></span>
* <span data-ttu-id="3707c-1305">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="3707c-1305">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="3707c-1306">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="3707c-1306">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="3707c-1307">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="3707c-1307">Manage App</span></span>
* <span data-ttu-id="3707c-1308">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="3707c-1308">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="3707c-1309">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="3707c-1309">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1310">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1310">Role</span></span>
* <span data-ttu-id="3707c-1311">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="3707c-1311">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="3707c-1312">SignalR</span><span class="sxs-lookup"><span data-stu-id="3707c-1312">SignalR</span></span>
* <span data-ttu-id="3707c-1313">Primera versión</span><span class="sxs-lookup"><span data-stu-id="3707c-1313">First release</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1314">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1314">Storage</span></span>
* <span data-ttu-id="3707c-1315">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="3707c-1315">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="3707c-1316">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="3707c-1316">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1317">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1317">VM</span></span>
* <span data-ttu-id="3707c-1318">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="3707c-1318">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="3707c-1319">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="3707c-1319">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="3707c-1320">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1320">August 28, 2018</span></span>

<span data-ttu-id="3707c-1321">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="3707c-1321">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1322">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1322">Core</span></span>

* <span data-ttu-id="3707c-1323">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="3707c-1323">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="3707c-1324">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3707c-1324">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1325">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1325">ACR</span></span>

* <span data-ttu-id="3707c-1326">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="3707c-1326">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="3707c-1327">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="3707c-1327">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1328">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1328">ACS</span></span>

* <span data-ttu-id="3707c-1329">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="3707c-1329">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="3707c-1330">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="3707c-1330">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1331">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1331">AppService</span></span>

* <span data-ttu-id="3707c-1332">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="3707c-1332">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="3707c-1333">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1333">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="3707c-1334">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-1334">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="3707c-1335">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="3707c-1335">Backup</span></span>

* <span data-ttu-id="3707c-1336">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-1336">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="3707c-1337">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="3707c-1337">Bot Service</span></span>

* <span data-ttu-id="3707c-1338">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="3707c-1338">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3707c-1339">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="3707c-1339">Cognitive Services</span></span>

* <span data-ttu-id="3707c-1340">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="3707c-1340">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-1341">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-1341">IoT</span></span>

* <span data-ttu-id="3707c-1342">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="3707c-1342">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-1343">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-1343">Monitor</span></span>

* <span data-ttu-id="3707c-1344">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="3707c-1344">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="3707c-1345">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="3707c-1345">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1346">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1346">Network</span></span>

* <span data-ttu-id="3707c-1347">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-1347">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-1348">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1348">Resource</span></span>

* <span data-ttu-id="3707c-1349">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-1349">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1350">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1350">Storage</span></span>

* <span data-ttu-id="3707c-1351">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-1351">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1352">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1352">VM</span></span>

* <span data-ttu-id="3707c-1353">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-1353">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="3707c-1354">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1354">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="3707c-1355">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1355">Auguest 14, 2018</span></span>

<span data-ttu-id="3707c-1356">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="3707c-1356">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1357">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1357">Core</span></span>

* <span data-ttu-id="3707c-1358">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="3707c-1358">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="3707c-1359">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="3707c-1359">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="3707c-1360">Telemetría</span><span class="sxs-lookup"><span data-stu-id="3707c-1360">Telemetry</span></span>

* <span data-ttu-id="3707c-1361">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="3707c-1361">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1362">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1362">ACR</span></span>

* <span data-ttu-id="3707c-1363">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1363">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="3707c-1364">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="3707c-1364">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1365">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1365">ACS</span></span>

* <span data-ttu-id="3707c-1366">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="3707c-1366">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="3707c-1367">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="3707c-1367">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="3707c-1368">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="3707c-1368">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="3707c-1369">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="3707c-1369">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="3707c-1370">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="3707c-1370">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="3707c-1371">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1371">AppService</span></span>

* <span data-ttu-id="3707c-1372">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="3707c-1372">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="3707c-1373">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="3707c-1373">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="3707c-1374">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3707c-1374">BatchAI</span></span>

* <span data-ttu-id="3707c-1375">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="3707c-1375">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="3707c-1376">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1376">Container</span></span>

* <span data-ttu-id="3707c-1377">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1377">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="3707c-1378">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-1378">IoT</span></span>

* <span data-ttu-id="3707c-1379">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="3707c-1379">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="3707c-1380">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="3707c-1380">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="3707c-1381">Iot Central</span><span class="sxs-lookup"><span data-stu-id="3707c-1381">Iot Central</span></span>

* <span data-ttu-id="3707c-1382">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="3707c-1382">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-1383">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3707c-1383">KeyVault</span></span>


* <span data-ttu-id="3707c-1384">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="3707c-1384">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="3707c-1385">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="3707c-1385">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="3707c-1386">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="3707c-1386">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="3707c-1387">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="3707c-1387">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="3707c-1388">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="3707c-1388">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="3707c-1389">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="3707c-1389">Relay</span></span>

* <span data-ttu-id="3707c-1390">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="3707c-1390">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1391">Sql</span><span class="sxs-lookup"><span data-stu-id="3707c-1391">Sql</span></span>

* <span data-ttu-id="3707c-1392">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1392">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1393">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1393">Storage</span></span>

* <span data-ttu-id="3707c-1394">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="3707c-1394">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="3707c-1395">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="3707c-1395">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="3707c-1396">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="3707c-1396">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="3707c-1397">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="3707c-1397">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="3707c-1398">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1398">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1399">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1399">VM</span></span>

* <span data-ttu-id="3707c-1400">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="3707c-1400">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="3707c-1401">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1401">July 31, 2018</span></span>

<span data-ttu-id="3707c-1402">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="3707c-1402">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1403">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1403">ACR</span></span>

* <span data-ttu-id="3707c-1404">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1404">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="3707c-1405">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1405">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1406">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1406">ACS</span></span>

* <span data-ttu-id="3707c-1407">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="3707c-1407">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-1408">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-1408">Batch</span></span>

* <span data-ttu-id="3707c-1409">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="3707c-1409">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1410">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1410">Container</span></span>

* <span data-ttu-id="3707c-1411">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="3707c-1411">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1412">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1412">Network</span></span>

* <span data-ttu-id="3707c-1413">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3707c-1413">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="3707c-1414">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1414">Resource</span></span>

* <span data-ttu-id="3707c-1415">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="3707c-1415">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="3707c-1416">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="3707c-1416">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1417">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1417">Role</span></span>

* <span data-ttu-id="3707c-1418">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="3707c-1418">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="3707c-1419">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="3707c-1419">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="3707c-1420">Search</span><span class="sxs-lookup"><span data-stu-id="3707c-1420">Search</span></span>

* <span data-ttu-id="3707c-1421">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="3707c-1421">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="3707c-1422">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="3707c-1422">Service Bus</span></span>

* <span data-ttu-id="3707c-1423">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="3707c-1423">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="3707c-1424">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="3707c-1424">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="3707c-1425">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="3707c-1425">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="3707c-1426">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="3707c-1426">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1427">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1427">Storage</span></span>

* <span data-ttu-id="3707c-1428">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="3707c-1428">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="3707c-1429">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1429">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1430">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1430">VM</span></span>

* <span data-ttu-id="3707c-1431">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="3707c-1431">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="3707c-1432">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="3707c-1432">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="3707c-1433">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="3707c-1433">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="3707c-1434">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="3707c-1434">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="3707c-1435">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1435">July 18, 2018</span></span>

<span data-ttu-id="3707c-1436">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="3707c-1436">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1437">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1437">Core</span></span>

* <span data-ttu-id="3707c-1438">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="3707c-1438">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="3707c-1439">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="3707c-1439">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="3707c-1440">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-1440">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1441">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1441">ACR</span></span>

* <span data-ttu-id="3707c-1442">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="3707c-1442">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="3707c-1443">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="3707c-1443">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="3707c-1444">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="3707c-1444">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="3707c-1445">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="3707c-1445">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1446">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1446">ACS</span></span>

* <span data-ttu-id="3707c-1447">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="3707c-1447">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1448">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1448">AppService</span></span>

* <span data-ttu-id="3707c-1449">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="3707c-1449">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-1450">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-1450">Batch</span></span>

* <span data-ttu-id="3707c-1451">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="3707c-1451">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="3707c-1452">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="3707c-1452">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3707c-1453">Batch AI</span><span class="sxs-lookup"><span data-stu-id="3707c-1453">Batch AI</span></span>

* <span data-ttu-id="3707c-1454">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="3707c-1454">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1455">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1455">Container</span></span>

* <span data-ttu-id="3707c-1456">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="3707c-1456">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="3707c-1457">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="3707c-1457">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1458">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1458">Network</span></span>

* <span data-ttu-id="3707c-1459">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1459">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="3707c-1460">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1460">Added `network nic wait`</span></span>
* <span data-ttu-id="3707c-1461">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="3707c-1461">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="3707c-1462">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="3707c-1462">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="3707c-1463">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1463">Resource</span></span>

* <span data-ttu-id="3707c-1464">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="3707c-1464">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="3707c-1465">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="3707c-1465">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="3707c-1466">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1466">Added `deployment wait` command</span></span>
* <span data-ttu-id="3707c-1467">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="3707c-1467">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1468">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1468">SQL</span></span>

* <span data-ttu-id="3707c-1469">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1469">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="3707c-1470">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="3707c-1470">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="3707c-1471">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="3707c-1471">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1472">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1472">Storage</span></span>

* <span data-ttu-id="3707c-1473">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="3707c-1473">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1474">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1474">VM</span></span>

* <span data-ttu-id="3707c-1475">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="3707c-1475">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="3707c-1476">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1476">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="3707c-1477">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1477">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="3707c-1478">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1478">July 3, 2018</span></span>

<span data-ttu-id="3707c-1479">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="3707c-1479">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="3707c-1480">AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-1480">AKS</span></span>

* <span data-ttu-id="3707c-1481">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="3707c-1481">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="3707c-1482">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1482">July 3, 2018</span></span>

<span data-ttu-id="3707c-1483">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="3707c-1483">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1484">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1484">Core</span></span>

* <span data-ttu-id="3707c-1485">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="3707c-1485">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1486">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1486">ACR</span></span>

* <span data-ttu-id="3707c-1487">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="3707c-1487">Added polling build status</span></span>
* <span data-ttu-id="3707c-1488">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="3707c-1488">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="3707c-1489">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="3707c-1489">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1490">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1490">ACS</span></span>

* <span data-ttu-id="3707c-1491">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="3707c-1491">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="3707c-1492">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="3707c-1492">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="3707c-1493">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1493">Updated options for `aks browse` command.</span></span> <span data-ttu-id="3707c-1494">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="3707c-1494">Added `--listen-port` support</span></span>
* <span data-ttu-id="3707c-1495">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1495">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="3707c-1496">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="3707c-1496">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="3707c-1497">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="3707c-1497">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1498">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1498">AppService</span></span>

* <span data-ttu-id="3707c-1499">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="3707c-1499">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="3707c-1500">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="3707c-1500">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="3707c-1501">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="3707c-1501">Backup</span></span>

* <span data-ttu-id="3707c-1502">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="3707c-1502">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="3707c-1503">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3707c-1503">BatchAI</span></span>

* <span data-ttu-id="3707c-1504">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="3707c-1504">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="3707c-1505">Nube</span><span class="sxs-lookup"><span data-stu-id="3707c-1505">Cloud</span></span>

* <span data-ttu-id="3707c-1506">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="3707c-1506">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1507">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1507">Container</span></span>

* <span data-ttu-id="3707c-1508">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="3707c-1508">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="3707c-1509">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="3707c-1509">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="3707c-1510">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="3707c-1510">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-1511">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-1511">Extension</span></span>

* <span data-ttu-id="3707c-1512">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="3707c-1512">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1513">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1513">Network</span></span>

* <span data-ttu-id="3707c-1514">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="3707c-1514">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-1515">Rdbms</span><span class="sxs-lookup"><span data-stu-id="3707c-1515">Rdbms</span></span>

* <span data-ttu-id="3707c-1516">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1516">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-1517">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1517">Resource</span></span>

* <span data-ttu-id="3707c-1518">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="3707c-1518">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1519">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1519">VM</span></span>

* <span data-ttu-id="3707c-1520">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="3707c-1520">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="3707c-1521">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1521">June 25, 2018</span></span>

<span data-ttu-id="3707c-1522">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="3707c-1522">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="3707c-1523">CLI</span><span class="sxs-lookup"><span data-stu-id="3707c-1523">CLI</span></span>

* <span data-ttu-id="3707c-1524">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-1524">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="3707c-1525">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1525">June 19, 2018</span></span>

<span data-ttu-id="3707c-1526">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="3707c-1526">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1527">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1527">Core</span></span>

* <span data-ttu-id="3707c-1528">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1528">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1529">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1529">ACR</span></span>

* <span data-ttu-id="3707c-1530">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="3707c-1530">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="3707c-1531">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="3707c-1531">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1532">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1532">ACS</span></span>

* <span data-ttu-id="3707c-1533">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1533">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="3707c-1534">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1534">Added `--update` support</span></span>
* <span data-ttu-id="3707c-1535">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="3707c-1535">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="3707c-1536">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="3707c-1536">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="3707c-1537">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="3707c-1537">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="3707c-1538">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="3707c-1538">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="3707c-1539">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="3707c-1539">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="3707c-1540">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="3707c-1540">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1541">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1541">AppService</span></span>

* <span data-ttu-id="3707c-1542">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="3707c-1542">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="3707c-1543">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="3707c-1543">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-1544">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-1544">Batch</span></span>

* <span data-ttu-id="3707c-1545">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="3707c-1545">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3707c-1546">Batch AI</span><span class="sxs-lookup"><span data-stu-id="3707c-1546">Batch AI</span></span>

* <span data-ttu-id="3707c-1547">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="3707c-1547">Added support for workspaces.</span></span> <span data-ttu-id="3707c-1548">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="3707c-1548">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="3707c-1549">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="3707c-1549">Added support for experiments.</span></span> <span data-ttu-id="3707c-1550">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="3707c-1550">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="3707c-1551">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="3707c-1551">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="3707c-1552">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1552">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="3707c-1553">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="3707c-1553">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="3707c-1554">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1554">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="3707c-1555">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="3707c-1555">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="3707c-1556">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="3707c-1556">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="3707c-1557">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1557">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="3707c-1558">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1558">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="3707c-1559">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1559">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="3707c-1560">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1560">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="3707c-1561">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="3707c-1561">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="3707c-1562">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="3707c-1562">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="3707c-1563">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1563">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="3707c-1564">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="3707c-1564">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="3707c-1565">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="3707c-1565">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="3707c-1566">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="3707c-1566">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="3707c-1567">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="3707c-1567">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="3707c-1568">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="3707c-1568">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="3707c-1569">Mapas</span><span class="sxs-lookup"><span data-stu-id="3707c-1569">Maps</span></span>

* <span data-ttu-id="3707c-1570">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1570">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1571">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1571">Network</span></span>

* <span data-ttu-id="3707c-1572">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="3707c-1572">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="3707c-1573">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="3707c-1573">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="3707c-1574">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="3707c-1574">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="3707c-1575">Reservations</span><span class="sxs-lookup"><span data-stu-id="3707c-1575">Reservations</span></span>

* <span data-ttu-id="3707c-1576">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1576">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="3707c-1577">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1577">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="3707c-1578">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1578">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="3707c-1579">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1579">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="3707c-1580">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1580">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="3707c-1581">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1581">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1582">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1582">Role</span></span>

* <span data-ttu-id="3707c-1583">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="3707c-1583">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1584">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1584">SQL</span></span>

* <span data-ttu-id="3707c-1585">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="3707c-1585">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1586">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1586">Storage</span></span>

* <span data-ttu-id="3707c-1587">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="3707c-1587">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1588">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1588">VM</span></span>

* <span data-ttu-id="3707c-1589">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1589">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="3707c-1590">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="3707c-1590">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="3707c-1591">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="3707c-1591">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="3707c-1592">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1592">June 13, 2018</span></span>

<span data-ttu-id="3707c-1593">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="3707c-1593">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1594">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1594">Core</span></span>

* <span data-ttu-id="3707c-1595">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="3707c-1595">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="3707c-1596">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1596">June 13, 2018</span></span>

<span data-ttu-id="3707c-1597">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="3707c-1597">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="3707c-1598">AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-1598">AKS</span></span>

* <span data-ttu-id="3707c-1599">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1599">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="3707c-1600">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="3707c-1600">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="3707c-1601">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1601">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="3707c-1602">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1602">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="3707c-1603">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1603">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1604">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1604">AppService</span></span>

* <span data-ttu-id="3707c-1605">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="3707c-1605">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="3707c-1606">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1606">June 5, 2018</span></span>

<span data-ttu-id="3707c-1607">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="3707c-1607">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1608">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1608">Interactive</span></span>

* <span data-ttu-id="3707c-1609">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="3707c-1609">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="3707c-1610">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1610">June 5, 2018</span></span>

<span data-ttu-id="3707c-1611">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="3707c-1611">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1612">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1612">Core</span></span>

* <span data-ttu-id="3707c-1613">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="3707c-1613">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="3707c-1614">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="3707c-1614">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1615">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1615">ACR</span></span>

* <span data-ttu-id="3707c-1616">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="3707c-1616">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="3707c-1617">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1617">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="3707c-1618">AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-1618">AKS</span></span>

* <span data-ttu-id="3707c-1619">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="3707c-1619">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-1620">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-1620">Batch</span></span>

* <span data-ttu-id="3707c-1621">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="3707c-1621">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-1622">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-1622">IOT</span></span>

* <span data-ttu-id="3707c-1623">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="3707c-1623">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1624">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1624">Network</span></span>

* <span data-ttu-id="3707c-1625">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="3707c-1625">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="3707c-1626">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="3707c-1626">Policy Insights</span></span>

* <span data-ttu-id="3707c-1627">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="3707c-1627">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="3707c-1628">ARM</span><span class="sxs-lookup"><span data-stu-id="3707c-1628">ARM</span></span>

* <span data-ttu-id="3707c-1629">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1629">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1630">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1630">SQL</span></span>

* <span data-ttu-id="3707c-1631">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="3707c-1631">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="3707c-1632">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="3707c-1632">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="3707c-1633">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1633">Storage</span></span>

* <span data-ttu-id="3707c-1634">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="3707c-1634">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1635">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1635">VM</span></span>

* <span data-ttu-id="3707c-1636">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="3707c-1636">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="3707c-1637">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1637">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="3707c-1638">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1638">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="3707c-1639">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1639">May 22, 2018</span></span>

<span data-ttu-id="3707c-1640">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="3707c-1640">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1641">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1641">Core</span></span>

* <span data-ttu-id="3707c-1642">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="3707c-1642">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1643">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1643">ACS</span></span>

* <span data-ttu-id="3707c-1644">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="3707c-1644">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="3707c-1645">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="3707c-1645">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1646">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-1646">AppService</span></span>

* <span data-ttu-id="3707c-1647">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="3707c-1647">Improved generic update commands</span></span>
* <span data-ttu-id="3707c-1648">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="3707c-1648">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1649">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1649">Container</span></span>

* <span data-ttu-id="3707c-1650">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="3707c-1650">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="3707c-1651">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-1651">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-1652">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-1652">Extension</span></span>

* <span data-ttu-id="3707c-1653">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="3707c-1653">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1654">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1654">Interactive</span></span>

* <span data-ttu-id="3707c-1655">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="3707c-1655">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="3707c-1656">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="3707c-1656">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-1657">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3707c-1657">KeyVault</span></span>

* <span data-ttu-id="3707c-1658">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="3707c-1658">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1659">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1659">Network</span></span>

* <span data-ttu-id="3707c-1660">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="3707c-1660">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="3707c-1661">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="3707c-1661">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1662">SQL</span></span>

* <span data-ttu-id="3707c-1663">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="3707c-1663">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="3707c-1664">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="3707c-1664">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="3707c-1665">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="3707c-1665">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="3707c-1666">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="3707c-1666">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="3707c-1667">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="3707c-1667">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="3707c-1668">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1668">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="3707c-1669">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="3707c-1669">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="3707c-1670">`edition`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1670">`edition`.</span></span> <span data-ttu-id="3707c-1671">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="3707c-1671">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="3707c-1672">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1672">`elasticPoolName`.</span></span> <span data-ttu-id="3707c-1673">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="3707c-1673">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="3707c-1674">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="3707c-1674">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="3707c-1675">`edition`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1675">`edition`.</span></span> <span data-ttu-id="3707c-1676">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="3707c-1676">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="3707c-1677">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1677">`dtu`.</span></span> <span data-ttu-id="3707c-1678">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="3707c-1678">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="3707c-1679">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1679">`databaseDtuMin`.</span></span> <span data-ttu-id="3707c-1680">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="3707c-1680">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="3707c-1681">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1681">`databaseDtuMax`.</span></span> <span data-ttu-id="3707c-1682">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="3707c-1682">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="3707c-1683">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1683">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="3707c-1684">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1684">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1685">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1685">Storage</span></span>

* <span data-ttu-id="3707c-1686">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="3707c-1686">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="3707c-1687">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="3707c-1687">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1688">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1688">VM</span></span>

* <span data-ttu-id="3707c-1689">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1689">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="3707c-1690">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="3707c-1690">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="3707c-1691">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="3707c-1691">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="3707c-1692">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="3707c-1692">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="3707c-1693">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1693">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="3707c-1694">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1694">May 7, 2018</span></span>

<span data-ttu-id="3707c-1695">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="3707c-1695">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1696">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1696">Core</span></span>

* <span data-ttu-id="3707c-1697">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="3707c-1697">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="3707c-1698">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="3707c-1698">Added limited support for positional arguments</span></span>
* <span data-ttu-id="3707c-1699">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1699">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="3707c-1700">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="3707c-1700">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="3707c-1701">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1701">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="3707c-1702">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="3707c-1702">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="3707c-1703">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1703">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="3707c-1704">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="3707c-1704">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="3707c-1705">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1705">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1706">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1706">ACR</span></span>

* <span data-ttu-id="3707c-1707">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="3707c-1707">Added ACR Build commands</span></span>
* <span data-ttu-id="3707c-1708">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="3707c-1708">Improved resource not found error messages</span></span>
* <span data-ttu-id="3707c-1709">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="3707c-1709">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="3707c-1710">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="3707c-1710">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="3707c-1711">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="3707c-1711">Improved repository commands error messages</span></span>
* <span data-ttu-id="3707c-1712">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="3707c-1712">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1713">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1713">ACS</span></span>

* <span data-ttu-id="3707c-1714">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-1714">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="3707c-1715">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="3707c-1715">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="3707c-1716">AMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1716">AMS</span></span>

* <span data-ttu-id="3707c-1717">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="3707c-1717">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1718">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-1718">Appservice</span></span>

* <span data-ttu-id="3707c-1719">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="3707c-1719">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="3707c-1720">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1720">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="3707c-1721">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="3707c-1721">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="3707c-1722">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-1722">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="3707c-1723">Batch AI</span><span class="sxs-lookup"><span data-stu-id="3707c-1723">Batch AI</span></span>

* <span data-ttu-id="3707c-1724">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="3707c-1724">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3707c-1725">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="3707c-1725">Cognitive Services</span></span>

* <span data-ttu-id="3707c-1726">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="3707c-1726">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="3707c-1727">Consumo</span><span class="sxs-lookup"><span data-stu-id="3707c-1727">Consumption</span></span>

* <span data-ttu-id="3707c-1728">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="3707c-1728">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1729">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1729">Container</span></span>

* <span data-ttu-id="3707c-1730">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="3707c-1730">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="3707c-1731">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3707c-1731">Cosmos DB</span></span>

* <span data-ttu-id="3707c-1732">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3707c-1732">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="3707c-1733">DMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1733">DMS</span></span>

* <span data-ttu-id="3707c-1734">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1734">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-1735">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-1735">Extension</span></span>

* <span data-ttu-id="3707c-1736">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="3707c-1736">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1737">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1737">Interactive</span></span>

* <span data-ttu-id="3707c-1738">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="3707c-1738">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="3707c-1739">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="3707c-1739">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="3707c-1740">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="3707c-1740">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="3707c-1741">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1741">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="3707c-1742">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-1742">Lab</span></span>

* <span data-ttu-id="3707c-1743">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="3707c-1743">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1744">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1744">Network</span></span>

* <span data-ttu-id="3707c-1745">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="3707c-1745">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="3707c-1746">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-1746">Profile</span></span>

* <span data-ttu-id="3707c-1747">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1747">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="3707c-1748">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="3707c-1748">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="3707c-1749">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="3707c-1749">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="3707c-1750">Redis</span><span class="sxs-lookup"><span data-stu-id="3707c-1750">Redis</span></span>

* <span data-ttu-id="3707c-1751">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="3707c-1751">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="3707c-1752">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1752">Deprecated `redis list-all`.</span></span> <span data-ttu-id="3707c-1753">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="3707c-1753">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="3707c-1754">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="3707c-1754">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="3707c-1755">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1755">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1756">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1756">Role</span></span>

* <span data-ttu-id="3707c-1757">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="3707c-1757">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1758">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1758">Storage</span></span>

* <span data-ttu-id="3707c-1759">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="3707c-1759">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="3707c-1760">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="3707c-1760">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="3707c-1761">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="3707c-1761">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="3707c-1762">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="3707c-1762">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="3707c-1763">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="3707c-1763">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1764">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1764">VM</span></span>

* <span data-ttu-id="3707c-1765">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="3707c-1765">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="3707c-1766">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="3707c-1766">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="3707c-1767">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="3707c-1767">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="3707c-1768">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="3707c-1768">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="3707c-1769">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="3707c-1769">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="3707c-1770">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="3707c-1770">Added write accelerator support</span></span>
* <span data-ttu-id="3707c-1771">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1771">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="3707c-1772">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="3707c-1772">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="3707c-1773">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="3707c-1773">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="3707c-1774">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1774">April 10, 2018</span></span>

<span data-ttu-id="3707c-1775">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="3707c-1775">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1776">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1776">ACR</span></span>

* <span data-ttu-id="3707c-1777">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="3707c-1777">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1778">ACS</span></span>

* <span data-ttu-id="3707c-1779">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="3707c-1779">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1780">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-1780">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="3707c-1782">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="3707c-1782">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="3707c-1783">BatchAI</span><span class="sxs-lookup"><span data-stu-id="3707c-1783">BatchAI</span></span>

* <span data-ttu-id="3707c-1784">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="3707c-1784">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="3707c-1785">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="3707c-1785">Job level mounting</span></span>
  - <span data-ttu-id="3707c-1786">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="3707c-1786">Environment variables with secret values</span></span>
  - <span data-ttu-id="3707c-1787">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="3707c-1787">Performance counters settings</span></span>
  - <span data-ttu-id="3707c-1788">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="3707c-1788">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="3707c-1789">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="3707c-1789">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="3707c-1790">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="3707c-1790">Usage and limits reporting</span></span>
  - <span data-ttu-id="3707c-1791">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="3707c-1791">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="3707c-1792">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="3707c-1792">Support for custom images</span></span>
  - <span data-ttu-id="3707c-1793">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="3707c-1793">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="3707c-1794">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="3707c-1794">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="3707c-1795">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="3707c-1795">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="3707c-1796">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="3707c-1796">National clouds are supported</span></span>
* <span data-ttu-id="3707c-1797">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="3707c-1797">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="3707c-1798">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="3707c-1798">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="3707c-1799">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="3707c-1799">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="3707c-1800">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="3707c-1800">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="3707c-1801">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="3707c-1801">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="3707c-1802">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="3707c-1802">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="3707c-1803">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1803">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="3707c-1804">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="3707c-1804">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="3707c-1805">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="3707c-1805">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="3707c-1806">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1806">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="3707c-1807">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1807">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="3707c-1808">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="3707c-1808">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="3707c-1809">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1809">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="3707c-1810">Facturación</span><span class="sxs-lookup"><span data-stu-id="3707c-1810">Billing</span></span>

* <span data-ttu-id="3707c-1811">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="3707c-1811">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="3707c-1812">Consumo</span><span class="sxs-lookup"><span data-stu-id="3707c-1812">Consumption</span></span>

* <span data-ttu-id="3707c-1813">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1813">Added `marketplace` commands</span></span>
* <span data-ttu-id="3707c-1814">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="3707c-1814">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="3707c-1815">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="3707c-1815">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="3707c-1816">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="3707c-1816">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="3707c-1817">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="3707c-1817">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="3707c-1818">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="3707c-1818">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1819">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1819">Container</span></span>

* <span data-ttu-id="3707c-1820">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="3707c-1820">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="3707c-1821">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="3707c-1821">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-1822">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-1822">Extension</span></span>

* <span data-ttu-id="3707c-1823">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="3707c-1823">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1824">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1824">Interactive</span></span>

* <span data-ttu-id="3707c-1825">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="3707c-1825">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="3707c-1826">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1826">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="3707c-1827">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="3707c-1827">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1828">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1828">Network</span></span>

* <span data-ttu-id="3707c-1829">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1829">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="3707c-1830">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1830">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="3707c-1831">4910</span><span class="sxs-lookup"><span data-stu-id="3707c-1831">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="3707c-1832">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="3707c-1832">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="3707c-1833">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="3707c-1833">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="3707c-1834">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1834">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="3707c-1835">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1835">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="3707c-1836">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="3707c-1836">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-1837">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-1837">Profile</span></span>

* <span data-ttu-id="3707c-1838">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="3707c-1838">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="3707c-1839">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="3707c-1839">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-1840">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1840">RDBMS</span></span>

* <span data-ttu-id="3707c-1841">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1841">Added `georestore` command</span></span>
* <span data-ttu-id="3707c-1842">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1842">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-1843">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1843">Resource</span></span>

* <span data-ttu-id="3707c-1844">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1844">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="3707c-1845">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1845">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1846">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1846">SQL</span></span>

* <span data-ttu-id="3707c-1847">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="3707c-1847">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1848">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1848">Storage</span></span>

* <span data-ttu-id="3707c-1849">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="3707c-1849">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1850">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1850">VM</span></span>

* <span data-ttu-id="3707c-1851">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1851">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="3707c-1852">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="3707c-1852">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="3707c-1854">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1854">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="3707c-1855">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="3707c-1855">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="3707c-1856">5718</span><span class="sxs-lookup"><span data-stu-id="3707c-1856">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="3707c-1857">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="3707c-1857">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="3707c-1858">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1858">March 27, 2018</span></span>

<span data-ttu-id="3707c-1859">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="3707c-1859">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1860">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1860">Core</span></span>

* <span data-ttu-id="3707c-1861">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="3707c-1861">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1862">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1862">ACS</span></span>

* <span data-ttu-id="3707c-1863">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="3707c-1863">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1864">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-1864">Appservice</span></span>

* <span data-ttu-id="3707c-1865">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1865">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="3707c-1866">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1866">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="3707c-1867">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="3707c-1867">Backup</span></span>

* <span data-ttu-id="3707c-1868">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1868">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="3707c-1869">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1869">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="3707c-1870">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-1870">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="3707c-1871">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="3707c-1871">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1872">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1872">Container</span></span>

* <span data-ttu-id="3707c-1873">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1873">Added `container exec` command.</span></span> <span data-ttu-id="3707c-1874">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="3707c-1874">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="3707c-1875">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-1875">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-1876">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-1876">Extension</span></span>

* <span data-ttu-id="3707c-1877">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-1877">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="3707c-1878">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="3707c-1878">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="3707c-1879">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="3707c-1879">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1880">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1880">Interactive</span></span>

* <span data-ttu-id="3707c-1881">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1881">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="3707c-1882">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="3707c-1882">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="3707c-1883">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-1883">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="3707c-1884">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="3707c-1884">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="3707c-1885">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-1885">Lab</span></span>

* <span data-ttu-id="3707c-1886">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="3707c-1886">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-1887">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-1887">Monitor</span></span>

* <span data-ttu-id="3707c-1888">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="3707c-1888">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="3707c-1889">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="3707c-1889">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="3707c-1890">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="3707c-1890">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1891">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1891">Network</span></span>

* <span data-ttu-id="3707c-1892">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="3707c-1892">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-1893">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-1893">Profile</span></span>

* <span data-ttu-id="3707c-1894">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="3707c-1894">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-1895">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1895">RDBMS</span></span>

* <span data-ttu-id="3707c-1896">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="3707c-1896">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-1897">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1897">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="3707c-1899">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1899">Role</span></span>

* <span data-ttu-id="3707c-1900">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1900">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="3707c-1901">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="3707c-1901">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="3707c-1902">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1902">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="3707c-1903">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1903">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="3707c-1904">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="3707c-1904">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1905">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1905">Storage</span></span>

* <span data-ttu-id="3707c-1906">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="3707c-1906">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="3707c-1907">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="3707c-1907">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1908">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1908">VM</span></span>

* <span data-ttu-id="3707c-1909">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="3707c-1909">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="3707c-1910">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1910">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="3707c-1911">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="3707c-1911">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="3707c-1912">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="3707c-1912">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="3707c-1913">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1913">March 13, 2018</span></span>

<span data-ttu-id="3707c-1914">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="3707c-1914">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-1915">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-1915">ACR</span></span>

* <span data-ttu-id="3707c-1916">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1916">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="3707c-1917">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1917">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="3707c-1918">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="3707c-1918">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1919">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1919">ACS</span></span>

* <span data-ttu-id="3707c-1920">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="3707c-1920">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="3707c-1921">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="3707c-1921">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="3707c-1922">Advisor</span><span class="sxs-lookup"><span data-stu-id="3707c-1922">Advisor</span></span>

* <span data-ttu-id="3707c-1923">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="3707c-1923">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="3707c-1924">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="3707c-1924">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="3707c-1925">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="3707c-1925">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="3707c-1926">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="3707c-1926">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="3707c-1927">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1927">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1928">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-1928">Appservice</span></span>

* <span data-ttu-id="3707c-1929">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1929">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="3707c-1930">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1930">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="3707c-1931">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="3707c-1931">Eventhubs</span></span>

* <span data-ttu-id="3707c-1932">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="3707c-1932">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-1933">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-1933">Extension</span></span>

* <span data-ttu-id="3707c-1934">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="3707c-1934">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-1935">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-1935">Interactive</span></span>

* <span data-ttu-id="3707c-1936">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="3707c-1936">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="3707c-1937">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="3707c-1937">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="3707c-1938">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="3707c-1938">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="3707c-1939">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="3707c-1939">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-1940">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-1940">Monitor</span></span>

* <span data-ttu-id="3707c-1941">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1941">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="3707c-1942">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1942">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="3707c-1943">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1943">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="3707c-1944">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1944">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1945">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1945">Network</span></span>

* <span data-ttu-id="3707c-1946">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="3707c-1946">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="3707c-1947">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-1947">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="3707c-1948">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1948">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="3707c-1949">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1949">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-1950">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-1950">Profile</span></span>

* <span data-ttu-id="3707c-1951">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1951">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="3707c-1952">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="3707c-1952">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-1953">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-1953">RDBMS</span></span>

* <span data-ttu-id="3707c-1954">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="3707c-1954">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="3707c-1955">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="3707c-1955">Service Bus</span></span>

* <span data-ttu-id="3707c-1956">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="3707c-1956">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1957">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1957">Storage</span></span>

* <span data-ttu-id="3707c-1958">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="3707c-1958">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="3707c-1959">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="3707c-1959">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1960">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1960">VM</span></span>

* <span data-ttu-id="3707c-1961">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="3707c-1961">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="3707c-1962">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1962">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="3707c-1963">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-1963">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="3707c-1964">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="3707c-1964">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="3707c-1965">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1965">February 27, 2018</span></span>

<span data-ttu-id="3707c-1966">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="3707c-1966">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="3707c-1967">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-1967">Core</span></span>

* <span data-ttu-id="3707c-1968">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="3707c-1968">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="3707c-1969">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="3707c-1969">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="3707c-1970">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="3707c-1970">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-1971">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-1971">ACS</span></span>

* <span data-ttu-id="3707c-1972">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="3707c-1972">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="3707c-1973">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="3707c-1973">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="3707c-1974">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="3707c-1974">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="3707c-1975">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="3707c-1975">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-1976">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-1976">Appservice</span></span>

* <span data-ttu-id="3707c-1977">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="3707c-1977">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="3707c-1978">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="3707c-1978">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="3707c-1979">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="3707c-1979">Cognitive Services</span></span>

* <span data-ttu-id="3707c-1980">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="3707c-1980">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="3707c-1981">Consumo</span><span class="sxs-lookup"><span data-stu-id="3707c-1981">Consumption</span></span>

* <span data-ttu-id="3707c-1982">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="3707c-1982">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="3707c-1983">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="3707c-1983">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="3707c-1984">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-1984">Container</span></span>

* <span data-ttu-id="3707c-1985">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="3707c-1985">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="3707c-1986">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-1986">Network</span></span>

* <span data-ttu-id="3707c-1987">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="3707c-1987">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-1988">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-1988">Resource</span></span>

* <span data-ttu-id="3707c-1989">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="3707c-1989">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="3707c-1990">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-1990">Role</span></span>

* <span data-ttu-id="3707c-1991">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="3707c-1991">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-1992">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-1992">SQL</span></span>

* <span data-ttu-id="3707c-1993">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="3707c-1993">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-1994">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-1994">Storage</span></span>

* <span data-ttu-id="3707c-1995">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="3707c-1995">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-1996">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-1996">VM</span></span>

* <span data-ttu-id="3707c-1997">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="3707c-1997">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="3707c-1998">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-1998">February 13, 2018</span></span>

<span data-ttu-id="3707c-1999">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="3707c-1999">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="3707c-2000">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2000">Core</span></span>

* <span data-ttu-id="3707c-2001">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="3707c-2001">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2002">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2002">ACS</span></span>

* <span data-ttu-id="3707c-2003">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2003">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="3707c-2004">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2004">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="3707c-2005">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3707c-2005">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="3707c-2006">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-2006">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="3707c-2007">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="3707c-2007">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="3707c-2008">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="3707c-2008">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="3707c-2009">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3707c-2009">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="3707c-2010">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="3707c-2010">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2011">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2011">Appservice</span></span>

* <span data-ttu-id="3707c-2012">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="3707c-2012">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="3707c-2013">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="3707c-2013">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="3707c-2014">CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-2014">CDN</span></span>

* <span data-ttu-id="3707c-2015">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2015">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="3707c-2016">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-2016">Container</span></span>

* <span data-ttu-id="3707c-2017">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="3707c-2017">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="3707c-2018">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-2018">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-2019">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-2019">CosmosDB</span></span>

* <span data-ttu-id="3707c-2020">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="3707c-2020">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-2021">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-2021">Extension</span></span>

* <span data-ttu-id="3707c-2022">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2022">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="3707c-2023">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2023">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="3707c-2024">Comentarios</span><span class="sxs-lookup"><span data-stu-id="3707c-2024">Feedback</span></span>

* <span data-ttu-id="3707c-2025">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="3707c-2025">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-2026">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-2026">Interactive</span></span>

* <span data-ttu-id="3707c-2027">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="3707c-2027">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="3707c-2028">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="3707c-2028">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-2029">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-2029">IoT</span></span>

* <span data-ttu-id="3707c-2030">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2030">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="3707c-2031">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2031">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="3707c-2032">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2032">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="3707c-2033">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="3707c-2033">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-2034">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2034">Monitor</span></span>

* <span data-ttu-id="3707c-2035">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2035">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2036">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2036">Network</span></span>

* <span data-ttu-id="3707c-2037">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-2037">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="3707c-2038">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-2038">Profile</span></span>

* <span data-ttu-id="3707c-2039">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="3707c-2039">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2040">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2040">Resource</span></span>

* <span data-ttu-id="3707c-2041">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="3707c-2041">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="3707c-2042">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-2042">Role</span></span>

* <span data-ttu-id="3707c-2043">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2043">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2044">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-2044">SQL</span></span>

* <span data-ttu-id="3707c-2045">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2045">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="3707c-2046">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2046">Added `sql db rename`</span></span>
* <span data-ttu-id="3707c-2047">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="3707c-2047">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2048">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2048">Storage</span></span>

* <span data-ttu-id="3707c-2049">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="3707c-2049">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2050">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2050">VM</span></span>

* <span data-ttu-id="3707c-2051">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="3707c-2051">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="3707c-2052">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="3707c-2052">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="3707c-2053">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="3707c-2053">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="3707c-2054">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-2054">January 31, 2018</span></span>

<span data-ttu-id="3707c-2055">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="3707c-2055">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="3707c-2056">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2056">Core</span></span>

* <span data-ttu-id="3707c-2057">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="3707c-2057">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="3707c-2058">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="3707c-2058">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="3707c-2059">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="3707c-2059">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="3707c-2060">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="3707c-2060">Use `--verbose` to see</span></span>
* <span data-ttu-id="3707c-2061">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="3707c-2061">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2062">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2062">ACS</span></span>

* <span data-ttu-id="3707c-2063">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="3707c-2063">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="3707c-2064">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="3707c-2064">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2065">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2065">Appservice</span></span>

* <span data-ttu-id="3707c-2066">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="3707c-2066">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="3707c-2067">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="3707c-2067">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="3707c-2068">CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-2068">CDN</span></span>

* <span data-ttu-id="3707c-2069">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2069">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-2070">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-2070">CosmosDB</span></span>

* <span data-ttu-id="3707c-2071">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="3707c-2071">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-2072">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-2072">Interactive</span></span>

* <span data-ttu-id="3707c-2073">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="3707c-2073">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2074">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2074">Network</span></span>

* <span data-ttu-id="3707c-2075">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2075">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="3707c-2076">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="3707c-2076">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="3707c-2077">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2077">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="3707c-2078">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2078">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="3707c-2079">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="3707c-2079">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="3707c-2080">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="3707c-2080">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="3707c-2081">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="3707c-2081">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="3707c-2082">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="3707c-2082">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="3707c-2083">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="3707c-2083">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="3707c-2084">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="3707c-2084">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-2085">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-2085">Profile</span></span>

* <span data-ttu-id="3707c-2086">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="3707c-2086">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2087">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2087">Resource</span></span>

* <span data-ttu-id="3707c-2088">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="3707c-2088">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2089">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2089">Storage</span></span>

* <span data-ttu-id="3707c-2090">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="3707c-2090">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="3707c-2091">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="3707c-2091">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="3707c-2092">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="3707c-2092">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="3707c-2093">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2093">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="3707c-2094">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="3707c-2094">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2095">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2095">VM</span></span>

* <span data-ttu-id="3707c-2096">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="3707c-2096">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="3707c-2097">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="3707c-2097">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="3707c-2098">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="3707c-2098">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="3707c-2099">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2099">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="3707c-2100">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="3707c-2100">January 17, 2018</span></span>

<span data-ttu-id="3707c-2101">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="3707c-2101">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-2102">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-2102">ACR</span></span>

* <span data-ttu-id="3707c-2103">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="3707c-2103">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="3707c-2104">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="3707c-2104">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2105">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2105">ACS</span></span>

* <span data-ttu-id="3707c-2106">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="3707c-2106">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="3707c-2107">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="3707c-2107">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2108">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2108">Appservice</span></span>

* <span data-ttu-id="3707c-2109">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="3707c-2109">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="3707c-2110">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="3707c-2110">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="3707c-2111">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="3707c-2111">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="3707c-2112">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="3707c-2112">Backup</span></span>

* <span data-ttu-id="3707c-2113">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="3707c-2113">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="3707c-2114">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="3707c-2114">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="3707c-2115">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="3707c-2115">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="3707c-2116">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="3707c-2116">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="3707c-2117">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="3707c-2117">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-2118">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-2118">Batch</span></span>

* <span data-ttu-id="3707c-2119">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="3707c-2119">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="3707c-2120">Nube</span><span class="sxs-lookup"><span data-stu-id="3707c-2120">Cloud</span></span>

* <span data-ttu-id="3707c-2121">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="3707c-2121">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="3707c-2122">Consumo</span><span class="sxs-lookup"><span data-stu-id="3707c-2122">Consumption</span></span>

* <span data-ttu-id="3707c-2123">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="3707c-2123">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="3707c-2124">Event Grid</span><span class="sxs-lookup"><span data-stu-id="3707c-2124">Event Grid</span></span>

* <span data-ttu-id="3707c-2125">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="3707c-2125">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="3707c-2126">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="3707c-2126">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="3707c-2127">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2127">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="3707c-2128">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="3707c-2128">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="3707c-2129">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2129">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="3707c-2130">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2130">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="3707c-2131">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="3707c-2131">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="3707c-2132">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="3707c-2132">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-2133">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-2133">Interactive</span></span>

* <span data-ttu-id="3707c-2134">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="3707c-2134">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="3707c-2135">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="3707c-2135">Fixed errors on startup</span></span>
* <span data-ttu-id="3707c-2136">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="3707c-2136">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-2137">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-2137">IoT</span></span>

* <span data-ttu-id="3707c-2138">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="3707c-2138">Added support for device provisioning service</span></span>
* <span data-ttu-id="3707c-2139">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-2139">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="3707c-2140">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-2140">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-2141">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2141">Monitor</span></span>

* <span data-ttu-id="3707c-2142">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="3707c-2142">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="3707c-2143">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2143">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="3707c-2144">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="3707c-2144">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2145">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2145">Network</span></span>

* <span data-ttu-id="3707c-2146">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2146">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="3707c-2147">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2147">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-2148">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-2148">Profile</span></span>

* <span data-ttu-id="3707c-2149">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="3707c-2149">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="3707c-2150">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-2150">Role</span></span>

* <span data-ttu-id="3707c-2151">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="3707c-2151">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3707c-2152">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3707c-2152">Service Fabric</span></span>

* <span data-ttu-id="3707c-2153">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="3707c-2153">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="3707c-2154">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="3707c-2154">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2155">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2155">VM</span></span>

* <span data-ttu-id="3707c-2156">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="3707c-2156">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="3707c-2157">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="3707c-2157">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="3707c-2158">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="3707c-2158">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="3707c-2159">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="3707c-2159">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="3707c-2160">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="3707c-2160">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="3707c-2161">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2161">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="3707c-2162">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2162">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="3707c-2163">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="3707c-2163">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="3707c-2164">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2164">December 19, 2017</span></span>

<span data-ttu-id="3707c-2165">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="3707c-2165">Version 2.0.23</span></span>

* <span data-ttu-id="3707c-2166">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="3707c-2166">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="3707c-2167">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-2167">Container</span></span>

* <span data-ttu-id="3707c-2168">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-2168">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2169">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2169">Network</span></span>

* <span data-ttu-id="3707c-2170">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2170">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="3707c-2171">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2171">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2172">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2172">Storage</span></span>

* <span data-ttu-id="3707c-2173">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="3707c-2173">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2174">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2174">VM</span></span>

* <span data-ttu-id="3707c-2175">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="3707c-2175">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="3707c-2176">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2176">December 5, 2017</span></span>

<span data-ttu-id="3707c-2177">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="3707c-2177">Version 2.0.22</span></span>

* <span data-ttu-id="3707c-2178">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2178">Removed `az component` commands.</span></span> <span data-ttu-id="3707c-2179">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="3707c-2179">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="3707c-2180">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2180">Core</span></span>
* <span data-ttu-id="3707c-2181">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="3707c-2181">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="3707c-2182">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="3707c-2182">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2183">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2183">ACS</span></span>

* <span data-ttu-id="3707c-2184">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="3707c-2184">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="3707c-2185">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2185">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="3707c-2186">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="3707c-2186">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="3707c-2187">Advisor</span><span class="sxs-lookup"><span data-stu-id="3707c-2187">Advisor</span></span>

* <span data-ttu-id="3707c-2188">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="3707c-2188">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2189">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2189">Appservice</span></span>

* <span data-ttu-id="3707c-2190">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="3707c-2190">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="3707c-2191">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="3707c-2191">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="3707c-2192">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="3707c-2192">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="3707c-2193">Consumo</span><span class="sxs-lookup"><span data-stu-id="3707c-2193">Consumption</span></span>

* <span data-ttu-id="3707c-2194">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="3707c-2194">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="3707c-2195">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-2195">Container</span></span>

* <span data-ttu-id="3707c-2196">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="3707c-2196">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-2197">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2197">Monitor</span></span>

* <span data-ttu-id="3707c-2198">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="3707c-2198">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2199">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2199">Resource</span></span>

* <span data-ttu-id="3707c-2200">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="3707c-2200">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="3707c-2201">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-2201">Role</span></span>

* <span data-ttu-id="3707c-2202">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="3707c-2202">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="3707c-2203">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="3707c-2203">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="3707c-2204">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="3707c-2204">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2205">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-2205">SQL</span></span>

* <span data-ttu-id="3707c-2206">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="3707c-2206">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="3707c-2207">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2207">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2208">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2208">VM</span></span>

* <span data-ttu-id="3707c-2209">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="3707c-2209">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="3707c-2210">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2210">November 14, 2017</span></span>

<span data-ttu-id="3707c-2211">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="3707c-2211">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-2212">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-2212">ACR</span></span>

* <span data-ttu-id="3707c-2213">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="3707c-2213">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="3707c-2214">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2214">ACS</span></span>

* <span data-ttu-id="3707c-2215">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="3707c-2215">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="3707c-2216">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2216">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="3707c-2217">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="3707c-2217">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="3707c-2218">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="3707c-2218">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="3707c-2219">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="3707c-2219">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2220">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2220">Appservice</span></span>

* <span data-ttu-id="3707c-2221">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="3707c-2221">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="3707c-2222">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="3707c-2222">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="3707c-2223">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="3707c-2223">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="3707c-2224">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="3707c-2224">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="3707c-2225">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="3707c-2225">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="3707c-2226">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="3707c-2226">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-2227">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-2227">Batch</span></span>

* <span data-ttu-id="3707c-2228">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="3707c-2228">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="3707c-2229">Batchai</span><span class="sxs-lookup"><span data-stu-id="3707c-2229">Batchai</span></span>

* <span data-ttu-id="3707c-2230">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2230">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="3707c-2231">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2231">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="3707c-2232">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="3707c-2232">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="3707c-2233">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2233">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="3707c-2234">Nube</span><span class="sxs-lookup"><span data-stu-id="3707c-2234">Cloud</span></span>

* <span data-ttu-id="3707c-2235">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="3707c-2235">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="3707c-2236">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-2236">Container</span></span>

* <span data-ttu-id="3707c-2237">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="3707c-2237">Added support to open multiple ports</span></span>
* <span data-ttu-id="3707c-2238">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="3707c-2238">Added container group restart policy</span></span>
* <span data-ttu-id="3707c-2239">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="3707c-2239">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="3707c-2240">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="3707c-2240">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3707c-2241">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3707c-2241">Data Lake Analytics</span></span>

* <span data-ttu-id="3707c-2242">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="3707c-2242">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3707c-2243">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3707c-2243">Data Lake Store</span></span>

* <span data-ttu-id="3707c-2244">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="3707c-2244">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-2245">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-2245">Extension</span></span>

* <span data-ttu-id="3707c-2246">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="3707c-2246">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="3707c-2247">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="3707c-2247">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-2248">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-2248">IoT</span></span>

* <span data-ttu-id="3707c-2249">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="3707c-2249">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-2250">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2250">Monitor</span></span>

* <span data-ttu-id="3707c-2251">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2251">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2252">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2252">Network</span></span>

* <span data-ttu-id="3707c-2253">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="3707c-2253">Added support for CAA DNS records</span></span>
* <span data-ttu-id="3707c-2254">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2254">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="3707c-2255">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2255">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="3707c-2256">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="3707c-2256">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="3707c-2257">Reservations</span><span class="sxs-lookup"><span data-stu-id="3707c-2257">Reservations</span></span>

* <span data-ttu-id="3707c-2258">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="3707c-2258">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2259">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2259">Resource</span></span>

* <span data-ttu-id="3707c-2260">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-2260">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2261">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-2261">SQL</span></span>

* <span data-ttu-id="3707c-2262">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2262">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2263">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2263">Storage</span></span>

* <span data-ttu-id="3707c-2264">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="3707c-2264">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="3707c-2265">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="3707c-2265">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="3707c-2266">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="3707c-2266">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="3707c-2267">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="3707c-2267">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="3707c-2268">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2268">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="3707c-2269">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="3707c-2269">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="3707c-2270">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="3707c-2270">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2271">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2271">VM</span></span>

* <span data-ttu-id="3707c-2272">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="3707c-2272">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="3707c-2273">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="3707c-2273">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="3707c-2274">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="3707c-2274">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="3707c-2275">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2275">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="3707c-2276">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="3707c-2276">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="3707c-2277">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2277">October 24, 2017</span></span>

<span data-ttu-id="3707c-2278">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="3707c-2278">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="3707c-2279">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2279">Core</span></span>

* <span data-ttu-id="3707c-2280">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="3707c-2280">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-2281">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-2281">ACR</span></span>

* <span data-ttu-id="3707c-2282">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="3707c-2282">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="3707c-2283">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="3707c-2283">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="3707c-2284">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="3707c-2284">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2285">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2285">ACS</span></span>

* <span data-ttu-id="3707c-2286">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="3707c-2286">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="3707c-2287">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3707c-2287">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2288">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2288">Appservice</span></span>

* <span data-ttu-id="3707c-2289">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="3707c-2289">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="3707c-2290">Componente</span><span class="sxs-lookup"><span data-stu-id="3707c-2290">Component</span></span>

* <span data-ttu-id="3707c-2291">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="3707c-2291">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-2292">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2292">Monitor</span></span>

* <span data-ttu-id="3707c-2293">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2293">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2294">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2294">Resource</span></span>

* <span data-ttu-id="3707c-2295">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="3707c-2295">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="3707c-2296">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="3707c-2296">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2297">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2297">VM</span></span>

* <span data-ttu-id="3707c-2298">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2298">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="3707c-2299">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2299">October 9, 2017</span></span>

<span data-ttu-id="3707c-2300">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="3707c-2300">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="3707c-2301">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2301">Core</span></span>

* <span data-ttu-id="3707c-2302">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="3707c-2302">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2303">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2303">Appservice</span></span>

* <span data-ttu-id="3707c-2304">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2304">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-2305">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-2305">Batch</span></span>

* <span data-ttu-id="3707c-2306">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="3707c-2306">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="3707c-2307">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="3707c-2307">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="3707c-2308">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-2308">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="3707c-2309">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="3707c-2309">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="3707c-2310">Batchai</span><span class="sxs-lookup"><span data-stu-id="3707c-2310">Batchai</span></span>

* <span data-ttu-id="3707c-2311">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-2311">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-2312">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3707c-2312">Keyvault</span></span>

* <span data-ttu-id="3707c-2313">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3707c-2313">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="3707c-2314">(#4448)</span><span class="sxs-lookup"><span data-stu-id="3707c-2314">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="3707c-2315">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2315">Network</span></span>

* <span data-ttu-id="3707c-2316">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="3707c-2316">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="3707c-2317">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="3707c-2317">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2318">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2318">Resource</span></span>

* <span data-ttu-id="3707c-2319">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-2319">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="3707c-2320">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="3707c-2320">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="3707c-2321">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="3707c-2321">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="3707c-2322">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="3707c-2322">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2323">Sql</span><span class="sxs-lookup"><span data-stu-id="3707c-2323">Sql</span></span>

* <span data-ttu-id="3707c-2324">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="3707c-2324">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="3707c-2325">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="3707c-2325">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="3707c-2326">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="3707c-2326">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2327">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2327">Storage</span></span>

* <span data-ttu-id="3707c-2328">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="3707c-2328">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2329">Vm</span><span class="sxs-lookup"><span data-stu-id="3707c-2329">Vm</span></span>

* <span data-ttu-id="3707c-2330">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="3707c-2330">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="3707c-2331">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2331">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="3707c-2332">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="3707c-2332">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="3707c-2333">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2333">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="3707c-2334">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2334">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="3707c-2335">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2335">September 22, 2017</span></span>

<span data-ttu-id="3707c-2336">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="3707c-2336">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2337">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2337">Resource</span></span>

* <span data-ttu-id="3707c-2338">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="3707c-2338">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="3707c-2339">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="3707c-2339">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="3707c-2340">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2340">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="3707c-2341">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="3707c-2341">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2342">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2342">Network</span></span>

* <span data-ttu-id="3707c-2343">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="3707c-2343">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="3707c-2344">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="3707c-2344">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="3707c-2345">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="3707c-2345">Added `asg` application security group commands</span></span>
* <span data-ttu-id="3707c-2346">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2346">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="3707c-2347">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2347">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3707c-2348">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2348">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="3707c-2349">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2349">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2350">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2350">Storage</span></span>

* <span data-ttu-id="3707c-2351">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="3707c-2351">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3707c-2352">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="3707c-2352">Eventgrid</span></span>

* <span data-ttu-id="3707c-2353">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="3707c-2353">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2354">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-2354">SQL</span></span>

* <span data-ttu-id="3707c-2355">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="3707c-2355">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="3707c-2356">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="3707c-2356">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="3707c-2357">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2357">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-2358">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3707c-2358">Keyvault</span></span>

* <span data-ttu-id="3707c-2359">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="3707c-2359">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2360">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2360">VM</span></span>

* <span data-ttu-id="3707c-2361">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2361">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="3707c-2362">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="3707c-2362">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="3707c-2363">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2363">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="3707c-2364">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="3707c-2364">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="3707c-2365">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="3707c-2365">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="3707c-2366">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="3707c-2366">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2367">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2367">ACS</span></span>

* <span data-ttu-id="3707c-2368">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2368">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2369">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2369">Appservice</span></span>

* <span data-ttu-id="3707c-2370">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2370">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="3707c-2371">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="3707c-2371">Backup</span></span>

* <span data-ttu-id="3707c-2372">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-2372">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="3707c-2373">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2373">September 11, 2017</span></span>

<span data-ttu-id="3707c-2374">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="3707c-2374">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="3707c-2375">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2375">Core</span></span>

* <span data-ttu-id="3707c-2376">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="3707c-2376">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="3707c-2377">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="3707c-2377">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2378">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2378">Acs</span></span>

* <span data-ttu-id="3707c-2379">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2379">Added `acs list-locations` command</span></span>
* <span data-ttu-id="3707c-2380">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="3707c-2380">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2381">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2381">Appservice</span></span>

* <span data-ttu-id="3707c-2382">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="3707c-2382">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="3707c-2383">CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-2383">CDN</span></span>

* <span data-ttu-id="3707c-2384">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2384">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="3707c-2385">Extensión</span><span class="sxs-lookup"><span data-stu-id="3707c-2385">Extension</span></span>

* <span data-ttu-id="3707c-2386">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="3707c-2386">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-2387">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3707c-2387">Keyvault</span></span>

* <span data-ttu-id="3707c-2388">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="3707c-2388">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2389">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2389">Network</span></span>

* <span data-ttu-id="3707c-2390">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2390">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3707c-2391">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2391">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="3707c-2392">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2392">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="3707c-2393">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2393">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3707c-2394">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2394">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2395">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2395">Resource</span></span>

* <span data-ttu-id="3707c-2396">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2396">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="3707c-2397">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2397">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="3707c-2398">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="3707c-2398">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="3707c-2399">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="3707c-2399">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2400">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-2400">SQL</span></span>

* <span data-ttu-id="3707c-2401">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2401">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2402">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2402">VM</span></span>

* <span data-ttu-id="3707c-2403">Problema corregido: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2403">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="3707c-2404">Problema corregido: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="3707c-2404">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="3707c-2405">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2405">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="3707c-2406">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="3707c-2406">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="3707c-2407">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2407">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="3707c-2408">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2408">August 31, 2017</span></span>

<span data-ttu-id="3707c-2409">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="3707c-2409">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-2410">Keyvault</span><span class="sxs-lookup"><span data-stu-id="3707c-2410">Keyvault</span></span>

* <span data-ttu-id="3707c-2411">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2411">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="3707c-2412">Sf</span><span class="sxs-lookup"><span data-stu-id="3707c-2412">Sf</span></span>

* <span data-ttu-id="3707c-2413">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="3707c-2413">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2414">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2414">Storage</span></span>

* <span data-ttu-id="3707c-2415">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="3707c-2415">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="3707c-2416">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="3707c-2416">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="3707c-2417">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2417">August 28, 2017</span></span>

<span data-ttu-id="3707c-2418">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="3707c-2418">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="3707c-2419">CLI</span><span class="sxs-lookup"><span data-stu-id="3707c-2419">CLI</span></span>

* <span data-ttu-id="3707c-2420">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="3707c-2420">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2421">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2421">ACS</span></span>

* <span data-ttu-id="3707c-2422">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-2422">Corrected preview regions</span></span>
* <span data-ttu-id="3707c-2423">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="3707c-2423">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="3707c-2424">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="3707c-2424">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2425">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2425">Appservice</span></span>

* <span data-ttu-id="3707c-2426">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2426">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="3707c-2427">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2427">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="3707c-2428">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2428">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="3707c-2429">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="3707c-2429">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="3707c-2430">Problema corregido: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="3707c-2430">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-2431">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-2431">IoT</span></span>

* <span data-ttu-id="3707c-2432">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="3707c-2432">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2433">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2433">Network</span></span>

* <span data-ttu-id="3707c-2434">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="3707c-2434">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3707c-2435">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3707c-2435">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="3707c-2436">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2436">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3707c-2437">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2437">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3707c-2438">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2438">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-2439">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-2439">Profile</span></span>

* <span data-ttu-id="3707c-2440">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="3707c-2440">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3707c-2441">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3707c-2441">Service Fabric</span></span>

* <span data-ttu-id="3707c-2442">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-2442">Preview release</span></span>
* <span data-ttu-id="3707c-2443">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="3707c-2443">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="3707c-2444">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="3707c-2444">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="3707c-2445">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2445">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2446">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2446">Storage</span></span>

* <span data-ttu-id="3707c-2447">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="3707c-2447">Enabled setting blob tier</span></span>
* <span data-ttu-id="3707c-2448">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="3707c-2448">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="3707c-2449">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2449">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="3707c-2450">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="3707c-2450">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="3707c-2451">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="3707c-2451">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="3707c-2452">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="3707c-2452">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2453">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2453">VM</span></span>

* <span data-ttu-id="3707c-2454">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2454">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="3707c-2455">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2455">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="3707c-2456">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2456">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="3707c-2457">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="3707c-2457">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="3707c-2458">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="3707c-2458">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="3707c-2459">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2459">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="3707c-2460">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2460">August 15, 2017</span></span>

<span data-ttu-id="3707c-2461">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="3707c-2461">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2462">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2462">ACS</span></span>

* <span data-ttu-id="3707c-2463">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="3707c-2463">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2464">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2464">Appservice</span></span>

* <span data-ttu-id="3707c-2465">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="3707c-2465">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="3707c-2466">Event Grid</span><span class="sxs-lookup"><span data-stu-id="3707c-2466">Event Grid</span></span>

* <span data-ttu-id="3707c-2467">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="3707c-2467">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="3707c-2468">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2468">August 11, 2017</span></span>

<span data-ttu-id="3707c-2469">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="3707c-2469">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2470">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2470">ACS</span></span>

* <span data-ttu-id="3707c-2471">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-2471">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-2472">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-2472">Batch</span></span>

* <span data-ttu-id="3707c-2473">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="3707c-2473">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="3707c-2474">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="3707c-2474">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="3707c-2475">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="3707c-2475">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="3707c-2476">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="3707c-2476">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="3707c-2477">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="3707c-2477">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="3707c-2478">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="3707c-2478">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="3707c-2479">Componente</span><span class="sxs-lookup"><span data-stu-id="3707c-2479">Component</span></span>

* <span data-ttu-id="3707c-2480">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="3707c-2480">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="3707c-2481">Contenedor</span><span class="sxs-lookup"><span data-stu-id="3707c-2481">Container</span></span>

* <span data-ttu-id="3707c-2482">`create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="3707c-2482">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="3707c-2483">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3707c-2483">Data Lake Store</span></span>

* <span data-ttu-id="3707c-2484">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="3707c-2484">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="3707c-2485">Event Grid</span><span class="sxs-lookup"><span data-stu-id="3707c-2485">Event Grid</span></span>

* <span data-ttu-id="3707c-2486">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="3707c-2486">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2487">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2487">Network</span></span>

* <span data-ttu-id="3707c-2488">`lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="3707c-2488">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="3707c-2489">`application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2489">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="3707c-2490">`application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="3707c-2490">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="3707c-2491">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2491">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-2492">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-2492">Profile</span></span>

* <span data-ttu-id="3707c-2493">`account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="3707c-2493">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2494">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2494">Storage</span></span>

* <span data-ttu-id="3707c-2495">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="3707c-2495">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2496">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2496">VM</span></span>

* <span data-ttu-id="3707c-2497">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="3707c-2497">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="3707c-2498">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2498">Exposed `list-skus` command</span></span>
* <span data-ttu-id="3707c-2499">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="3707c-2499">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="3707c-2500">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="3707c-2500">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="3707c-2501">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="3707c-2501">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="3707c-2502">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2502">July 28, 2017</span></span>

<span data-ttu-id="3707c-2503">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="3707c-2503">Version 2.0.12</span></span>

* <span data-ttu-id="3707c-2504">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="3707c-2504">Added container commands</span></span>
* <span data-ttu-id="3707c-2505">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="3707c-2505">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="3707c-2506">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2506">Core</span></span>

* <span data-ttu-id="3707c-2507">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="3707c-2507">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="3707c-2508">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="3707c-2508">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="3707c-2509">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="3707c-2509">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="3707c-2510">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="3707c-2510">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="3707c-2511">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="3707c-2511">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="3707c-2512">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="3707c-2512">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="3707c-2513">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="3707c-2513">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3707c-2514">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="3707c-2514">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="3707c-2515">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="3707c-2515">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="3707c-2516">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="3707c-2516">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="3707c-2517">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="3707c-2517">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="3707c-2518">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="3707c-2518">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="3707c-2519">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2519">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="3707c-2520">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2520">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="3707c-2521">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3707c-2521">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="3707c-2522">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="3707c-2522">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="3707c-2523">ACR</span><span class="sxs-lookup"><span data-stu-id="3707c-2523">ACR</span></span>

* <span data-ttu-id="3707c-2524">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="3707c-2524">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="3707c-2525">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="3707c-2525">Support SKU update for managed registries</span></span>
* <span data-ttu-id="3707c-2526">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2526">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="3707c-2527">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="3707c-2527">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="3707c-2528">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="3707c-2528">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="3707c-2529">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="3707c-2529">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2530">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2530">ACS</span></span>

* <span data-ttu-id="3707c-2531">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="3707c-2531">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2532">Appservice</span><span class="sxs-lookup"><span data-stu-id="3707c-2532">Appservice</span></span>

* <span data-ttu-id="3707c-2533">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="3707c-2533">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="3707c-2534">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="3707c-2534">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="3707c-2535">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2535">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="3707c-2536">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="3707c-2536">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="3707c-2537">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="3707c-2537">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="3707c-2538">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="3707c-2538">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="3707c-2539">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="3707c-2539">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="3707c-2540">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="3707c-2540">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="3707c-2541">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="3707c-2541">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="3707c-2542">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="3707c-2542">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="3707c-2543">Batch</span><span class="sxs-lookup"><span data-stu-id="3707c-2543">Batch</span></span>

* <span data-ttu-id="3707c-2544">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="3707c-2544">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="3707c-2545">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2545">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="3707c-2546">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2546">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="3707c-2547">CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-2547">CDN</span></span>

* <span data-ttu-id="3707c-2548">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="3707c-2548">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="3707c-2549">Nube</span><span class="sxs-lookup"><span data-stu-id="3707c-2549">Cloud</span></span>

* <span data-ttu-id="3707c-2550">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="3707c-2550">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="3707c-2551">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="3707c-2551">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="3707c-2552">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="3707c-2552">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="3707c-2553">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="3707c-2553">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="3707c-2554">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2554">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-2555">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-2555">CosmosDB</span></span>

* <span data-ttu-id="3707c-2556">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="3707c-2556">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="3707c-2557">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="3707c-2557">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3707c-2558">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3707c-2558">Data Lake Analytics</span></span>

* <span data-ttu-id="3707c-2559">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2559">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="3707c-2560">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2560">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="3707c-2561">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2561">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3707c-2562">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3707c-2562">Data Lake Store</span></span>

* <span data-ttu-id="3707c-2563">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2563">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="3707c-2564">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="3707c-2564">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="3707c-2565">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2565">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="3707c-2566">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="3707c-2566">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="3707c-2567">Interactive</span><span class="sxs-lookup"><span data-stu-id="3707c-2567">Interactive</span></span>

* <span data-ttu-id="3707c-2568">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="3707c-2568">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="3707c-2569">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2569">Increased test coverage</span></span>
* <span data-ttu-id="3707c-2570">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="3707c-2570">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="3707c-2571">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="3707c-2571">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="3707c-2572">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="3707c-2572">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="3707c-2573">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="3707c-2573">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="3707c-2574">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="3707c-2574">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3707c-2575">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2575">Added `--progress` flag</span></span>
* <span data-ttu-id="3707c-2576">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="3707c-2576">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="3707c-2577">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="3707c-2577">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="3707c-2578">IoT</span><span class="sxs-lookup"><span data-stu-id="3707c-2578">IoT</span></span>

* <span data-ttu-id="3707c-2579">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="3707c-2579">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="3707c-2580">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="3707c-2580">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="3707c-2581">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="3707c-2581">Key vault</span></span>

* <span data-ttu-id="3707c-2582">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="3707c-2582">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="3707c-2583">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="3707c-2583">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="3707c-2584">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="3707c-2584">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3707c-2585">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="3707c-2585">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3707c-2586">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="3707c-2586">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="3707c-2587">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="3707c-2587">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="3707c-2588">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="3707c-2588">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="3707c-2589">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="3707c-2589">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="3707c-2590">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-2590">Lab</span></span>

* <span data-ttu-id="3707c-2591">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2591">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="3707c-2592">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2592">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-2593">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2593">Monitor</span></span>

* <span data-ttu-id="3707c-2594">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="3707c-2594">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="3707c-2595">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2595">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="3707c-2596">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2596">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="3707c-2597">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2597">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="3707c-2598">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2598">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="3707c-2599">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="3707c-2599">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="3707c-2600">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="3707c-2600">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="3707c-2601">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2601">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="3707c-2602">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="3707c-2602">`location` no longer required</span></span>
  * <span data-ttu-id="3707c-2603">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="3707c-2603">Add name and ID support for target</span></span>
  * <span data-ttu-id="3707c-2604">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2604">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="3707c-2605">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="3707c-2605">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="3707c-2606">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="3707c-2606">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="3707c-2607">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="3707c-2607">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="3707c-2608">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2608">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="3707c-2609">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="3707c-2609">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2610">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2610">Network</span></span>

* <span data-ttu-id="3707c-2611">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2611">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="3707c-2612">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2612">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="3707c-2613">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="3707c-2613">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="3707c-2614">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="3707c-2614">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="3707c-2615">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2615">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="3707c-2616">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2616">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="3707c-2617">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="3707c-2617">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="3707c-2618">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="3707c-2618">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="3707c-2619">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="3707c-2619">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="3707c-2620">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="3707c-2620">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="3707c-2621">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2621">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="3707c-2622">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2622">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="3707c-2623">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="3707c-2623">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="3707c-2624">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2624">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="3707c-2625">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2625">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="3707c-2626">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2626">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="3707c-2627">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="3707c-2627">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="3707c-2628">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2628">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="3707c-2629">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2629">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="3707c-2630">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2630">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="3707c-2631">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2631">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="3707c-2632">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2632">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="3707c-2633">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2633">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="3707c-2634">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="3707c-2634">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="3707c-2635">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="3707c-2635">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="3707c-2636">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="3707c-2636">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="3707c-2637">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="3707c-2637">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-2638">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-2638">Profile</span></span>

* <span data-ttu-id="3707c-2639">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="3707c-2639">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="3707c-2640">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="3707c-2640">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="3707c-2641">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="3707c-2641">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="3707c-2642">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="3707c-2642">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="3707c-2643">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="3707c-2643">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="3707c-2644">RDBMS</span><span class="sxs-lookup"><span data-stu-id="3707c-2644">RDBMS</span></span>

* <span data-ttu-id="3707c-2645">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="3707c-2645">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="3707c-2646">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="3707c-2646">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="3707c-2647">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="3707c-2647">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="3707c-2648">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="3707c-2648">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2649">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2649">Resource</span></span>

* <span data-ttu-id="3707c-2650">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2650">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="3707c-2651">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2651">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="3707c-2652">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2652">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="3707c-2653">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2653">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="3707c-2654">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="3707c-2654">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="3707c-2655">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2655">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="3707c-2656">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="3707c-2656">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="3707c-2657">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2657">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="3707c-2658">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-2658">Role</span></span>

* <span data-ttu-id="3707c-2659">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="3707c-2659">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="3707c-2660">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="3707c-2660">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="3707c-2661">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2661">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="3707c-2662">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2662">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="3707c-2663">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2663">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3707c-2664">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3707c-2664">Service Fabric</span></span>
* <span data-ttu-id="3707c-2665">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="3707c-2665">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="3707c-2666">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="3707c-2666">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="3707c-2667">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="3707c-2667">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2668">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-2668">SQL</span></span>

* <span data-ttu-id="3707c-2669">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="3707c-2669">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="3707c-2670">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2670">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="3707c-2671">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="3707c-2671">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2672">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2672">Storage</span></span>

* <span data-ttu-id="3707c-2673">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="3707c-2673">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="3707c-2674">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="3707c-2674">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="3707c-2675">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="3707c-2675">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="3707c-2676">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="3707c-2676">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="3707c-2677">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="3707c-2677">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="3707c-2678">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="3707c-2678">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2679">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2679">VM</span></span>

* <span data-ttu-id="3707c-2680">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="3707c-2680">Support configuring nsg</span></span>
* <span data-ttu-id="3707c-2681">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="3707c-2681">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="3707c-2682">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="3707c-2682">Support managed service identities</span></span>
* <span data-ttu-id="3707c-2683">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="3707c-2683">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="3707c-2684">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="3707c-2684">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="3707c-2685">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2685">May 10, 2017</span></span>

<span data-ttu-id="3707c-2686">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="3707c-2686">Version 2.0.6</span></span>

* <span data-ttu-id="3707c-2687">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="3707c-2687">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="3707c-2688">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="3707c-2688">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="3707c-2689">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3707c-2689">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="3707c-2690">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="3707c-2690">Include Cognitive Services module</span></span>
* <span data-ttu-id="3707c-2691">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3707c-2691">Include Service Fabric module</span></span>
* <span data-ttu-id="3707c-2692">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="3707c-2692">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="3707c-2693">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="3707c-2693">Add support for CDN commands</span></span>
* <span data-ttu-id="3707c-2694">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="3707c-2694">Remove Container module</span></span>
* <span data-ttu-id="3707c-2695">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="3707c-2695">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="3707c-2696">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="3707c-2696">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="3707c-2697">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2697">Core</span></span>

* <span data-ttu-id="3707c-2698">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="3707c-2698">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="3707c-2699">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="3707c-2699">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="3707c-2700">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="3707c-2700">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="3707c-2701">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="3707c-2701">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="3707c-2702">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="3707c-2702">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="3707c-2703">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="3707c-2703">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="3707c-2704">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="3707c-2704">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="3707c-2705">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="3707c-2705">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="3707c-2706">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="3707c-2706">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="3707c-2707">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="3707c-2707">core: Improved performance</span></span>
* <span data-ttu-id="3707c-2708">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="3707c-2708">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="3707c-2709">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="3707c-2709">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2710">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2710">ACS</span></span>

* <span data-ttu-id="3707c-2711">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="3707c-2711">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="3707c-2712">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="3707c-2712">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="3707c-2713">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="3707c-2713">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="3707c-2714">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="3707c-2714">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2715">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-2715">AppService</span></span>

* <span data-ttu-id="3707c-2716">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="3707c-2716">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="3707c-2717">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="3707c-2717">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="3707c-2718">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="3707c-2718">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="3707c-2719">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="3707c-2719">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="3707c-2720">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="3707c-2720">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="3707c-2721">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="3707c-2721">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="3707c-2722">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="3707c-2722">support slot swap with preview</span></span>
* <span data-ttu-id="3707c-2723">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="3707c-2723">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="3707c-2724">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="3707c-2724">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3707c-2725">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-2725">CosmosDB</span></span>

* <span data-ttu-id="3707c-2726">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="3707c-2726">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="3707c-2727">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="3707c-2727">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="3707c-2728">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="3707c-2728">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="3707c-2729">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="3707c-2729">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3707c-2730">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3707c-2730">Data Lake Analytics</span></span>

* <span data-ttu-id="3707c-2731">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="3707c-2731">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="3707c-2732">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="3707c-2732">Add support for new catalog item type: package.</span></span> <span data-ttu-id="3707c-2733">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="3707c-2733">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="3707c-2734">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="3707c-2734">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="3707c-2735">Tabla</span><span class="sxs-lookup"><span data-stu-id="3707c-2735">Table</span></span>
  * <span data-ttu-id="3707c-2736">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="3707c-2736">Table valued function</span></span>
  * <span data-ttu-id="3707c-2737">Ver</span><span class="sxs-lookup"><span data-stu-id="3707c-2737">View</span></span>
  * <span data-ttu-id="3707c-2738">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="3707c-2738">Table Statistics.</span></span> <span data-ttu-id="3707c-2739">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="3707c-2739">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3707c-2740">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3707c-2740">Data Lake Store</span></span>

* <span data-ttu-id="3707c-2741">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="3707c-2741">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="3707c-2742">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="3707c-2742">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="3707c-2743">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="3707c-2743">missed help for access show.</span></span> <span data-ttu-id="3707c-2744">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="3707c-2744">adding it.</span></span> <span data-ttu-id="3707c-2745">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="3707c-2745">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="3707c-2746">Buscar</span><span class="sxs-lookup"><span data-stu-id="3707c-2746">Find</span></span>

* <span data-ttu-id="3707c-2747">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="3707c-2747">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="3707c-2748">KeyVault</span><span class="sxs-lookup"><span data-stu-id="3707c-2748">KeyVault</span></span>

* <span data-ttu-id="3707c-2749">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="3707c-2749">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="3707c-2750">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="3707c-2750">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="3707c-2751">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="3707c-2751">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="3707c-2752">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="3707c-2752">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="3707c-2753">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="3707c-2753">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="3707c-2754">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-2754">Lab</span></span>

* <span data-ttu-id="3707c-2755">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-2755">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="3707c-2756">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-2756">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="3707c-2757">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-2757">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="3707c-2758">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-2758">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="3707c-2759">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="3707c-2759">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="3707c-2760">Supervisión</span><span class="sxs-lookup"><span data-stu-id="3707c-2760">Monitor</span></span>

* <span data-ttu-id="3707c-2761">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="3707c-2761">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="3707c-2762">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="3707c-2762">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="3707c-2763">Red</span><span class="sxs-lookup"><span data-stu-id="3707c-2763">Network</span></span>

* <span data-ttu-id="3707c-2764">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="3707c-2764">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="3707c-2765">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2765">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="3707c-2766">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="3707c-2766">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="3707c-2767">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="3707c-2767">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="3707c-2768">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="3707c-2768">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="3707c-2769">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="3707c-2769">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="3707c-2770">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="3707c-2770">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="3707c-2771">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="3707c-2771">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="3707c-2772">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="3707c-2772">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="3707c-2773">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="3707c-2773">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="3707c-2774">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="3707c-2774">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="3707c-2775">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2775">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="3707c-2776">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="3707c-2776">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="3707c-2777">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="3707c-2777">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="3707c-2778">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="3707c-2778">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="3707c-2779">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="3707c-2779">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="3707c-2780">Perfil</span><span class="sxs-lookup"><span data-stu-id="3707c-2780">Profile</span></span>

* <span data-ttu-id="3707c-2781">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="3707c-2781">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="3707c-2782">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="3707c-2782">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="3707c-2783">Redis</span><span class="sxs-lookup"><span data-stu-id="3707c-2783">Redis</span></span>

* <span data-ttu-id="3707c-2784">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="3707c-2784">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="3707c-2785">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="3707c-2785">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="3707c-2786">Resource</span><span class="sxs-lookup"><span data-stu-id="3707c-2786">Resource</span></span>

* <span data-ttu-id="3707c-2787">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="3707c-2787">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="3707c-2788">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="3707c-2788">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="3707c-2789">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="3707c-2789">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="3707c-2790">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="3707c-2790">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="3707c-2791">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="3707c-2791">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="3707c-2792">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="3707c-2792">Add docs for az lock update.</span></span> <span data-ttu-id="3707c-2793">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="3707c-2793">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="3707c-2794">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="3707c-2794">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="3707c-2795">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="3707c-2795">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="3707c-2796">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="3707c-2796">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="3707c-2797">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="3707c-2797">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="3707c-2798">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="3707c-2798">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="3707c-2799">Role</span><span class="sxs-lookup"><span data-stu-id="3707c-2799">Role</span></span>

* <span data-ttu-id="3707c-2800">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="3707c-2800">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="3707c-2801">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="3707c-2801">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="3707c-2802">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="3707c-2802">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="3707c-2803">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="3707c-2803">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="3707c-2804">SQL</span><span class="sxs-lookup"><span data-stu-id="3707c-2804">SQL</span></span>

* <span data-ttu-id="3707c-2805">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="3707c-2805">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="3707c-2806">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="3707c-2806">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="3707c-2807">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2807">Storage</span></span>

* <span data-ttu-id="3707c-2808">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="3707c-2808">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="3707c-2809">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="3707c-2809">Add support for incremental blob copy</span></span>
* <span data-ttu-id="3707c-2810">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="3707c-2810">Add support for large block blob upload</span></span>
* <span data-ttu-id="3707c-2811">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="3707c-2811">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2812">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2812">VM</span></span>

* <span data-ttu-id="3707c-2813">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="3707c-2813">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="3707c-2814">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="3707c-2814">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="3707c-2815">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="3707c-2815">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="3707c-2816">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="3707c-2816">az vm/vmss disk</span></span>
  3. <span data-ttu-id="3707c-2817">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="3707c-2817">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="3707c-2818">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="3707c-2818">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="3707c-2819">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="3707c-2819">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="3707c-2820">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2820">April 3, 2017</span></span>

<span data-ttu-id="3707c-2821">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="3707c-2821">Version 2.0.2</span></span>

<span data-ttu-id="3707c-2822">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="3707c-2822">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="3707c-2823">Core</span><span class="sxs-lookup"><span data-stu-id="3707c-2823">Core</span></span>

* <span data-ttu-id="3707c-2824">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="3707c-2824">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="3707c-2825">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="3707c-2825">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="3707c-2826">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="3707c-2826">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="3707c-2827">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="3707c-2827">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3707c-2828">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="3707c-2828">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="3707c-2829">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="3707c-2829">Add prompting for missing template parameters.</span></span> <span data-ttu-id="3707c-2830">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="3707c-2830">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="3707c-2831">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="3707c-2831">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="3707c-2832">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="3707c-2832">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="3707c-2833">ACS</span><span class="sxs-lookup"><span data-stu-id="3707c-2833">ACS</span></span>

* <span data-ttu-id="3707c-2834">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="3707c-2834">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="3707c-2835">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="3707c-2835">Add support for ssh key password prompting.</span></span> <span data-ttu-id="3707c-2836">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="3707c-2836">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="3707c-2837">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="3707c-2837">Add support for windows clusters.</span></span> <span data-ttu-id="3707c-2838">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="3707c-2838">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="3707c-2839">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="3707c-2839">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="3707c-2840">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="3707c-2840">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="3707c-2841">AppService</span><span class="sxs-lookup"><span data-stu-id="3707c-2841">AppService</span></span>

* <span data-ttu-id="3707c-2842">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="3707c-2842">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="3707c-2843">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="3707c-2843">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="3707c-2844">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="3707c-2844">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="3707c-2845">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="3707c-2845">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="3707c-2846">DataLake</span><span class="sxs-lookup"><span data-stu-id="3707c-2846">DataLake</span></span>

* <span data-ttu-id="3707c-2847">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3707c-2847">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="3707c-2848">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3707c-2848">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="3707c-2849">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="3707c-2849">DocuemntDB</span></span>

* <span data-ttu-id="3707c-2850">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="3707c-2850">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="3707c-2851">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="3707c-2851">VM</span></span>

* <span data-ttu-id="3707c-2852">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="3707c-2852">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="3707c-2853">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="3707c-2853">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="3707c-2854">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="3707c-2854">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="3707c-2855">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="3707c-2855">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3707c-2856">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="3707c-2856">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="3707c-2857">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="3707c-2857">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="3707c-2858">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="3707c-2858">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="3707c-2859">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="3707c-2859">February 27, 2017</span></span>

<span data-ttu-id="3707c-2860">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="3707c-2860">Version 2.0.0</span></span>

<span data-ttu-id="3707c-2861">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="3707c-2861">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="3707c-2862">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="3707c-2862">Container Service (acs)</span></span>
- <span data-ttu-id="3707c-2863">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="3707c-2863">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="3707c-2864">Redes</span><span class="sxs-lookup"><span data-stu-id="3707c-2864">Networking</span></span>
- <span data-ttu-id="3707c-2865">Storage</span><span class="sxs-lookup"><span data-stu-id="3707c-2865">Storage</span></span>

<span data-ttu-id="3707c-2866">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="3707c-2866">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="3707c-2867">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="3707c-2867">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="3707c-2868">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="3707c-2868">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="3707c-2869">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="3707c-2869">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="3707c-2870">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="3707c-2870">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="3707c-2871">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="3707c-2871">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="3707c-2872">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="3707c-2872">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="3707c-2873">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="3707c-2873">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="3707c-2874">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="3707c-2874">Provide feedback from the command line with the `az feedback` command</span></span>

