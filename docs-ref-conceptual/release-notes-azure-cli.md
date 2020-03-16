---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/10/2020
ms.topic: article
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ff3a1da2343b96bfd78b20742c2c15707932f3d7
ms.sourcegitcommit: 21bc2a7125b6c38bf1c4def0a0e66e6673de4805
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/10/2020
ms.locfileid: "79037955"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="9fd5f-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="9fd5f-103">Azure CLI release notes</span></span>

## <a name="march-10-2020"></a><span data-ttu-id="9fd5f-104">10 de marzo de 2020</span><span class="sxs-lookup"><span data-stu-id="9fd5f-104">March 10, 2020</span></span>

<span data-ttu-id="9fd5f-105">Versión 2.2.0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-105">Version 2.2.0</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-106">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-106">ACR</span></span>

* <span data-ttu-id="9fd5f-107">Corrección: `az acr login` generaba un error incorrectamente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-107">Fix: `az acr login` wrongly raise error</span></span>
* <span data-ttu-id="9fd5f-108">Se ha agregado un nuevo comando `az acr helm install-cli`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-108">Add new command `az acr helm install-cli`</span></span>
* <span data-ttu-id="9fd5f-109">Se ha agregado compatibilidad con vínculos privados y CMK.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-109">Add private link and CMK support</span></span>
* <span data-ttu-id="9fd5f-110">Se ha agregado el comando "private-link-resource list".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-110">add 'private-link-resource list' command</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-111">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-111">AKS</span></span>

* <span data-ttu-id="9fd5f-112">Se ha corregido la exploración de AKS en Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-112">fix the aks browse in cloud shell</span></span>
* <span data-ttu-id="9fd5f-113">az aks: se han corregido los errores del complemento de supervisión y agentpool NoneType.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-113">az aks: Fix monitoring addon and agentpool NoneType errors</span></span>
* <span data-ttu-id="9fd5f-114">Se ha agregado --nodepool-tags al grupo de nodos al crear el clúster de Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-114">Add --nodepool-tags to node pool when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="9fd5f-115">Se ha agregado -tags al agregar o actualizar un grupo de nodos en el clúster.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-115">Add --tags when adding or updating a nodepool to cluster</span></span>
* <span data-ttu-id="9fd5f-116">aks create: se ha agregado`--enable-private-cluster`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-116">aks create: add `--enable-private-cluster`</span></span>
* <span data-ttu-id="9fd5f-117">Se ha agregado --nodepool-labels al crear el clúter de Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-117">add --nodepool-labels when creating azure kubernetes cluster</span></span>
* <span data-ttu-id="9fd5f-118">Se ha agregado -labels al agregar un nuevo grupo de nodos al clúster de Azure Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-118">add --labels when adding a new nodepool to azure kubernetes cluster</span></span>
* <span data-ttu-id="9fd5f-119">Se ha agregado la barra / que faltaba en la dirección URL del panel.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-119">add missing / in the dashboard url</span></span>
* <span data-ttu-id="9fd5f-120">Se ha agregado compatibilidad para crear clústeres de AKS habilitando la identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-120">Support create aks clusters enabling managed identity</span></span>
* <span data-ttu-id="9fd5f-121">az aks: se valida que el complemento de red sea "azure" o "kubenet".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-121">az aks: Validate network plugin to be either "azure" or "kubenet"</span></span>
* <span data-ttu-id="9fd5f-122">az aks: se ha agregado compatibilidad con claves de sesión de AAD.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-122">az aks: Add aad session key support</span></span>
* <span data-ttu-id="9fd5f-123">[CAMBIO IMPORTANTE] az aks: se admiten cambios de MSI para GF y BF para omsagent (supervisión de contenedores) (n.º 1).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-123">[BREAKING CHANGE] az aks: support msi changes for GF and BF for omsagent (Container monitoring)(#1)</span></span>
* <span data-ttu-id="9fd5f-124">az aks use-dev-spaces: Se ha agregado la opción de tipo de punto de conexión al comando use-dev-spaces para personalizar el punto de conexión creado en un controlador de Azure Dev Spaces.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-124">az aks use-dev-spaces: Adding endpoint type option to the use-dev-spaces command to customize the endpoint created on an Azure Dev Spaces controller</span></span>

### <a name="appconfig"></a><span data-ttu-id="9fd5f-125">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9fd5f-125">AppConfig</span></span>

* <span data-ttu-id="9fd5f-126">Se permite usar "kv set" para agregar la característica y la referencia de keyvault.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-126">Unblock using "kv set" to add keyvault reference and feature …</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-127">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-127">AppService</span></span>

* <span data-ttu-id="9fd5f-128">az webapp create: se ha corregido un problema al ejecutar el comando con --runtime.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-128">az webapp create : Fix issue when running the command with --runtime</span></span>
* <span data-ttu-id="9fd5f-129">az functionapp deployment source config-zip: se ha agregado un mensaje de error si el nombre de la función o del grupo de recursos no es válido o no existe.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-129">az functionapp deployment source config-zip: Add an error message if resource group or function name are invalid/don't exist</span></span>
* <span data-ttu-id="9fd5f-130">functionapp create: se ha corregido el mensaje de advertencia que aparece con `functionapp create` actualmente y que indica una marca `--functions_version` pero usa erróneamente `_` en lugar de `-` en el nombre de la marca.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-130">functionapp create: Fix the warning message that appears with `functionapp create` today which cites a `--functions_version` flag but erroneously uses a `_` instead of a `-` in the flag name</span></span>
* <span data-ttu-id="9fd5f-131">az functionapp create: se ha actualizado el modo en que se establecían el valor de linuxFxVersion y el nombre de la imagen de contenedor para las aplicaciones de funciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-131">az functionapp create: Updated the way linuxFxVersion and container image name were being set for linux function apps</span></span>
* <span data-ttu-id="9fd5f-132">az functionapp deployment source config-zip: se ha corregido un problema debido a que la configuración de la aplicación cambia la condición de carrera durante la implementación del archivo zip, lo que da errores 5xx durante la implementación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-132">az functionapp deployment source config-zip: Fix an issue caused by app settings change racing condition during zip deploy, giving 5xx errors during deployment</span></span>
* <span data-ttu-id="9fd5f-133">Se ha corregido el error 5720946: az webapp backup no puede establecer el nombre.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-133">Fix #5720946: az webapp backup fails to set name</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-134">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-134">ARM</span></span>

* <span data-ttu-id="9fd5f-135">az resource: se han mejorado los ejemplos del módulo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-135">az resource: Improve the examples of the resource module</span></span>
* <span data-ttu-id="9fd5f-136">az policy assignment list: se permite enumerar las asignaciones de directivas en el ámbito del grupo de administración.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-136">az policy assignment list: Support listing policy assignments at Management Group scope</span></span>
* <span data-ttu-id="9fd5f-137">Se han agregado `az deployment group` y `az deployment operation group` para la implementación de plantilla en grupos de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-137">Add `az deployment group` and `az deployment operation group` for template deployment at resource groups.</span></span> <span data-ttu-id="9fd5f-138">Es un duplicado de `az group deployment` y `az group deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-138">This is a duplicate of `az group deployment` and `az group deployment operation`</span></span>
* <span data-ttu-id="9fd5f-139">Se han agregado `az deployment sub` y `az deployment operation sub` para la implementación de plantilla en el ámbito de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-139">Add `az deployment sub` and `az deployment operation sub` for template deployment at subscription scope.</span></span> <span data-ttu-id="9fd5f-140">Es un duplicado de `az deployment` y `az deployment operation`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-140">This is a duplicate of `az deployment` and `az deployment operation`</span></span>
* <span data-ttu-id="9fd5f-141">Se han agregado `az deployment mg` y `az deployment operation mg` para la implementación de plantilla en grupos de administración.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-141">Add `az deployment mg` and `az deployment operation mg` for template deployment at management groups</span></span>
* <span data-ttu-id="9fd5f-142">Se han agregado `az deployment tenant` y `az deployment operation tenant` para la implementación de plantilla en el ámbito del inquilino.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-142">Add `az deployment tenant` and `az deployment operation tenant` for template deployment at tenant scope</span></span>
* <span data-ttu-id="9fd5f-143">az policy assignment create: se ha agregado una descripción al parámetro `--location`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-143">az policy assignment create: Add a description to the `--location` parameter</span></span>
* <span data-ttu-id="9fd5f-144">az group deployment create: se ha agregado el parámetro `--aux-tenants` para admitir varios inquilinos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-144">az group deployment create: Add parameter `--aux-tenants` to support cross tenants</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-145">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-145">CDN</span></span>

* <span data-ttu-id="9fd5f-146">Se han agregado comandos WAF de CDN.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-146">Add CDN WAF commands</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-147">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-147">Compute</span></span>

* <span data-ttu-id="9fd5f-148">az sig image-version: se ha agregado --data-snapshot-luns.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-148">az sig image-version: add --data-snapshot-luns</span></span>
* <span data-ttu-id="9fd5f-149">az ppg show: se ha agregado --colocation-status para poder capturar el estado de coubicación de todos los recursos del grupo de ubicación de proximidad.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-149">az ppg show: add --colocation-status to enable fetching the colocation status of all the resources in the proximity placement group</span></span>
* <span data-ttu-id="9fd5f-150">az vmss create/update: se admiten reparaciones automáticas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-150">az vmss create/update: support automatic repairs</span></span>
* <span data-ttu-id="9fd5f-151">[CAMBIO IMPORTANTE] az image template: se ha cambiado el nombre de la plantilla a builder.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-151">[BREAKING CHANGE] az image template: rename template to builder</span></span>
* <span data-ttu-id="9fd5f-152">az image builder create: se ha agregado --image-template.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-152">az image builder create: add --image-template</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fd5f-153">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-153">Cosmos DB</span></span>

* <span data-ttu-id="9fd5f-154">Se han agregado los cmdlets Sql stored procedure, udf y trigger.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-154">Add Sql stored procedure, udf and trigger cmdlets</span></span>
* <span data-ttu-id="9fd5f-155">az cosmosdb create: se ha agregado --key-uri para poder agregar información de cifrado del almacén de claves.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-155">az cosmosdb create: add --key-uri to support adding key vault encryption information</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-156">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-156">KeyVault</span></span>

* <span data-ttu-id="9fd5f-157">keyvault create: soft-delete está habilitado de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-157">keyvault create: enable soft-delete by default</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-158">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-158">Monitor</span></span>

* <span data-ttu-id="9fd5f-159">az monitor metrics alert create: se admite `~` en `--condition`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-159">az monitor metrics alert create: support `~` in `--condition`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-160">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-160">Network</span></span>

* <span data-ttu-id="9fd5f-161">az network application-gateway rewrite-rule create: se admite la configuración de la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-161">az network application-gateway rewrite-rule create: support url configuration</span></span>
* <span data-ttu-id="9fd5f-162">az network dns zone import: --zone-name no hará distinción de mayúsculas y minúsculas en el futuro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-162">az network dns zone import: --zone-name will be case insensitive in the future</span></span>
* <span data-ttu-id="9fd5f-163">az network private-endpoint/private-link-service: se ha quitado la etiqueta de versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-163">az network private-endpoint/private-link-service: remove preview label</span></span>
* <span data-ttu-id="9fd5f-164">az network bastion: se admiten hosts bastión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-164">az network bastion: support bastion</span></span>
* <span data-ttu-id="9fd5f-165">az network vnet list-available-ips: permite enumerar la lista de IPS disponibles en una red virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-165">az network vnet list-available-ips: support list available ips in a vnet</span></span>
* <span data-ttu-id="9fd5f-166">az network watcher flow-log create/list/delete/update: se han agregado nuevos comandos para administrar el registro del flujo del monitor y se expone --location para identificar el monitor explícitamente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-166">az network watcher flow-log create/list/delete/update: add new commands to manage watcher flow log and exposing --location to identify watcher explicitly</span></span>
* <span data-ttu-id="9fd5f-167">az network watcher flow-log configure: en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-167">az network watcher flow-log configure: deprecated</span></span>
* <span data-ttu-id="9fd5f-168">az network watcher flow-log show: se admiten --location y --name para obtener un resutlado con formato ARM; la salida con el formato antiguo ha quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-168">az network watcher flow-log show: support --location and --name to get ARM-formatted result, deprecated old formatted output</span></span>

### <a name="policy"></a><span data-ttu-id="9fd5f-169">Directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-169">Policy</span></span>

* <span data-ttu-id="9fd5f-170">az policy assignment create: Se ha corregido el error por el que el nombre de la asignación de directiva generado automáticamente supera el límite.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-170">az policy assignment create: Fix the bug that automatically generated name of policy assignment exceeds the limit</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-171">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-171">RBAC</span></span>

* <span data-ttu-id="9fd5f-172">az ad group show: se ha corregido el error por el que el valor de --group se trataba como un problema de regex.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-172">az ad group show: fix --group value treated as regex problem</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-173">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-173">RDBMS</span></span>

* <span data-ttu-id="9fd5f-174">Se ha actualizado la versión del SDK de azure-mgmt-rdbms a la 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-174">Bump the azure-mgmt-rdbms SDK version to 2.0.0</span></span>
* <span data-ttu-id="9fd5f-175">az postgres private-endpoint-connection: administración de las conexiones de punto de conexión privado de postgres.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-175">az postgres private-endpoint-connection: manage postgres private endpoint connections</span></span>
* <span data-ttu-id="9fd5f-176">az postgres private-link-resource: administración de los recursos de vínculo privado de postgres.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-176">az postgres private-link-resource: manage postgres private link resources</span></span>
* <span data-ttu-id="9fd5f-177">az mysql private-endpoint-connection: administración de las conexiones de punto de conexión privado mysql.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-177">az mysql private-endpoint-connection: manage mysql private endpoint connections</span></span>
* <span data-ttu-id="9fd5f-178">az mysql private-link-resource: administración de los recursos de vínculo privado de mysql.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-178">az mysql private-link-resource: manage mysql private link resources</span></span>
* <span data-ttu-id="9fd5f-179">az mariadb private-endpoint-connection: administración de las conexiones de punto de conexión privado mariadb.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-179">az mariadb private-endpoint-connection: manage mariadb private endpoint connections</span></span>
* <span data-ttu-id="9fd5f-180">az mariadb private-link-resource: administración de los recursos de vínculo privado de mariadb.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-180">az mariadb private-link-resource: manage mariadb private link resources</span></span>
* <span data-ttu-id="9fd5f-181">Actualización de las pruebas de punto de conexión privado de RDBMS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-181">Updating RDBMS Private Endpoint Tests</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-182">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-182">SQL</span></span>

* <span data-ttu-id="9fd5f-183">Sql midb: se han agregado list-deleted, show-deleted, update-retention, show-retention.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-183">Sql midb Add: list-deleted, show-deleted, update-retention, show-retention</span></span>
* <span data-ttu-id="9fd5f-184">sql server create: se ha agregado la marca opcional "Enable" o "Disable" de public-network-access a sql server create.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-184">(sql server create:) Add optional public-network-access 'Enable'/'Disable' flag to sql server create</span></span>
* <span data-ttu-id="9fd5f-185">sql server update: se han realizado algunos cambios visibles para el usuario.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-185">(sql server update:) make some customer-facing change</span></span>
* <span data-ttu-id="9fd5f-186">Se ha agregado la propiedad minimal_tls_version para MI y SQL DB.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-186">Add minimal_tls_version property for MI and SQL DB</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-187">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-187">Storage</span></span>

* <span data-ttu-id="9fd5f-188">az storage blob delete-batch: Comportamiento incorrecto de la marca `--dryrun`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-188">az storage blob delete-batch: Misbehaving `--dryrun` flag</span></span>
* <span data-ttu-id="9fd5f-189">az storage account network-rule add (corrección de errores): se ha agregado que la operación debe ser idempotente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-189">az storage account network-rule add (bug fix): add operation should be idempotent</span></span>
* <span data-ttu-id="9fd5f-190">az storage account create/update: se permite elegir el enrutamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-190">az storage account create/update: Add Routing Preference support</span></span>
* <span data-ttu-id="9fd5f-191">Se ha actualizado la versión de azure-mgmt-storage a la 8.0.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-191">Upgrade azure-mgmt-storage version to 8.0.0</span></span>
* <span data-ttu-id="9fd5f-192">az storage container immutability create: se ha agregado el parámetro --allow-protected-append-write.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-192">az storage container immutability create: add --allow-protected-append-write parameter</span></span>
* <span data-ttu-id="9fd5f-193">az storage account private-link-resource list: se ha agregado compatibilidad para enumerar los recursos de vínculo privado de la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-193">az storage account private-link-resource list: Add support to list private link resources for storage account</span></span>
* <span data-ttu-id="9fd5f-194">az storage account private-endpoint-connection approve/reject/show/delete: compatibilidad para administrar las conexiones de punto de conexión privado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-194">az storage account private-endpoint-connection approve/reject/show/delete: Support to manage private endpoint connections</span></span>
* <span data-ttu-id="9fd5f-195">az storage account blob-service-properties update: se han agregado --enable-restore-policy y --restore-days.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-195">az storage account blob-service-properties update: add --enable-restore-policy and --restore-days</span></span>
* <span data-ttu-id="9fd5f-196">az storage blob restore: se ha agregado compatibilidad para restaurar intervalos de blobs.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-196">az storage blob restore: Add support to restore blob ranges</span></span>

## <a name="february-18-2020"></a><span data-ttu-id="9fd5f-197">18 de febrero de 2020</span><span class="sxs-lookup"><span data-stu-id="9fd5f-197">February 18, 2020</span></span>

<span data-ttu-id="9fd5f-198">Versión 2.1.0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-198">Version 2.1.0</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-199">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-199">ACR</span></span>

* <span data-ttu-id="9fd5f-200">Se ha agregado un nuevo argumento `--expose-token` a `az acr login`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-200">Add a new argument `--expose-token` for `az acr login`</span></span>
* <span data-ttu-id="9fd5f-201">Se ha corregido la salida incorrecta de `az acr task identity show -n Name -r Registry -o table`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-201">Fix the incorrect output of `az acr task identity show -n Name -r Registry -o table`</span></span>
* <span data-ttu-id="9fd5f-202">az acr login: se inicia un CLIError si el comando de Docker devuelve errores.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-202">az acr login: Throw a CLIError if there are errors returned by docker command</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-203">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-203">ACS</span></span>

* <span data-ttu-id="9fd5f-204">aks create/update: se ha agregado la validación `--vnet-subnet-id`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-204">aks create/update: add `--vnet-subnet-id` validation</span></span>

### <a name="aladdin"></a><span data-ttu-id="9fd5f-205">Aladdin</span><span class="sxs-lookup"><span data-stu-id="9fd5f-205">Aladdin</span></span>

* <span data-ttu-id="9fd5f-206">Se analizan los ejemplos generados en los archivos _help.py de los comandos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-206">Parse generated examples into commands' _help.py</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-207">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-207">AMS</span></span>

* <span data-ttu-id="9fd5f-208">az ams ya está disponible con carácter general.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-208">az ams is GA now</span></span>

### <a name="appconfig"></a><span data-ttu-id="9fd5f-209">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9fd5f-209">AppConfig</span></span>

* <span data-ttu-id="9fd5f-210">Se ha revisado el mensaje de ayuda para excluir un filtro de clave/etiqueta no compatible.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-210">Revise help message to exclude unsupported key/label filter</span></span>
* <span data-ttu-id="9fd5f-211">Se ha quitado la etiqueta de versión preliminar en la mayoría de los comandos, salvo las marcas de identidad administrada y características.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-211">Remove preview tag for most commands excluding managed identity and feature flags</span></span>
* <span data-ttu-id="9fd5f-212">Se ha agregado una clave administrada de cliente al actualizar los almacenes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-212">Add customer managed key when updating stores</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-213">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-213">AppService</span></span>

* <span data-ttu-id="9fd5f-214">az webapp list-runtimes: se ha corregido el error de list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-214">az webapp list-runtimes: Fix the bug for list-runtimes</span></span>
* <span data-ttu-id="9fd5f-215">Se ha agregado az webapp|functionapp config ssl create.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-215">Add az webapp|functionapp config ssl create</span></span>
* <span data-ttu-id="9fd5f-216">Se ha agregado compatibilidad con las aplicaciones de funciones v3 y Node 12.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-216">Add support for v3 function apps and node 12</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-217">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-217">ARM</span></span>

* <span data-ttu-id="9fd5f-218">az policy assignment create: se ha corregido el mensaje de error cuando el parámetro `--policy` no es válido.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-218">az policy assignment create: Fix the error message when the `--policy` parameter is invalid</span></span>
* <span data-ttu-id="9fd5f-219">az group deployment create: se ha corregido el error "stat: path too long for Windows" (stat: la ruta es demasiado larga para Windows) cuando se usa un archivo parameters.json de gran tamaño.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-219">az group deployment create: Fix "stat: path too long for Windows" error when using large parameters.json file</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-220">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-220">Backup</span></span>

* <span data-ttu-id="9fd5f-221">Se ha corregido el flujo de recuperación en el nivel de elemento de OLR.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-221">Fix for item level recovery flow in OLR</span></span>
* <span data-ttu-id="9fd5f-222">Se ha agregado compatibilidad con restauración como archivos para bases de datos SQL y SAP.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-222">Add restore as files support for SQL and SAP Databases</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-223">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-223">Compute</span></span>

* <span data-ttu-id="9fd5f-224">vm/vmss/availability-set update: se ha agregado --ppg para poder actualizar ProximityPlacementGroup.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-224">vm/vmss/availability-set update: add --ppg to allowing updating ProximityPlacementGroup</span></span>
* <span data-ttu-id="9fd5f-225">vmss create: se ha agregado --data-disk-iops y --data-disk-mbps.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-225">vmss create: add --data-disk-iops and --data-disk-mbps</span></span>
* <span data-ttu-id="9fd5f-226">az vm host: se ha quitado la etiqueta de versión preliminar en `vm host` y `vm host group`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-226">az vm host: remove preview tag for `vm host` and `vm host group`</span></span>
* <span data-ttu-id="9fd5f-227">[CAMBIO IMPORTANTE] Se ha corregido el error 10728: `az vm create`: se crea una subred automáticamente si se especifica una red virtual y no existe una subred</span><span class="sxs-lookup"><span data-stu-id="9fd5f-227">[BREAKING CHANGE] Fix #10728: `az vm create`: create subnet automatically if vnet is specified and subnet not exists</span></span>
* <span data-ttu-id="9fd5f-228">Se ha aumentado la solidez de la lista de imágenes de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-228">Increase robustness of vm image list</span></span>

### <a name="eventhub"></a><span data-ttu-id="9fd5f-229">Eventhub</span><span class="sxs-lookup"><span data-stu-id="9fd5f-229">Eventhub</span></span>

* <span data-ttu-id="9fd5f-230">Compatibilidad de Azure Stack con el perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-230">Azure Stack support for 2019-03-01-hybrid profile</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-231">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-231">KeyVault</span></span>

* <span data-ttu-id="9fd5f-232">az keyvault key create: se ha agregado un nuevo valor `import` al parámetro `--ops`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-232">az keyvault key create: add a new value `import` for parameter `--ops`</span></span>
* <span data-ttu-id="9fd5f-233">az keyvault key list-versions: se ha agregado compatibilidad con el parámetro `--id` para especificar claves.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-233">az keyvault key list-versions: support parameter `--id` for specifying keys</span></span>
* <span data-ttu-id="9fd5f-234">Se ha agregado compatibilidad con conexiones de punto de conexión privado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-234">Support private endpoint connections</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-235">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-235">Network</span></span>

* <span data-ttu-id="9fd5f-236">Cambio a azure-mgmt-network 9.0.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-236">Bump to azure-mgmt-network 9.0.0</span></span>
* <span data-ttu-id="9fd5f-237">az network private-link-service update/create: se ha agregado compatibilidad con --enable-proxy-protocol.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-237">az network private-link-service update/create: support --enable-proxy-protocol</span></span>
* <span data-ttu-id="9fd5f-238">Se ha agregado la característica Monitor de conexión V2.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-238">Add connection Monitor V2 feature</span></span>

### <a name="packaging"></a><span data-ttu-id="9fd5f-239">Packaging</span><span class="sxs-lookup"><span data-stu-id="9fd5f-239">Packaging</span></span>

* <span data-ttu-id="9fd5f-240">[CAMBIO IMPORTANTE] Python 2.7 deja de ser compatible.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-240">[BREAKING CHANGE] Drop support for Python 2.7</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-241">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-241">Profile</span></span>

* <span data-ttu-id="9fd5f-242">Vista previa: Se han agregado nuevos atributos `homeTenantId` y `managedByTenants` a las cuentas de suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-242">Preview: Add new attributes `homeTenantId` and `managedByTenants` to subscription accounts.</span></span> <span data-ttu-id="9fd5f-243">Vuelva a ejecutar `az login` para aplicar los cambios.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-243">Please re-run `az login` for the changes to take effect</span></span>
* <span data-ttu-id="9fd5f-244">az login: se muestra una advertencia cuando aparece una suscripción en más de un inquilino, y se toma la primera como predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-244">az login: Show a warning when a subscription is listed from more than one tenants and default to the first one.</span></span> <span data-ttu-id="9fd5f-245">Para seleccionar un inquilino específico al obtener acceso a esta suscripción, incluya `--tenant` en `az login`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-245">To select a specific tenant when accessing this subscription, please include `--tenant` in `az login`</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-246">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-246">Role</span></span>

* <span data-ttu-id="9fd5f-247">az role assignment create: se ha corregido el error por el que, al asignar un rol a una entidad de servicio por nombre para mostrar, se produce un error HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-247">az role assignment create: Fix the error that assigning a role to a service principal by display name yields a HTTP 400</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-248">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-248">SQL</span></span>

* <span data-ttu-id="9fd5f-249">Se ha actualizado el cmdlet `az sql mi update` de Instancia administrada de SQL Database con dos nuevos parámetros: tier y family.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-249">Update SQL Managed Instance cmdlet `az sql mi update` with two new parameters: tier and family</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-250">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-250">Storage</span></span>

* <span data-ttu-id="9fd5f-251">[CAMBIO IMPORTANTE] `az storage account create`: Se ha cambiado el tipo de cuenta de almacenamiento predeterminada a StorageV2.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-251">[BREAKING CHANGE] `az storage account create`: Change default storage account kind to StorageV2</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="9fd5f-252">4 de febrero de 2020</span><span class="sxs-lookup"><span data-stu-id="9fd5f-252">February 04, 2020</span></span>

<span data-ttu-id="9fd5f-253">Versión 2.0.81</span><span class="sxs-lookup"><span data-stu-id="9fd5f-253">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-254">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-254">ACS</span></span>

* <span data-ttu-id="9fd5f-255">Se ha agregado compatibilidad para establecer los puertos asignados de salida y los tiempos de espera de inactividad en el equilibrador de carga estándar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-255">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="9fd5f-256">Actualización a la versión de API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="9fd5f-256">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-257">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-257">ACR</span></span>

* <span data-ttu-id="9fd5f-258">[CAMBIO IMPORTANTE]  `az acr delete` mostrará un aviso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-258">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="9fd5f-259">[CAMBIO IMPORTANTE] "az acr task delete" mostrará un aviso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-259">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="9fd5f-260">Se ha agregado un nuevo grupo de comandos "az acr taskrun show/list/delete" para la administración de la ejecución de tareas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-260">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-261">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-261">AKS</span></span>

* <span data-ttu-id="9fd5f-262">Cada clúster obtiene una entidad de servicio independiente para mejorar el aislamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-262">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="9fd5f-263">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9fd5f-263">AppConfig</span></span>

* <span data-ttu-id="9fd5f-264">Se ha agregado compatibilidad con la importación y exportación de referencias al almacén de claves hacia y desde appservice.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-264">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="9fd5f-265">Se ha agregado compatibilidad con la importación y exportación de todas las etiquetas de appconfig a appconfig.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-265">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="9fd5f-266">Ahora se validan los nombres de clave y de característica antes de establecerlos e importarlos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-266">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="9fd5f-267">Se ha expuesto la modificación de la SKU para el almacén de configuración.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-267">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="9fd5f-268">Se ha agregado el grupo de comandos para identidades administradas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-268">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-269">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-269">AppService</span></span>

* <span data-ttu-id="9fd5f-270">Azure Stack: exposición de los comandos del perfil 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-270">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="9fd5f-271">functionapp: se ha incorporado la capacidad de crear aplicaciones de función de Java en Linux.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-271">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-272">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-272">ARM</span></span>

* <span data-ttu-id="9fd5f-273">Corrección del problema 10246: `az resource tag` se bloquea cuando el parámetro `--ids` pasado es un identificador de grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-273">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="9fd5f-274">Corrección del problema 11658: el comando `az group export` no admite los parámetros `--query` y `--output`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-274">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="9fd5f-275">Corrección del problema 10279: el código de salida de `az group deployment validate` es 0 cuando se produce un error en la comprobación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-275">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="9fd5f-276">Corrección del problema 9916: se ha mejorado el mensaje de error del conflicto entre la etiqueta y otras condiciones de filtro del comando `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-276">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="9fd5f-277">Se ha agregado un nuevo parámetro `--managed-by` para admitir la adición de información de managedBy para el comando `az group create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-277">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="9fd5f-278">Red Hat OpenShift en Azure</span><span class="sxs-lookup"><span data-stu-id="9fd5f-278">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="9fd5f-279">Se ha agregado el subgrupo `monitor` para administrar la supervisión de Log Analytics en el clúster de Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-279">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-280">BotService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-280">BotService</span></span>

* <span data-ttu-id="9fd5f-281">Corrección del problema 11697: `az bot create` no es idempotente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-281">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="9fd5f-282">Se han cambiado las pruebas de corrección del nombre para que se ejecuten solo en modo activo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-282">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-283">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-283">CDN</span></span>

* <span data-ttu-id="9fd5f-284">Se ha incorporado compatibilidad con la característica rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-284">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="9fd5f-285">Se ha agregado un nuevo grupo de comandos "cdn endpoint rule" para administrar reglas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-285">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="9fd5f-286">Se ha actualizado la versión de azure-mgmt-cdn a la 4.0.0 para usar la versión de API 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-286">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="9fd5f-287">Administrador de implementaciones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-287">Deployment Manager</span></span>

* <span data-ttu-id="9fd5f-288">Se ha agregado la operación de lista para todos los recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-288">Add list operation for all resources.</span></span>
* <span data-ttu-id="9fd5f-289">Se ha mejorado el recurso de paso para el nuevo tipo de paso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-289">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="9fd5f-290">Se ha actualizado el paquete azure-mgmt-deploymentmanager para usar la versión 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-290">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-291">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-291">IoT</span></span>

* <span data-ttu-id="9fd5f-292">Los comandos "IoT hub Job" han quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-292">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="9fd5f-293">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fd5f-293">IoT Central</span></span>

* <span data-ttu-id="9fd5f-294">Se ha agregado compatibilidad con la creación y actualización de aplicaciones con el nuevo nombre de SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-294">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-295">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-295">Key Vault</span></span>

* <span data-ttu-id="9fd5f-296">Se ha agregado un nuevo comando `az keyvault key download` para descargar claves.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-296">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="9fd5f-297">Varios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-297">Misc</span></span>

* <span data-ttu-id="9fd5f-298">Corrección 6371: se ha agregado compatibilidad con la finalización de nombres de archivo y variables de entorno en Bash.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-298">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-299">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-299">Network</span></span>

* <span data-ttu-id="9fd5f-300">Fix #2092: az network dns record-set add/remove. Se ha agregado una advertencia cuando no se encuentra el conjunto de registros.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-300">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="9fd5f-301">En el futuro, se admitirá un argumento adicional para confirmar esta creación automática.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-301">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="9fd5f-302">Directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-302">Policy</span></span>

* <span data-ttu-id="9fd5f-303">Se ha agregado un nuevo comando `az policy metadata` para recuperar recursos de metadatos de directivas enriquecidos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-303">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="9fd5f-304">`az policy remediation create`: especifica si se debe volver a evaluar la compatibilidad antes de la corrección con el parámetro `--resource-discovery-mode`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-304">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-305">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-305">Profile</span></span>

* <span data-ttu-id="9fd5f-306">`az account get-access-token`: se ha agregado el parámetro `--tenant` para adquirir el token para el inquilino directamente, sin necesidad de especificar una suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-306">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-307">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-307">RBAC</span></span>

* <span data-ttu-id="9fd5f-308">[CAMBIO IMPORTANTE] Corrección 11883: `az role assignment create`: si el ámbito está vacío se mostrará un aviso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-308">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="9fd5f-309">Seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-309">Security</span></span>

* <span data-ttu-id="9fd5f-310">Se han agregado los nuevos comandos `az atp show` y `az atp update` para ver y administrar la configuración de protección contra amenazas avanzada para las cuentas de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-310">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-311">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-311">SQL</span></span>

* <span data-ttu-id="9fd5f-312">`sql dw create`: los parámetros `--zone-redundant` y `--read-replica-count` han quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-312">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="9fd5f-313">Estos parámetros no se aplican a DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-313">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="9fd5f-314">[CAMBIO IMPORTANTE] `az sql db create`: Se han quitado "WideWorldImportersStd" y "WideWorldImportersFull" como valores permitidos documentados de "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-314">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="9fd5f-315">Estas bases de datos de ejemplo siempre provocarán un error en la creación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-315">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="9fd5f-316">Se han agregado los nuevos comandos `sql db classification show/list/update/delete` y `sql db classification recommendation list/enable/disable` para administrar las clasificaciones de confidencialidad de las bases de datos SQL.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-316">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="9fd5f-317">`az sql db audit-policy`: corrección para acciones y grupos de auditoría vacíos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-317">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-318">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-318">Storage</span></span>

* <span data-ttu-id="9fd5f-319">Se ha agregado un nuevo grupo de comandos `az storage share-rm` para usar el proveedor de recursos Microsoft.Storage para las operaciones de administración de recursos compartidos de archivos de Azure.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-319">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="9fd5f-320">Corrección del problema 11415: error de permisos para `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-320">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="9fd5f-321">Se ha integrado Azcopy 10.3.3 y se ha agregado compatibilidad con Win32.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-321">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="9fd5f-322">`az storage copy`: se han agregado los parámetros `--include-path`, `--include-pattern`, `--exclude-path` y `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-322">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="9fd5f-323">`az storage remove`: se han cambiado los parámetros `--inlcude` y `--exclude` por los parámetros `--include-path`, `--include-pattern`, `--exclude-path` y `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-323">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="9fd5f-324">`az storage sync`: se han agregado los parámetros `--include-pattern`, `--exclude-path` y `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-324">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9fd5f-325">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-325">ServiceFabric</span></span>

* <span data-ttu-id="9fd5f-326">Se han agregado nuevos comandos para administrar aplicaciones y servicios.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-326">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="9fd5f-327">13 de enero de 2020</span><span class="sxs-lookup"><span data-stu-id="9fd5f-327">January 13, 2020</span></span>

<span data-ttu-id="9fd5f-328">Versión 2.0.80</span><span class="sxs-lookup"><span data-stu-id="9fd5f-328">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-329">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-329">Compute</span></span>

* <span data-ttu-id="9fd5f-330">disk update: Se han agregado --disk-encryption-set y --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-330">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="9fd5f-331">snapshot create/update: Se han agregado --disk-encryption-set y --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-331">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-332">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-332">Storage</span></span>

* <span data-ttu-id="9fd5f-333">Se ha actualizado la versión de azure-mgmt-storage a la 7.1.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-333">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="9fd5f-334">`az storage account create`: Se han agregado `--encryption-key-type-for-table` y `--encryption-key-type-for-queue` para admitir el servicio de cifrado de tablas y colas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-334">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="9fd5f-335">7 de enero de 2020</span><span class="sxs-lookup"><span data-stu-id="9fd5f-335">January 07, 2020</span></span>

<span data-ttu-id="9fd5f-336">Versión 2.0.79</span><span class="sxs-lookup"><span data-stu-id="9fd5f-336">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-337">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-337">ACR</span></span>

* <span data-ttu-id="9fd5f-338">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro "--os" para "acr build", "acr task create/update", "acr run" y "acr pack".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-338">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="9fd5f-339">En su lugar, utilice "--platform".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-339">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="9fd5f-340">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9fd5f-340">AppConfig</span></span>

* <span data-ttu-id="9fd5f-341">Se ha agregado compatibilidad para la importación y exportación de marcas de características.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-341">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="9fd5f-342">Se ha agregado el nuevo comando "az appconfig kv set-keyvault" para crear la referencia de Key Vault.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-342">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="9fd5f-343">Compatibilidad con diversas convenciones de nomenclatura al exportar marcas de características a un archivo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-343">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-344">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-344">AppService</span></span>

* <span data-ttu-id="9fd5f-345">Se ha corregido el problema 7154: actualización de la documentación del comando <> para usar acentos invertidos en lugar de comillas simples.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-345">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="9fd5f-346">Se ha corregido el problema 11287: webapp up: de forma predeterminada, la aplicación creada con up "debe estar habilitada para SSL".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-346">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="9fd5f-347">Se ha corregido el problema 11592: se ha agregado la marca az webapp up para sitios HTML estáticos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-347">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-348">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-348">ARM</span></span>

* <span data-ttu-id="9fd5f-349">Se ha corregido `az resource tag`: no se pueden actualizar las etiquetas del almacén de Recovery Services.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-349">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-350">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-350">Backup</span></span>

* <span data-ttu-id="9fd5f-351">Se ha agregado un nuevo comando "backup protection undelete" para habilitar la característica de eliminación temporal para la carga de trabajo de IaasVM.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-351">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="9fd5f-352">Se ha agregado el nuevo parámetro "--soft-delete-feature-state" al comando set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-352">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="9fd5f-353">Se ha agregado compatibilidad con la exclusión de disco para la carga de trabajo de IaasVM.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-353">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-354">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-354">Compute</span></span>

* <span data-ttu-id="9fd5f-355">Se ha corregido el error de `vm create` en el perfil de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-355">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="9fd5f-356">vm monitor metrics tail/list-definitions: compatibilidad con métricas de consultas y definiciones de lista para una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-356">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="9fd5f-357">Se ha agregado la nueva acción del comando reapply para az vm.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-357">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-358">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-358">HDInsight</span></span>

* <span data-ttu-id="9fd5f-359">Compatibilidad con la creación de un clúster de Kafka con Kafka Rest Proxy.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-359">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="9fd5f-360">Se ha actualizado azure-mgmt-hdinsight a la versión 1.3.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-360">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="9fd5f-361">Varios:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-361">Misc.</span></span>

* <span data-ttu-id="9fd5f-362">Se ha agregado el comando en versión preliminar `az version show` para mostrar las versiones de los módulos de la CLI de Azure y las extensiones en formato JSON de forma predeterminada o con el formato configurado con --output.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-362">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="9fd5f-363">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9fd5f-363">Event Hubs</span></span>

* <span data-ttu-id="9fd5f-364">[CAMBIO IMPORTANTE] Se ha eliminado la opción de estado "ReceiveDisabled" de los comandos "az eventhubs eventhub update" y "az eventhubs eventhub create".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-364">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="9fd5f-365">Esta opción no es válida para entidades de Event Hubs.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-365">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fd5f-366">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-366">Service Bus</span></span>

* <span data-ttu-id="9fd5f-367">[CAMBIO IMPORTANTE] Se ha eliminado la opción de estado "ReceiveDisabled" de los comandos "az servicebus topic create", "az servicebus topic update", "az servicebus queue create" y "az servicebus queue update".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-367">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="9fd5f-368">Esta opción no es válida para temas y colas de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-368">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-369">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-369">RBAC</span></span>

* <span data-ttu-id="9fd5f-370">Se ha corregido el error 11712: `az ad app/sp show` no devuelve el código de salida 3 cuando la aplicación o la entidad de servicio no existen.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-370">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-371">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-371">Storage</span></span>

* <span data-ttu-id="9fd5f-372">`az storage account create`: se ha eliminado la marca en versión preliminar para el parámetro --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-372">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="9fd5f-373">Se ha actualizado la versión de azure-mgmt-storage a la 7.0.0 para usar la versión de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-373">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="9fd5f-374">Se han agregado los nuevos parámetros `--enable-delete-retention` y `--delete-retention-days` para admitir la administración de la directiva de retención de eliminación para blob-service-properties de la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-374">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="9fd5f-375">17 de diciembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-375">December 17, 2019</span></span>

<span data-ttu-id="9fd5f-376">2.0.78</span><span class="sxs-lookup"><span data-stu-id="9fd5f-376">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-377">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-377">ACR</span></span>

* <span data-ttu-id="9fd5f-378">Se ha agregado la compatibilidad con el contexto local en acr task run.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-378">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-379">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-379">ACS</span></span>

* <span data-ttu-id="9fd5f-380">[CAMBIO IMPORTANTE] az openshift create: se ha cambiado el nombre de `--workspace-resource-id` a `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-380">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-381">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-381">AMS</span></span>

* <span data-ttu-id="9fd5f-382">Se han actualizado los comandos show para devolver un código 3 cuando no se encuentra el recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-382">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="9fd5f-383">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9fd5f-383">AppConfig</span></span>

* <span data-ttu-id="9fd5f-384">Se ha corregido el error al anexar la versión de la API a la dirección URL de la solicitud.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-384">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="9fd5f-385">La solución existente no funciona con la paginación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-385">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="9fd5f-386">Se ha agregado compatibilidad para mostrar idiomas además del inglés, ya que el servicio de back-end admite Unicode para la globalización.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-386">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-387">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-387">AppService</span></span>

* <span data-ttu-id="9fd5f-388">Se ha corregido el problema 11217: webapp: az webapp config ssl upload debe admitir el parámetro de ranura.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-388">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="9fd5f-389">Se ha corregido el problema 10965: Error: El nombre no puede estar vacío.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-389">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="9fd5f-390">Se permite la eliminación por ip_address y subnet (dirección IP y subred).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-390">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="9fd5f-391">Se ha agregado compatibilidad con la importación de certificados desde `az webapp config ssl import` de Key Vault.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-391">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-392">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-392">ARM</span></span>

* <span data-ttu-id="9fd5f-393">Se ha actualizado el paquete azure-mgmt-resource para usar la versión 6.0.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-393">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="9fd5f-394">Compatibilidad entre inquilinos para el comando `az group deployment create` mediante la adición del nuevo parámetro `--aux-subs`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-394">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="9fd5f-395">Se ha agregado un nuevo parámetro `--metadata` para admitir la adición de información de metadatos para definiciones de conjuntos de directivas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-395">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-396">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-396">Backup</span></span>

* <span data-ttu-id="9fd5f-397">Se ha agregado compatibilidad con la copia de seguridad para cargas de trabajo de SQL y SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-397">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-398">BotService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-398">BotService</span></span>

* <span data-ttu-id="9fd5f-399">[Cambio importante] Se ha eliminado la marca "--version" del comando en versión preliminar "az bot create".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-399">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="9fd5f-400">Solo se admiten los bots del SDK V4.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-400">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="9fd5f-401">Se ha agregado la comprobación de disponibilidad del nombre para "az bot create".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-401">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="9fd5f-402">Se ha agregado compatibilidad para actualizar la dirección URL del icono de un bot mediante "az bot update".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-402">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="9fd5f-403">Se ha agregado compatibilidad para actualizar un canal de Direct Line mediante "az bot directline update".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-403">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="9fd5f-404">Se ha agregado compatibilidad con la marca "--enable-enhanced-auth" para "az bot directline create".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-404">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="9fd5f-405">Los siguientes grupos de comandos están en disponibilidad general y no en versión preliminar: "az bot authsetting".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-405">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="9fd5f-406">Los siguientes comandos de "az bot" están en disponibilidad general y no en versión preliminar: "create", "prepare-deploy", "show", "delete", "update".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-406">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="9fd5f-407">Se ha corregido el cambio realizado por "az bot prepare-deploy" del valor de "--proj-file-path" a minúsculas (por ejemplo, de "Test.csproj" a "test.csproj").</span><span class="sxs-lookup"><span data-stu-id="9fd5f-407">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-408">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-408">Compute</span></span>

* <span data-ttu-id="9fd5f-409">vmss create/update: Se ha agregado --scale-in-policy, que decide qué máquinas virtuales se eligen para su eliminación cuando se reduce el tamaño de un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-409">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="9fd5f-410">vm/vmss update: Se ha agregado --priority.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-410">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="9fd5f-411">vm/vmss update: Se ha agregado --max-price.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-411">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="9fd5f-412">Se ha agregado el grupo de comandos disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-412">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="9fd5f-413">disk create: Se han agregado --encryption-type y --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-413">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="9fd5f-414">vm/vmss create: Se han agregado --os-disk-encryption-set y --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-414">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-415">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-415">Core</span></span>

* <span data-ttu-id="9fd5f-416">Se eliminó la compatibilidad con Python 3.4.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-416">Removed support for Python 3.4</span></span>
* <span data-ttu-id="9fd5f-417">Complemento HaTS survey en varios comandos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-417">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="9fd5f-418">DLS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-418">DLS</span></span>

* <span data-ttu-id="9fd5f-419">Se ha actualizado la versión del SDK de ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-419">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="9fd5f-420">Instalar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-420">Install</span></span>

* <span data-ttu-id="9fd5f-421">El script de instalación admite Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-421">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-422">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-422">IOT</span></span>

* <span data-ttu-id="9fd5f-423">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro --failover-region de manual-failover.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-423">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="9fd5f-424">Ahora se realizará la conmutación por error a la región secundaria emparejada geográficamente asignada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-424">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-425">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-425">Key Vault</span></span>

* <span data-ttu-id="9fd5f-426">Se ha corregido el error 8095: `az keyvault storage remove`: mejora del mensaje de ayuda.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-426">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="9fd5f-427">Se ha corregido el error 8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: se ha corregido el error de validación en el parámetro `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-427">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="9fd5f-428">Se ha corregido el error 10512: `az keyvault set-policy`: mejora del mensaje de error cuando no se especifican `--object-id`, `--spn` ni `--upn`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-428">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="9fd5f-429">Se ha corregido el error 10846: `az keyvault secret show-deleted`: cuando se especifica `--id`, no se requiere `--name/-n`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-429">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="9fd5f-430">Se ha corregido el error 11084: `az keyvault secret download`: mejora del mensaje de ayuda del parámetro `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-430">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-431">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-431">Network</span></span>

* <span data-ttu-id="9fd5f-432">az network application-gateway probe: se ha agregado compatibilidad con la opción -port para especificar un puerto para sondear servidores de back-end en la creación y actualización.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-432">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="9fd5f-433">az network application-gateway url-path-map create/update: se ha corregido el error de `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-433">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="9fd5f-434">az network application-gateway: se ha agregado compatibilidad con `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-434">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="9fd5f-435">az network list-service-aliases: se ha agregado compatibilidad con los alias de servicio de lista, que se pueden usar para las directivas del punto de conexión de servicio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-435">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="9fd5f-436">az network dns zone import: se ha agregado compatibilidad con .@ en el nombre de registro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-436">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="9fd5f-437">Packaging</span><span class="sxs-lookup"><span data-stu-id="9fd5f-437">Packaging</span></span>

* <span data-ttu-id="9fd5f-438">Se han agregado compilaciones de perímetro posterior para la instalación de pip.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-438">Added back edge builds for pip install</span></span>
* <span data-ttu-id="9fd5f-439">Se ha agregado el paquete eoan de Ubuntu.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-439">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="9fd5f-440">Directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-440">Policy</span></span>

* <span data-ttu-id="9fd5f-441">Se ha agregado compatibilidad con la versión 2019-09-01 de Policy API.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-441">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="9fd5f-442">az policy set-definition: se ha agregado compatibilidad con la agrupación dentro de definiciones de conjuntos de directivas con el parámetro `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-442">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="9fd5f-443">Redis</span><span class="sxs-lookup"><span data-stu-id="9fd5f-443">Redis</span></span>

* <span data-ttu-id="9fd5f-444">Se ha agregado el parámetro en versión preliminar `--replicas-per-master` al comando `az redis create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-444">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="9fd5f-445">Se ha actualizado azure-mgmt-redis de la versión 6.0.0 a la 7.0.0rc1.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-445">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9fd5f-446">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-446">ServiceFabric</span></span>

* <span data-ttu-id="9fd5f-447">Se ha corregido la lógica de adición de tipo de nodo, incluido el error 10963: la adición de un nuevo tipo de nodo con el nivel de durabilidad Gold siempre producirá un error de la CLI.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-447">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="9fd5f-448">La versión de ServiceFabricNodeVmExt se ha actualizado al a 1.1 en la plantilla de creación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-448">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-449">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-449">SQL</span></span>

* <span data-ttu-id="9fd5f-450">Se han agregado los parámetros "--read-scale" y "--read-replicas" a los comandos create y update de SQL DB para admitir la administración de escalado de lectura.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-450">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-451">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-451">Storage</span></span>

* <span data-ttu-id="9fd5f-452">Versión de disponibilidad general de la propiedad de recursos compartidos de archivos grandes para el comando de creación y actualización de la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-452">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="9fd5f-453">Versión de disponibilidad general de la compatibilidad de los token de SAS para la delegación de usuarios.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-453">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="9fd5f-454">Se han agregado los nuevos comandos `az storage account blob-service-properties show` y `az storage account blob-service-properties update --enable-change-feed` para administrar las propiedades de Blob Service para la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-454">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="9fd5f-455">[PRÓXIMO CAMBIO IMPORTANTE] `az storage copy`: ya no se admite el carácter `*` como comodín en la dirección URL, pero se agregarán nuevos parámetros --include-pattern y --exclude-pattern con compatibilidad con caracteres comodín `*`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-455">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="9fd5f-456">Se ha corregido el problema 11043: se ha agregado compatibilidad para eliminar todo el contenedor o el recurso compartido en el comando `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-456">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="9fd5f-457">26 de noviembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-457">November 26, 2019</span></span>

<span data-ttu-id="9fd5f-458">Versión 2.0.77</span><span class="sxs-lookup"><span data-stu-id="9fd5f-458">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-459">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-459">ACR</span></span>

* <span data-ttu-id="9fd5f-460">El parámetro `--branch` de acr task create/update ha quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-460">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="9fd5f-461">Red Hat OpenShift en Azure</span><span class="sxs-lookup"><span data-stu-id="9fd5f-461">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="9fd5f-462">Se ha agregado la marca `--workspace-resource-id` para permitir la creación de un clúster de Red Hat OpenShift en Azure con supervisión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-462">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="9fd5f-463">Se ha agregado `monitor_profile` para crear un clúster de Red Hat OpenShift en Azure con supervisión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-463">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-464">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-464">AKS</span></span>

* <span data-ttu-id="9fd5f-465">Se ha agregado compatibilidad con la operación de rotación de certificados del clúster mediante "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-465">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="9fd5f-466">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9fd5f-466">AppConfig</span></span>

* <span data-ttu-id="9fd5f-467">Se ha agregado compatibilidad con el uso de ":" como separador de `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-467">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="9fd5f-468">Se ha corregido un problema para enumerar los valores de clave con varias etiquetas que incluyen la etiqueta nula.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-468">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="9fd5f-469">Se ha actualizado el SDK del plano de administración, azure-mgmt-appconfiguration, a la versión 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-469">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="9fd5f-470">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-470">AppService</span></span>

* <span data-ttu-id="9fd5f-471">Se ha corregido el problema 11100: Error de atributo para az webapp up al crear el plan de servicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-471">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="9fd5f-472">az webapp up: cuando se fuerza la creación o implementación en un sitio para lenguajes admitidos, no se usan los valores predeterminados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-472">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="9fd5f-473">Se ha agregado compatibilidad para App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="9fd5f-473">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-474">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-474">Backup</span></span>

* <span data-ttu-id="9fd5f-475">Se ha corregido el problema en los elementos asociados a listas de directivas de az backup.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-475">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="9fd5f-476">Se ha agregado el parámetro opcional BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-476">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-477">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-477">Compute</span></span>

* <span data-ttu-id="9fd5f-478">Se ha actualizado la versión de la API de proceso, discos e instantáneas a la 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-478">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="9fd5f-479">vmss create: mejoras para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="9fd5f-479">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="9fd5f-480">sig image-definition create: se ha agregado --os-state para poder especificar si las máquinas virtuales creadas con esta imagen están "Generalizadas" o "Especializadas".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-480">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="9fd5f-481">sig image-definition create: se ha agregado --hyper-v-generation para poder especificar la generación del hipervisor.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-481">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="9fd5f-482">sig image-version create: se ha agregado compatibilidad con --os-snapshot y --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-482">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="9fd5f-483">image create: se ha agregado --data-disk-caching para poder especificar la configuración de almacenamiento en caché de los discos de datos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-483">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="9fd5f-484">Actualización del SDK de Compute para Python a la versión 10.0.0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-484">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="9fd5f-485">vm/vmss create: se ha agregado "Spot" a la propiedad de la enumeración "Priority".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-485">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="9fd5f-486">[Cambio importante] Se ha cambiado el nombre del parámetro "--max-billing" a "--max-price" para máquinas virtuales y VMSS, para que sean coherentes con los cmdlets de Swagger y Powershell.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-486">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="9fd5f-487">vm monitor log show: se ha agregado compatibilidad para la consulta del registro en el área de trabajo de Log Analytics vinculada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-487">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-488">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-488">IOT</span></span>

* <span data-ttu-id="9fd5f-489">Corrección 2531: se han agregado argumentos de utilidad para la actualización del concentrador.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-489">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="9fd5f-490">Corrección 8323: se han agregado los parámetros que faltaban para crear el punto de conexión personalizado de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-490">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="9fd5f-491">Corrección del error de regresión: se han revertido los cambios que invalidan el punto de conexión de almacenamiento predeterminado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-491">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-492">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-492">Key Vault</span></span>

* <span data-ttu-id="9fd5f-493">Corrección 11121: ahora, con `az keyvault certificate list`, al pasar `--include-pending` no se requiere un valor `true` o `false`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-493">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="9fd5f-494">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="9fd5f-494">NetAppFiles</span></span>

* <span data-ttu-id="9fd5f-495">Se ha actualizado azure-mgmt-netapp a la versión 0.7.0, que incluye algunas propiedades de volumen adicionales asociadas a futuras operaciones de replicación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-495">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-496">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-496">Network</span></span>

* <span data-ttu-id="9fd5f-497">application-gateway waf-config: en desuso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-497">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="9fd5f-498">application-gateway waf-policy: se han agregado reglas administradas de subgrupo para administrar conjuntos de reglas administradas y reglas de exclusión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-498">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="9fd5f-499">application-gateway waf-policy: se ha agregado la configuración de directivas de subgrupo para administrar la configuración global de una directiva de WAF.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-499">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="9fd5f-500">[Cambio importante] application-gateway waf-policy: se ha cambiado el nombre de la regla de subgrupo a regla personalizada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-500">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="9fd5f-501">application-gateway http-listener: se ha agregado --firewall-policy en la creación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-501">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="9fd5f-502">application-gateway url-path-map rule: se ha agregado --firewall-policy en la creación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-502">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="9fd5f-503">Packaging</span><span class="sxs-lookup"><span data-stu-id="9fd5f-503">Packaging</span></span>

* <span data-ttu-id="9fd5f-504">Se ha reescrito az wrapper en Python.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-504">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="9fd5f-505">Se ha agregado compatibilidad para Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-505">Added support for Python 3.8</span></span>
* <span data-ttu-id="9fd5f-506">Se ha cambiado a Python 3 para el paquete RPM.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-506">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-507">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-507">Profile</span></span>

* <span data-ttu-id="9fd5f-508">Se ha corregido el error al ejecutar `az login -u {} -p {}` con una cuenta Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-508">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="9fd5f-509">Se ha corregido el error `SSLError` al ejecutar `az login` detrás de un servidor proxy con certificado raíz autofirmado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-509">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="9fd5f-510">Corrección 10578: `az login` se bloquea cuando se inicia más de una instancia al mismo tiempo en Windows o WSL.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-510">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="9fd5f-511">Corrección 11059: `az login --allow-no-subscriptions` produce un error si hay suscripciones en el inquilino.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-511">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="9fd5f-512">Corrección 11238: después de cambiar el nombre de una suscripción, al iniciar sesión con MSI aparecerá dos veces la misma suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-512">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-513">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-513">RBAC</span></span>

* <span data-ttu-id="9fd5f-514">Corrección 10996: corrección del error para `--force-change-password-next-login` en `az ad user update` cuando no se especifica `--password`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-514">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="9fd5f-515">Redis</span><span class="sxs-lookup"><span data-stu-id="9fd5f-515">Redis</span></span>

* <span data-ttu-id="9fd5f-516">Corrección 2902: se impedía establecer configuraciones de memoria al actualizar la memoria caché de la SKU Básica.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-516">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="9fd5f-517">Reservations</span><span class="sxs-lookup"><span data-stu-id="9fd5f-517">Reservations</span></span>

* <span data-ttu-id="9fd5f-518">Actualización de la versión del SDK a la 0.6.0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-518">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="9fd5f-519">Se ha agregado información de detalles del plan de facturación después de llamar a Get-Gatalogs.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-519">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="9fd5f-520">Se ha agregado el nuevo comando `az reservations reservation-order calculate` para calcular el precio de una reserva.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-520">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="9fd5f-521">Se ha agregado el nuevo comando `az reservations reservation-order purchase` para adquirir una nueva reserva.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-521">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="9fd5f-522">Rest</span><span class="sxs-lookup"><span data-stu-id="9fd5f-522">Rest</span></span>
* <span data-ttu-id="9fd5f-523">Se ha cambiado `az rest` a Disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-523">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-524">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-524">SQL</span></span>

* <span data-ttu-id="9fd5f-525">Se ha actualizado azure-mgmt-sql a la versión 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-525">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-526">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-526">Storage</span></span>

* <span data-ttu-id="9fd5f-527">storage account create: se ha agregado --enable-hierarchical-namespace para admitir la semántica del sistema de archivos en Blob Service.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-527">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="9fd5f-528">Se ha eliminado la excepción no relacionada del mensaje de error.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-528">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="9fd5f-529">Se han corregido problemas con el mensaje de error incorrecto: "No tiene los permisos necesarios para realizar esta operación"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-529">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="9fd5f-530">en bloqueos de las reglas de red o en un error de autenticación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-530">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="9fd5f-531">4 de noviembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-531">November 4, 2019</span></span>

<span data-ttu-id="9fd5f-532">Versión 2.0.76</span><span class="sxs-lookup"><span data-stu-id="9fd5f-532">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-533">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-533">ACR</span></span>

* <span data-ttu-id="9fd5f-534">Se ha agregado un parámetro en versión preliminar `--pack-image-tag` al comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-534">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="9fd5f-535">Se ha agregado compatibilidad para habilitar la auditoría al crear un registro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-535">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="9fd5f-536">Se admite RBAC en el ámbito del repositorio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-536">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-537">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-537">AKS</span></span>

* <span data-ttu-id="9fd5f-538">Se han agregado `--enable-cluster-autoscaler`, `--min-count` y `--max-count` al comando `az aks create`, que habilita el escalador automático de clústeres para el grupo de nodos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-538">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="9fd5f-539">Se han agregado las marcas anteriores, así como `--update-cluster-autoscaler` y `--disable-cluster-autoscaler`, al comando `az aks update`, lo que permite actualizar el escalador automático de clústeres.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-539">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="9fd5f-540">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9fd5f-540">AppConfig</span></span>

* <span data-ttu-id="9fd5f-541">Se ha agregado el grupo de comandos de características appConfig para administrar las marcas de características almacenadas en una configuración de aplicación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-541">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="9fd5f-542">Se ha corregido un error secundario menor del comando de appconfig de exportación de almacén de claves a archivo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-542">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="9fd5f-543">Se deja de leer el contenido del archivo de destino durante la exportación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-543">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-544">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-544">AppService</span></span>

* <span data-ttu-id="9fd5f-545">`az appservice plan create`: Se ha agregado compatibilidad para establecer "persitescaling" en plan create de appservice.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-545">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="9fd5f-546">Se ha corregido un problema por el que la operación de enlace de SSL de configuración de aplicación web quitaba las etiquetas existentes del recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-546">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="9fd5f-547">Se ha agregado la marca `--build-remote` a `az functionapp deployment source config-zip` para admitir la acción de compilación remota durante la implementación de la aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-547">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="9fd5f-548">Se ha cambiado la versión predeterminada del nodo en las aplicaciones de función a ~10 para Windows.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-548">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="9fd5f-549">Se ha agregado la propiedad `--runtime-version` a `az functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-549">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-550">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-550">ARM</span></span>

* <span data-ttu-id="9fd5f-551">`az deployment/group deployment validate`: Se ha agregado el parámetro `--handle-extended-json-format` para admitir varias líneas y comentarios en la plantilla JSON durante la implementación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-551">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="9fd5f-552">Se ha incrementado la versión de azure-mgmt-resource a 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-552">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-553">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-553">Backup</span></span>

* <span data-ttu-id="9fd5f-554">Se ha agregado compatibilidad con la copia de seguridad de AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-554">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-555">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-555">Compute</span></span>

* <span data-ttu-id="9fd5f-556">`az vm create`: Se ha agregado una advertencia al especificar juntas redes aceleradas y una NIC existente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-556">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="9fd5f-557">`az vm create`: Se ha agregado `--vmss` para especificar un conjunto de escalado de máquinas virtuales existente al que se debe asignar la máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-557">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="9fd5f-558">`az vm/vmss create`: Se ha agregado una copia local del archivo de alias de imagen para poder tener acceso a él en un entorno de red restringido.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-558">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="9fd5f-559">`az vmss create`: Se ha agregado `--orchestration-mode` para especificar cómo se administran las máquinas virtuales mediante el conjunto de escalado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-559">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="9fd5f-560">`az vm/vmss update`: Se ha agregado `--ultra-ssd-enabled` para poder actualizar la configuración de SSD.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-560">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="9fd5f-561">[CAMBIO IMPORTANTE] `az vm extension set`: Se ha corregido un error por el que los usuarios no podían establecer una extensión en una máquina virtual con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-561">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="9fd5f-562">Se han agregado nuevos comandos `az vm image terms accept/cancel/show` para administrar los términos de la imagen de Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-562">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="9fd5f-563">Se ha actualizado VMAccessForLinux a la versión 1.5.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-563">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-564">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-564">CosmosDB</span></span>

* <span data-ttu-id="9fd5f-565">[CAMBIO IMPORTANTE] `az sql container create`: Se ha cambiado el parámetro `--partition-key-path` a obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-565">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="9fd5f-566">[CAMBIO IMPORTANTE] `az gremlin graph create`: Se ha cambiado el parámetro `--partition-key-path` a obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-566">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="9fd5f-567">`az sql container create`: Se han agregado `--unique-key-policy` y `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-567">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="9fd5f-568">`az sql container create/update`: Se ha actualizado el esquema predeterminado `--idx`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-568">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="9fd5f-569">`gremlin graph create`: Se agregó `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-569">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="9fd5f-570">`gremlin graph create/update`: Se ha actualizado el esquema predeterminado `--idx`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-570">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="9fd5f-571">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="9fd5f-571">Fixed typo in help message</span></span>
* <span data-ttu-id="9fd5f-572">base de datos: Se ha agregado información sobre el desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-572">database: Added deprecation information</span></span>
* <span data-ttu-id="9fd5f-573">colección: Se ha agregado información sobre el desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-573">collection: Added deprecation information</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-574">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-574">IoT</span></span>

* <span data-ttu-id="9fd5f-575">Se ha agregado un nuevo tipo de origen de enrutamiento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="9fd5f-575">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="9fd5f-576">Se han corregido las características que faltan en `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-576">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-577">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-577">Key Vault</span></span>

* <span data-ttu-id="9fd5f-578">Se ha corregido un error inesperado cuando el archivo de certificado no existe.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-578">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="9fd5f-579">Se ha corregido `az keyvault recover/purge` porque no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-579">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="9fd5f-580">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="9fd5f-580">NetAppFiles</span></span>

* <span data-ttu-id="9fd5f-581">Se ha actualizado azure-mgmt-netapp a 0.6.0 para usar la API versión 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-581">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="9fd5f-582">Esta nueva versión de API incluye:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-582">This new API version includes:</span></span>

    - <span data-ttu-id="9fd5f-583">La creación del volumen `--protocol-types` ahora acepta "NFSv4.1", no "NFSv4".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-583">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="9fd5f-584">La propiedad de directiva de exportación de volumen ahora tiene el nombre "nfsv41", no "nfsv4".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-584">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="9fd5f-585">Se ha cambiado el nombre del volumen `--creation-token` a `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-585">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="9fd5f-586">La fecha de creación de la instantánea ahora se llamada simplemente "created".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-586">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-587">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-587">Network</span></span>

* <span data-ttu-id="9fd5f-588">`az network private-dns link vnet create/update`: Se ha agregado compatibilidad con la vinculación de redes virtuales entre inquilinos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-588">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="9fd5f-589">[CAMBIO IMPORTANTE] `az network vnet subnet list`: Se han cambiado `--resource-group` y `--vnet-name` para que ahora sean obligatorios.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-589">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="9fd5f-590">`az network public-ip prefix create`: se ha agregado compatibilidad para especificar la versión de la dirección IP (IPv4, IPv6) durante la creación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-590">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="9fd5f-591">Se ha aumentado la versión de Azure-MGMT-Network a 7.0.0 y la versión de API a 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-591">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="9fd5f-592">`az network vrouter`: se ha agregado compatibilidad con un nuevo enrutador virtual de servicio y el emparejamiento de enrutador virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-592">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="9fd5f-593">`az network express-route gateway connection`: Se ha agregado compatibilidad con `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-593">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-594">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-594">Profile</span></span>

* <span data-ttu-id="9fd5f-595">Se ha corregido `az account get-access-token --resource-type ms-graph` porque no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-595">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="9fd5f-596">Se ha quitado la advertencia de `az login`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-596">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-597">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-597">RBAC</span></span>

* <span data-ttu-id="9fd5f-598">Se ha corregido `az ad app update --id {} --display-name {}` porque no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-598">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9fd5f-599">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-599">ServiceFabric</span></span>

* <span data-ttu-id="9fd5f-600">`az sf cluster create`: Se ha corregido un problema mediante la modificación de VMSS de proceso template.json Windows y Linux de Service Fabric de discos estándar a discos administrados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-600">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-601">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-601">SQL</span></span>

* <span data-ttu-id="9fd5f-602">Se han agregado los parámetros `--compute-model`, `--auto-pause-delay`y `--min-capacity` para admitir las operaciones CRUD para la nueva oferta de SQL Database: Modelo de proceso sin servidor.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-602">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-603">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-603">Storage</span></span>

* <span data-ttu-id="9fd5f-604">`az storage account create/update`: Se ha agregado el parámetro --enable-files-adds y el grupo de argumentos de propiedades de Azure Active Directory para admitir la autenticación de AD DS en Azure Files.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-604">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="9fd5f-605">Se ha expandido `az storage account keys list/renew` para admitir la enumeración o regeneración de claves Kerberos de la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-605">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="9fd5f-606">15 de octubre de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-606">October 15, 2019</span></span>

<span data-ttu-id="9fd5f-607">Versión 2.0.75</span><span class="sxs-lookup"><span data-stu-id="9fd5f-607">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-608">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-608">AKS</span></span>

* <span data-ttu-id="9fd5f-609">Se ha cambiado el valor predeterminado de `--load-balancer-sku` a `standard` si es compatible con la versión de Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-609">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="9fd5f-610">Se ha cambiado el valor predeterminado de `--vm-set-type` a `virtualmachinescalesets` si es compatible con la versión de Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-610">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-611">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-611">AMS</span></span>

* <span data-ttu-id="9fd5f-612">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `job start` a `job create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-612">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="9fd5f-613">[CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--ask` de `content-key-policy create` para que use una cadena hexadecimal de 32 caracteres en lugar de UTF8.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-613">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-614">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-614">AppService</span></span>

* <span data-ttu-id="9fd5f-615">Se han agregado comandos `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-615">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="9fd5f-616">Se ha agregado un mejor control de errores a `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-616">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="9fd5f-617">Se ha agregado compatibilidad para la SKU `Isolated` a `appservice plan update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-617">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-618">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-618">ARM</span></span>

* <span data-ttu-id="9fd5f-619">Se ha agregado el parámetro `--handle-extended-json-format` a `deployment create` para admitir varias líneas y comentarios en la plantilla JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-619">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-620">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-620">Compute</span></span>

* <span data-ttu-id="9fd5f-621">Se ha agregado el parámetro `--enable-agent` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-621">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="9fd5f-622">Se ha cambiado `vm create` para que use SKU de IP pública estándar automáticamente al usar zonas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-622">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="9fd5f-623">Se ha cambiado `vm create` para que cree automáticamente un nombre de equipo válido para una máquina virtual si no se proporciona ninguno.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-623">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="9fd5f-624">Se ha agregado el parámetro `--computer-name-prefix` a `vmss create` para admitir el prefijo de nombre de equipo personalizado de las máquinas virtuales en el VMSS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-624">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="9fd5f-625">Agregue el parámetro `--workspace` a `vm create` para habilitar automáticamente el área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-625">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="9fd5f-626">Se ha actualizado la versión de API de galerías a 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-626">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-627">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-627">Core</span></span>

* <span data-ttu-id="9fd5f-628">Se ha agregado la comprobación de la sintaxis del parámetro `--set` en el comando de actualización genérico.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-628">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-629">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-629">IoT</span></span>

* <span data-ttu-id="9fd5f-630">Se ha corregido un problema por el que `iot hub show` producía un error con el mensaje "recurso no encontrado".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-630">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-631">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-631">Monitor</span></span>

* <span data-ttu-id="9fd5f-632">Se ha agregado compatibilidad para CRUD a `monitor log-analytics workspace`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-632">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-633">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-633">Network</span></span>

* <span data-ttu-id="9fd5f-634">Se ha agregado compatibilidad para la vinculación virtual entre inquilinos a `network private-dns link vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-634">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="9fd5f-635">[CAMBIO IMPORTANTE] Se ha cambiado `network vnet subnet list` para requerir los parámetros `--resource-group` y `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-635">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-636">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-636">SQL</span></span>

* <span data-ttu-id="9fd5f-637">Se han agregado comandos a `sql mi ad-admin` que admiten la configuración de un administrador de AAD en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-637">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-638">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-638">Storage</span></span>

* <span data-ttu-id="9fd5f-639">Se ha agregado el parámetro `--preserve-s2s-access-tier` a `storage copy` para conservar el nivel de acceso durante la copia de servicio a servicio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-639">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="9fd5f-640">Se ha agregado el parámetro `--enable-large-file-share` a `storage account [create|update]` para admitir recursos compartidos de archivos grandes para la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-640">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="9fd5f-641">24 de septiembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-641">September 24, 2019</span></span>

<span data-ttu-id="9fd5f-642">Versión 2.0.74</span><span class="sxs-lookup"><span data-stu-id="9fd5f-642">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-643">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-643">ACR</span></span>

* <span data-ttu-id="9fd5f-644">Se ha agregado un parámetro `--type` obligatorio a `acr config retention update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-644">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="9fd5f-645">[CAMBIO IMPORTANTE] Se ha cambiado el nombre del parámetro `--name -n` a `--registry -r ` para el grupo de comandos `acr config`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-645">[BREAKING CHANGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-646">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-646">AKS</span></span>

* <span data-ttu-id="9fd5f-647">Se ha agregado el parámetro `--load-balancer-sku` al comando `aks create`, lo que permite crear un clúster de AKS con SLB.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-647">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="9fd5f-648">Se han agregado los parámetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` y `--load-balancer-outbound-ip-prefixes` a los comandos `aks [create|update]`, lo que permite actualizar el perfil del equilibrador de carga de un clúster de AKS con SLB.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-648">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="9fd5f-649">Se ha agregado el parámetro `--vm-set-type` al comando `aks create`, lo que permite especificar los tipos de máquina virtual de un clúster de AKS (vmas o vmss).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-649">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-650">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-650">ARM</span></span>

* <span data-ttu-id="9fd5f-651">Se ha agregado el parámetro `--handle-extended-json-format` al comando `group deployment create` para admitir varias líneas y comentarios en la plantilla JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-651">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-652">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-652">Compute</span></span>

* <span data-ttu-id="9fd5f-653">Se ha agregado el parámetro `--terminate-notification-time` a los comandos `vmss [create|update]` para poder finalizar la capacidad de configurar eventos programados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-653">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="9fd5f-654">Se ha agregado el parámetro `--enable-terminate-notification` al comando `vmss update` para poder finalizar la capacidad de configurar eventos programados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-654">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="9fd5f-655">Se han agregado los parámetros `--priority,` `--eviction-policy,` `--max-billing` a los comandos `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-655">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="9fd5f-656">Se ha cambiado `disk create` para permitir especificar el tamaño exacto de la carga del disco.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-656">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="9fd5f-657">Se ha agregado compatibilidad para instantáneas incrementales de discos administrados a `snapshot create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-657">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fd5f-658">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-658">Cosmos DB</span></span>

* <span data-ttu-id="9fd5f-659">Se ha agregado el parámetro `--type <key-type>` al comando `cosmosdb keys list` para mostrar la clave, las claves de solo lectura o las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-659">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="9fd5f-660">Se agregó el comando `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-660">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="9fd5f-661">[EN DESUSO] Se han dejado de usar los comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` y `cosmosdb list-read-only-keys`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-661">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9fd5f-662">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-662">EventGrid</span></span>

* <span data-ttu-id="9fd5f-663">Se ha corregido el texto de ayuda del punto de conexión para que haga referencia al parámetro correcto.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-663">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-664">Key Vault</span></span>

* <span data-ttu-id="9fd5f-665">Se ha corregido un problema por el que un inquilino (`login -t`) podía producir un error en `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-665">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-666">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-666">Monitor</span></span>

* <span data-ttu-id="9fd5f-667">Se ha corregido un problema por el que no se permitía el carácter `:` en el argumento `--condition` de `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-667">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="9fd5f-668">Directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-668">Policy</span></span>

* <span data-ttu-id="9fd5f-669">Se ha agregado compatibilidad con la versión 2019-06-01 de Policy API.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-669">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="9fd5f-670">Se ha agregado el parámetro `--enforcement-mode` al comando `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-670">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-671">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-671">Storage</span></span>

* <span data-ttu-id="9fd5f-672">Se ha agregado el parámetro `--blob-type` al comando `az storage copy`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-672">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="9fd5f-673">10 de septiembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-673">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-674">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-674">ACR</span></span>

* <span data-ttu-id="9fd5f-675">Se ha agregado el grupo de comandos `acr config retention` para configurar la directiva de retención.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-675">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-676">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-676">AKS</span></span>

* <span data-ttu-id="9fd5f-677">Se ha agregado compatibilidad para la integración de ACR con los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-677">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="9fd5f-678">Se ha agregado el parámetro `--attach-acr` a `aks [create|update]` para asociar un ACR a un clúster de AKS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-678">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="9fd5f-679">Se ha agregado el parámetro `--detach-acr` a `aks update` para desasociar un ACR de un clúster de AKS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-679">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-680">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-680">ARM</span></span>

* <span data-ttu-id="9fd5f-681">Se ha actualizado para usar la versión 2019-05-10 de la API.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-681">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-682">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-682">Batch</span></span>

* <span data-ttu-id="9fd5f-683">Se han agregado nuevas opciones de configuración de JSON a `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-683">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="9fd5f-684">Se ha agregado `MountConfigurations` para montajes del sistema de archivos (consulte https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obtener más información).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-684">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="9fd5f-685">Se ha agregado la propiedad `publicIPs` opcional en `NetworkConfiguration` para las direcciones IP públicas en grupos (consulte https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obtener más información).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-685">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="9fd5f-686">Se ha agregado compatibilidad para la galería de imágenes compartidas a `--image`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-686">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="9fd5f-687">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--start-task-wait-for-success` en `batch pool create` a `true`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-687">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="9fd5f-688">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `Scope` en `AutoUserSpecification` para que siempre sea Pool (era `Task` en los nodos Windows, `Pool` en los nodos Linux).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-688">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="9fd5f-689">Este argumento solo se puede establecer desde una configuración de JSON con `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-689">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-690">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-690">HDInsight</span></span>

* <span data-ttu-id="9fd5f-691">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="9fd5f-691">GA release</span></span>
* <span data-ttu-id="9fd5f-692">[CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--workernode-count/-c` de `az hdinsight resize` para que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-692">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-693">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-693">Key Vault</span></span>

* <span data-ttu-id="9fd5f-694">Se ha corregido un problema por el que no se podían eliminar las subredes de las reglas de red.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-694">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="9fd5f-695">Se ha corregido un problema por el que se podían agregar subredes y direcciones IP duplicadas a las reglas de red.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-695">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-696">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-696">Network</span></span>

* <span data-ttu-id="9fd5f-697">Se ha agregado el parámetro `--interval` a `network watcher flow-log` para establecer el valor del intervalo de análisis del tráfico.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-697">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="9fd5f-698">Se ha agregado `network application-gateway identity` para administrar la identidad de puerta de enlace.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-698">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="9fd5f-699">Se ha agregado compatibilidad para establecer el identificador del almacén de claves en `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-699">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="9fd5f-700">Se agregó `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-700">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="9fd5f-701">Directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-701">Policy</span></span>

* <span data-ttu-id="9fd5f-702">Se ha actualizado para usar la versión 2019-01-01 de la API.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-702">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="9fd5f-703">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-703">August 27, 2019</span></span>

<span data-ttu-id="9fd5f-704">Versión 2.0.72</span><span class="sxs-lookup"><span data-stu-id="9fd5f-704">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-705">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-705">ACR</span></span>

* <span data-ttu-id="9fd5f-706">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para la SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-706">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="9fd5f-707">API Management</span><span class="sxs-lookup"><span data-stu-id="9fd5f-707">API Management</span></span>

* <span data-ttu-id="9fd5f-708">[VERSIÓN PRELIMINAR] Se ha agregado el grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-708">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-709">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-709">AppService</span></span>

* <span data-ttu-id="9fd5f-710">Se ha corregido un problema con el comando `webapp webjob continuous start` al especificar una ranura</span><span class="sxs-lookup"><span data-stu-id="9fd5f-710">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="9fd5f-711">Se ha cambiado `webapp up` para detectar la carpeta `env` y quitarla del archivo usado para la implementación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-711">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-712">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-712">Keyvault</span></span>

* <span data-ttu-id="9fd5f-713">Se ha corregido un error en `keyvault secret set` que hacía que se ignorara el argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-713">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-714">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-714">Network</span></span>

* <span data-ttu-id="9fd5f-715">Se ha agregado compatibilidad para las direcciones IPv6 con argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-715">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="9fd5f-716">Se han agregado nuevos comandos `network private-endpoint [create|update|list-types]` para la administración de un punto de conexión privado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-716">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="9fd5f-717">Se ha agregado el grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-717">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="9fd5f-718">Se agregaron los argumentos `--private-endpoint-network-policies` y `--private-link-service-network-policies` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-718">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-719">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-719">RBAC</span></span>

* <span data-ttu-id="9fd5f-720">Se ha corregido el problema con `ad app update --homepage` por el cual la página principal no se actualizaba</span><span class="sxs-lookup"><span data-stu-id="9fd5f-720">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9fd5f-721">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-721">ServiceFabric</span></span>

* <span data-ttu-id="9fd5f-722">Se ha agregado compatibilidad con los nombres de Key Vault que combinan mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-722">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="9fd5f-723">Se ha solucionado el problema que se producía al usar certificados en Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-723">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="9fd5f-724">Se ha solucionado el problema con el uso de archivos de certificado de PFX</span><span class="sxs-lookup"><span data-stu-id="9fd5f-724">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="9fd5f-725">Se ha solucionado el problema con `sf cluster certificate add` que se producía cuando no se especificaba el grupo de recursos de Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-725">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="9fd5f-726">Se ha corregido el problema con `sf cluster set` que no funcionaba</span><span class="sxs-lookup"><span data-stu-id="9fd5f-726">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="9fd5f-727">SignalR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-727">SignalR</span></span>

* <span data-ttu-id="9fd5f-728">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-728">Added new commands:</span></span>
  * <span data-ttu-id="9fd5f-729">`signalr cors`: Administración de SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-729">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="9fd5f-730">`signalr restart`: Reinicio de una instancia de SignalR Service</span><span class="sxs-lookup"><span data-stu-id="9fd5f-730">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="9fd5f-731">`signalr update`: Actualización de una instancia de SignalR Service</span><span class="sxs-lookup"><span data-stu-id="9fd5f-731">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="9fd5f-732">Se agregó el argumento `--service-mode` a `signalr create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-732">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-733">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-733">Storage</span></span>

* <span data-ttu-id="9fd5f-734">Se agregó el comando `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-734">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="9fd5f-735">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-735">August 13, 2019</span></span>

<span data-ttu-id="9fd5f-736">Versión 2.0.71</span><span class="sxs-lookup"><span data-stu-id="9fd5f-736">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-737">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-737">AppService</span></span>

* <span data-ttu-id="9fd5f-738">Se ha corregido un problema por el que se producían errores con los comandos `webapp webjob continuous` en los espacios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-738">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-739">BotService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-739">BotService</span></span>

* <span data-ttu-id="9fd5f-740">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para crear bots con el SDK v3.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-740">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="9fd5f-741">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9fd5f-741">CognitiveServices</span></span>

* <span data-ttu-id="9fd5f-742">Se agregaron los comandos `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-742">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fd5f-743">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-743">Cosmos DB</span></span>

* <span data-ttu-id="9fd5f-744">Se ha quitado la advertencia al actualizar varias ubicaciones de escritura.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-744">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="9fd5f-745">Se han agregado comandos CRUD para recursos de CosmosDB SQL, MongoDB, Cassandra, Gremlin y Table, así como capacidad de proceso para los recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-745">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-746">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-746">HDInsight</span></span>

<span data-ttu-id="9fd5f-747">Esta versión contiene un gran número de cambios importantes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-747">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="9fd5f-748">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-748">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="9fd5f-749">Cambio de nombre de `--storage-default-container` a `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-749">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="9fd5f-750">Cambio de nombre de `--storage-default-filesystem` a `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-750">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="9fd5f-751">[CAMBIO IMPORTANTE] Se ha cambiado el argumento `--name` de `application create` para que represente el nombre de la aplicación en lugar del nombre del clúster.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-751">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="9fd5f-752">Se ha agregado el argumento `--cluster-name` a `application create` para reemplazar la funcionalidad de `--name` antigua.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-752">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="9fd5f-753">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `application create`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-753">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="9fd5f-754">Cambio de nombre de `--application-type` a `--type`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-754">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="9fd5f-755">Cambio de nombre de `--marketplace-identifier` a `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-755">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="9fd5f-756">Cambio de nombre de `--https-endpoint-access-mode` a `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-756">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="9fd5f-757">Se cambió el nombre de `--https-endpoint-destination-port` a `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-757">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="9fd5f-758">[CAMBIO IMPORTANTE] Se han quitado los parámetros de `application create`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-758">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="9fd5f-759">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--target-instance-count` a `--workernode-count` para `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-759">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="9fd5f-760">[CAMBIO IMPORTANTE] Se han cambiado todos los comandos del grupo `hdinsight script-action` para que usen el parámetro `--name` como nombre de la acción de script.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-760">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="9fd5f-761">Se ha agregado el argumento `--cluster-name` a todos los comandos `hdinsight script-action` para reemplazar la funcionalidad de `--name` antigua.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-761">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="9fd5f-762">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--script-execution-id` a `--execution-id` para todos los comandos `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-762">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="9fd5f-763">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `hdinsight script-action show` a `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-763">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="9fd5f-764">[CAMBIO IMPORTANTE] Se han cambiado los parámetros a `hdinsight script-action execute --roles` para que estén separados por espacios en lugar de por comas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-764">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="9fd5f-765">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--persisted` de `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-765">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="9fd5f-766">Se ha cambiado el parámetro `hdinsight create --cluster-configurations` para aceptar una ruta a un archivo JSON local o una cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-766">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="9fd5f-767">Se ha agregado el comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-767">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="9fd5f-768">Se ha cambiado `hdinsight monitor enable --workspace` para aceptar un identificador o un nombre de área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-768">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="9fd5f-769">Se ha agregado el argumento `hdinsight monitor enable --primary-key`, que es necesario si se proporciona un identificador de área de trabajo como parámetro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-769">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="9fd5f-770">Se han agregado más ejemplos y se han actualizado las descripciones para los mensajes de ayuda.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-770">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-771">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-771">Interactive</span></span>

* <span data-ttu-id="9fd5f-772">Se ha corregido un error de carga.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-772">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="9fd5f-773">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-773">Kubernetes</span></span>

* <span data-ttu-id="9fd5f-774">Se ha cambiado para usar `https` si el puerto del contenedor del panel usa `https`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-774">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-775">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-775">Network</span></span>

* <span data-ttu-id="9fd5f-776">Se ha agregado el argumento `network dns record-set cname delete` a `--yes`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-776">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-777">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-777">Profile</span></span>

* <span data-ttu-id="9fd5f-778">Se ha agregado el argumento `--resource-type` a `account get-access-token` para obtener los tokens de acceso a recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-778">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9fd5f-779">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-779">ServiceFabric</span></span>

* <span data-ttu-id="9fd5f-780">Se han agregado todas las versiones del sistema operativo compatible para la creación de clústeres SF.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-780">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="9fd5f-781">Se ha corregido el error de validación de certificado principal.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-781">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-782">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-782">Storage</span></span>

* <span data-ttu-id="9fd5f-783">Se ha agregado el comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-783">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="9fd5f-784">30 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-784">July 30, 2019</span></span>

<span data-ttu-id="9fd5f-785">Versión 2.0.70</span><span class="sxs-lookup"><span data-stu-id="9fd5f-785">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-786">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-786">ACR</span></span>

* <span data-ttu-id="9fd5f-787">Se ha corregido el problema 9952 (una regresión en el comando `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-787">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="9fd5f-788">Se ha quitado el nombre predeterminado de la imagen del generador en `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-788">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-789">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-789">Appservice</span></span>

* <span data-ttu-id="9fd5f-790">Se ha cambiado `webapp config ssl` para que muestre un mensaje si no se encuentra un recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-790">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="9fd5f-791">Se ha corregido un problema por el que `functionapp create` no acepta el tipo de cuenta de almacenamiento `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-791">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="9fd5f-792">Se ha corregido un problema por el que `webapp up` producía un error si se ejecutaba con versiones anteriores de Python.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-792">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-793">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-793">Network</span></span>

* <span data-ttu-id="9fd5f-794">Se ha quitado un parámetro no válido `--ids` de `network nic ip-config add` (corrige el problema 9861).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-794">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="9fd5f-795">Corrige el problema 9604.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-795">Fixes #9604.</span></span> <span data-ttu-id="9fd5f-796">Se ha agregado el parámetro `--root-certs` a `network application-gateway http-settings [create|update]` para admitir los certificados raíz de confianza de los usuarios asociados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-796">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="9fd5f-797">Se ha corregido el argumento `--subscription` para `network dns record-set ns create` (9965).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-797">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-798">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-798">RBAC</span></span>

* <span data-ttu-id="9fd5f-799">Se agregó el comando `user update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-799">Added `user update` command</span></span>
* <span data-ttu-id="9fd5f-800">[EN DESUSO] Se ha dejado de usar `--upn-or-object-id` en los comandos relacionados con el usuario.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-800">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="9fd5f-801">Use el nuevo argumento `--id`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-801">Use replacement argument `--id`</span></span>
* <span data-ttu-id="9fd5f-802">Se ha agregado el argumento `--id` a los comandos relacionados con el usuario.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-802">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-803">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-803">SQL</span></span>

* <span data-ttu-id="9fd5f-804">Se han agregado comandos de administración para claves de instancia administrada y protector de TDE.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-804">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-805">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-805">Storage</span></span>

* <span data-ttu-id="9fd5f-806">Se agregó el comando `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-806">Added `storage remove` command</span></span>
* <span data-ttu-id="9fd5f-807">Se ha corregido un error con `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-807">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-808">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-808">VM</span></span>

* <span data-ttu-id="9fd5f-809">Se ha cambiado `list-skus` para que use la versión más reciente de la API para generar los detalles de la zona.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-809">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="9fd5f-810">Se ha cambiado el valor predeterminado de `--single-placement-group` a `false` para `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-810">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="9fd5f-811">Se ha agregado la posibilidad de seleccionar SKU de almacenamiento ZRS para `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-811">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="9fd5f-812">Se ha agregado un nuevo grupo de comandos `vm host` para admitir hosts dedicados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-812">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="9fd5f-813">Se han agregado los parámetros `--host` y `--host-group` en `vm create` para establecer un host dedicado de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-813">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="9fd5f-814">16 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-814">July 16, 2019</span></span>

<span data-ttu-id="9fd5f-815">Versión 2.0.69</span><span class="sxs-lookup"><span data-stu-id="9fd5f-815">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-816">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-816">Appservice</span></span>

* <span data-ttu-id="9fd5f-817">Se han cambiado los comandos de `webapp identity` para devolver un mensaje de error adecuado si el nombre del grupo de recursos o la aplicación no es válido.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-817">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="9fd5f-818">Se ha corregido `webapp list` para devolver el valor correcto de numberOfSites si no se ha proporcionado ningún grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-818">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="9fd5f-819">Se han corregido los efectos secundarios de `appservice plan create` y `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-819">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-820">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-820">Core</span></span>

* <span data-ttu-id="9fd5f-821">Se ha corregido el problema por el que `--subscription` aparecía a pesar de no ser aplicable.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-821">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-822">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-822">Batch</span></span>

* <span data-ttu-id="9fd5f-823">[CAMBIO IMPORTANTE] Se ha reemplazado `batch pool node-agent-skus list` por `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-823">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="9fd5f-824">Se ha agregado compatibilidad con las reglas de seguridad que bloquea el acceso de red a un grupo basado en el puerto de origen del tráfico cuando se usa la opción `--json-file` de `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-824">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="9fd5f-825">Agrega compatibilidad para ejecutar la tarea en el directorio de trabajo del contenedor o en el directorio de trabajo de la tarea por lotes cuando se usa la opción `--json-file` de `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-825">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="9fd5f-826">Se ha corregido el error en la opción `--application-package-references` de `batch pool create` por el que solo funcionaba con los valores predeterminados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-826">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9fd5f-827">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9fd5f-827">Eventhubs</span></span>

* <span data-ttu-id="9fd5f-828">Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-828">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-829">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-829">RDBMS</span></span>

* <span data-ttu-id="9fd5f-830">Se ha agregado un parámetro opcional para especificar la SKU de réplica para crear comandos de réplica.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-830">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="9fd5f-831">Se ha corregido el problema con el error de prueba de CI al crear la réplica de MySQL.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-831">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="9fd5f-832">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-832">Relay</span></span>

* <span data-ttu-id="9fd5f-833">Se ha corregido el problema con la conexión híbrida cuando la autorización del cliente está deshabilitada [n.º 8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-833">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="9fd5f-834">Se ha agregado el parámetro `--requires-transport-security` a `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-834">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9fd5f-835">Servicebus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-835">Servicebus</span></span>

* <span data-ttu-id="9fd5f-836">Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-836">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-837">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-837">Storage</span></span>

* <span data-ttu-id="9fd5f-838">Habilitar archivos AADDS para la actualización de la cuenta de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="9fd5f-838">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="9fd5f-839">Se ha corregido el problema `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-839">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="9fd5f-840">2 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-840">July 2, 2019</span></span>

<span data-ttu-id="9fd5f-841">Versión 2.0.68</span><span class="sxs-lookup"><span data-stu-id="9fd5f-841">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-842">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-842">Core</span></span>

* <span data-ttu-id="9fd5f-843">Los módulos de comandos ahora se consolidan en un único paquete distribuible de Python.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-843">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="9fd5f-844">Esto reemplaza el uso directo de muchos paquetes `azure-cli-` en PyPI.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-844">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="9fd5f-845">Esto reducirá el tamaño de la instalación y solo afecta a los usuarios que hayan instalado directamente mediante `pip`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-845">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-846">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-846">ACR</span></span>

* <span data-ttu-id="9fd5f-847">Se ha agregado compatibilidad para los desencadenadores de temporizador para las tareas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-847">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-848">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-848">Appservice</span></span>

* <span data-ttu-id="9fd5f-849">Se ha cambiado `functionapp create` para habilitar Application Insights de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-849">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="9fd5f-850">[CAMBIO IMPORTANTE] Se ha dejado de utilizar el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-850">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="9fd5f-851">Use el nuevo comando `az functionapp devops-pipeline` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-851">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="9fd5f-852">Se ha agregado compatibilidad con el plan de aplicación de funciones Consumo para Linux a `functionapp deployment config-zip`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-852">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fd5f-853">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-853">Cosmos DB</span></span>

* <span data-ttu-id="9fd5f-854">Se ha agregado compatibilidad para deshabilitar TTL.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-854">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="9fd5f-855">DLS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-855">DLS</span></span>

* <span data-ttu-id="9fd5f-856">Se ha actualizado la versión de ADLS (0.0.45).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-856">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="9fd5f-857">Comentarios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-857">Feedback</span></span>

* <span data-ttu-id="9fd5f-858">Al informar de un error de comando de extensión, `az feedback` ahora intenta abrir el explorador en la dirección URL del repositorio del proyecto de la extensión desde el índice.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-858">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-859">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-859">HDInsight</span></span>

* <span data-ttu-id="9fd5f-860">[CAMBIO IMPORTANTE] Se ha cambiado el nombre del grupo de comandos `oms` por `monitor`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-860">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="9fd5f-861">[CAMBIO IMPORTANTE] Ahora `--http-password/-p` es un parámetro necesario.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-861">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="9fd5f-862">Se han agregado completadores para los parámetros `--cluster-admin-account` y `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-862">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="9fd5f-863">Se ha cambiado el parámetro `cluster-users-group-dns` para que sea necesario cuando `—esp` está presente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-863">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="9fd5f-864">Se ha agregado un tiempo de espera para todos los autocompletadores de argumentos existentes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-864">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="9fd5f-865">Se ha agregado un tiempo de espera para transformar el nombre de recurso en un identificador de recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-865">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="9fd5f-866">Se han cambiado los autocompletadores para seleccionar recursos de cualquier grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-866">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="9fd5f-867">Puede ser un grupo de recursos diferente a que se especifica con `-g`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-867">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="9fd5f-868">Se ha agregado compatibilidad con los parámetros `--sub-domain-suffix` y `--disable_gateway_auth` en el comando `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-868">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="9fd5f-869">Servicios administrados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-869">Managed Services</span></span>

* <span data-ttu-id="9fd5f-870">Se ha introducido un módulo de comandos de servicios administrados en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-870">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-871">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-871">Profile</span></span>
* <span data-ttu-id="9fd5f-872">Se ha suprimido el argumento `--subscription` del comando de cierre de sesión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-872">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-873">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-873">RBAC</span></span>

* <span data-ttu-id="9fd5f-874">[CAMBIO IMPORTANTE] Se ha quitado el argumento `--password` de `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-874">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="9fd5f-875">Se ha agregado el parámetro `--assignee-principal-type` al comando `create` para evitar errores intermitentes causados por la latencia de replicación del servidor de grafos de AAD.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-875">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="9fd5f-876">Se ha corregido un bloqueo en `ad signed-in-user` al enumerar los objetos que posee.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-876">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="9fd5f-877">Se ha corregido el problema por el que `ad sp` no encontraba la aplicación correcta en una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-877">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-878">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-878">RDBMS</span></span>

* <span data-ttu-id="9fd5f-879">Se ha agregado compatibilidad para la replicación a MariaDB.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-879">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-880">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-880">SQL</span></span>

* <span data-ttu-id="9fd5f-881">Se han documentado los valores permitidos para `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-881">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-882">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-882">Storage</span></span>

* <span data-ttu-id="9fd5f-883">Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-883">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="9fd5f-884">Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-884">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="9fd5f-885">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-885">VM</span></span>

* <span data-ttu-id="9fd5f-886">Se ha corregido un error por el que `vmss create` devuelve un mensaje de error cuando se ejecuta con `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-886">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="9fd5f-887">Se ha quitado la validación del lado cliente para `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-887">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="9fd5f-888">No genera ningún error si `--single-placement-group` está establecido en `true` y `--instance-count` es mayor que 100 o se especifican zonas de disponibilidad, y deja esta validación al servicio de proceso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-888">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="9fd5f-889">Se ha corregido el error por el que `[vm|vmss] extension image list` produce un error cuando se usa con `--latest`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-889">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="9fd5f-890">18 de junio de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-890">June 18, 2019</span></span>

<span data-ttu-id="9fd5f-891">Versión 2.0.67</span><span class="sxs-lookup"><span data-stu-id="9fd5f-891">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-892">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-892">Core</span></span>

<span data-ttu-id="9fd5f-893">Esta versión introduce una nueva etiqueta [Preview] para indicar con mayor claridad a los clientes si un grupo de comandos, un comando o un argumento está en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-893">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="9fd5f-894">Antes esto se comunicaba en el texto de ayuda o se indicaba explícitamente en el número de versión del módulo de comandos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-894">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="9fd5f-895">La CLI eliminará los números de versión de los paquetes individuales en el futuro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-895">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="9fd5f-896">Si un comando está en versión preliminar, todos sus argumentos también lo están.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-896">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="9fd5f-897">Si un grupo de comandos está etiquetado como versión preliminar, se consideran que todos los comandos y argumentos también están en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-897">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="9fd5f-898">Como resultado de este cambio, pueden parecer que varios grupos de comandos están "repentinamente" en versión preliminar con esta versión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-898">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="9fd5f-899">Lo que realmente ha sucede es que la mayoría de los paquetes estaban en versión preliminar, pero se considera que están disponibles con carácter general con esta versión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-899">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-900">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-900">ACR</span></span>
* <span data-ttu-id="9fd5f-901">Se ha agregado el comando "acr check-health".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-901">Added 'acr check-health' command</span></span>
* <span data-ttu-id="9fd5f-902">Mejor control de los errores para los tokens AAD y para recuperar los comandos externos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-902">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-903">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-903">ACS</span></span>
* <span data-ttu-id="9fd5f-904">Los comandos en desuso de ACS ya no se muestran en la vista de la ayuda.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-904">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-905">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-905">AMS</span></span>
* <span data-ttu-id="9fd5f-906">[CAMBIO IMPORTANTE] Las cadenas de hora ISO 8601 se han cambiado para volver a archive-window-length y key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-906">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-907">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-907">AppService</span></span>
* <span data-ttu-id="9fd5f-908">Se ha agregado el enrutamiento basado en la ubicación para `webapp deleted list` y `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-908">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="9fd5f-909">Se ha corregido el problema por el que no se podía hacer clic la dirección URL de destino registrada de la aplicación web ("Puede iniciar la aplicación en...") en Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-909">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="9fd5f-910">Se ha corregido el problema por el que, al crear aplicaciones con algunas SKU, se producía un error de AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-910">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="9fd5f-911">Se ha agregado validación previa a `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-911">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="9fd5f-912">Se ha corregido `[webapp|functionapp] traffic-routing` para usar el valor correcto de actionHostName.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-912">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="9fd5f-913">Se ha agregado compatibilidad con ranuras a los comandos `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-913">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-914">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-914">Batch</span></span>
* <span data-ttu-id="9fd5f-915">Se ha corregido la regresión de autenticación de AAD causada por una notificación demasiado agresiva de errores de autenticación de clave compartida.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-915">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="9fd5f-916">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-916">BatchAI</span></span>
* <span data-ttu-id="9fd5f-917">Los comandos de BatchAI han dejado de usarse y están ocultos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-917">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-918">BotService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-918">BotService</span></span>
* <span data-ttu-id="9fd5f-919">Se ha agregado un aviso de advertencia "compatibilidad descontinuada" o "modo de mantenimiento" a los comandos que admiten el SDK v3.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-919">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-920">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-920">CosmosDB</span></span>
* <span data-ttu-id="9fd5f-921">[EN DESUSO] Se ha dejado de usar el comando `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-921">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="9fd5f-922">Se ha agregado el comando `cosmosdb keys list`, que reemplaza a `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-922">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="9fd5f-923">`cosmsodb create/update`: Se ha agregado el nuevo formato a --location para poder establecer la propiedad "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-923">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="9fd5f-924">Formato antiguo en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-924">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9fd5f-925">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-925">EventGrid</span></span>
* <span data-ttu-id="9fd5f-926">Se han agregado comandos `eventgrid domain` para las operaciones CRUD de dominios.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-926">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="9fd5f-927">Se han agregado comandos `eventgrid domain topic` para las operaciones CRUD de temas de dominio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-927">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="9fd5f-928">Se ha agregado el argumento `--odata-query` a `eventgrid [topic|event-subscription] list` para filtrar los resultados mediante la sintaxis de OData.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-928">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="9fd5f-929">`event-subscription create/update`: Se ha agregado servicebusqueue como nuevos valores para el parámetro `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-929">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="9fd5f-930">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para `--included-event-types All` con `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-930">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-931">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-931">HDInsight</span></span>
* <span data-ttu-id="9fd5f-932">Se ha agregado compatibilidad con el parámetro `--ssh-public-key` al comando `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-932">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-933">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-933">IoT</span></span>
* <span data-ttu-id="9fd5f-934">Se ha agregado compatibilidad para volver a generar las claves de directiva de autorización.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-934">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="9fd5f-935">Se ha agregado un SDK y compatibilidad con el servicio de aprovisionamiento de repositorio de DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-935">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-936">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-936">Network</span></span>
* <span data-ttu-id="9fd5f-937">Se ha agregado compatibilidad de las zonas con puertas de enlace NAT.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-937">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="9fd5f-938">Se ha agregado el comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-938">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="9fd5f-939">Se ha corregido el problema con `dns zone import` por el que los usuarios no podían importar registros A con caracteres comodín.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-939">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="9fd5f-940">Se ha corregido el problema con `watcher flow-log configure` por el que no se podía habilitar el registro de flujos en determinadas regiones.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-940">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-941">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-941">Resource</span></span>
* <span data-ttu-id="9fd5f-942">Se ha agregado el comando `az rest` para hacer llamadas de REST.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-942">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="9fd5f-943">Se ha corregido el error al usar `policy assignment list` con un grupo de recursos o un nivel de suscripción `--scope`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-943">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9fd5f-944">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-944">ServiceBus</span></span>
* <span data-ttu-id="9fd5f-945">Se ha corregido el error con `servicebus topic create --max-size` [9319](https://github.com/azure/azure-cli/issues/9319).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-945">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-946">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-946">SQL</span></span>
* <span data-ttu-id="9fd5f-947">Se ha cambiado `--location` para que sea opcionalpara `sql [server|mi] create`; usa la ubicación del grupo de recursos si no se especifica.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-947">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="9fd5f-948">Se ha corregido el error "No se puede iterar en el objeto NoneType" para `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-948">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="9fd5f-949">SQLVm</span><span class="sxs-lookup"><span data-stu-id="9fd5f-949">SQLVm</span></span>
* <span data-ttu-id="9fd5f-950">[CAMBIO IMPORTANTE] Se ha cambiado `sql vm create` para requerir el parámetro `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-950">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="9fd5f-951">Se ha cambiado para poder establecer el SKU de la imagen de SQL al crear o actualizar una máquina virtual de SQL.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-951">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-952">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-952">Storage</span></span>
* <span data-ttu-id="9fd5f-953">Se ha corregido un problema con una clave de cuenta que falta para `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-953">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="9fd5f-954">Se ha corregido un problema con `storage blob sync` en Linux.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-954">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-955">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-955">VM</span></span>
* <span data-ttu-id="9fd5f-956">[VERSIÓN PRELIMINAR] Se han agregado los comandos `vm image template` para compilar imágenes de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-956">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="9fd5f-957">4 de junio de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-957">June 4, 2019</span></span>

<span data-ttu-id="9fd5f-958">Versión 2.0.66</span><span class="sxs-lookup"><span data-stu-id="9fd5f-958">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-959">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-959">Core</span></span>
* <span data-ttu-id="9fd5f-960">Se ha corregido el problema por el que los comandos generan un error si `--output yaml` se usa con `--query`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-960">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-961">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-961">ACR</span></span>
* <span data-ttu-id="9fd5f-962">Se ha agregado el grupo de comandos "acr pack" para crear tareas de compilación rápida mediante Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-962">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-963">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-963">ACS</span></span>
* <span data-ttu-id="9fd5f-964">Se permite habilitar o deshabilitar el complemento kube-dashboard de AKS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-964">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="9fd5f-965">Se imprime un mensaje descriptivo cuando la suscripción no está en la lista de permitidos para usar Azure Red Hat OpenShift.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-965">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-966">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-966">Batch</span></span>
* <span data-ttu-id="9fd5f-967">Se ha mejorado el control de errores cuando no se ha iniciado sesión en una cuenta \[[9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="9fd5f-967">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-968">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-968">IoT</span></span>
* <span data-ttu-id="9fd5f-969">Se ha agregado compatibilidad para la conmutación por error manual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-969">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-970">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-970">Network</span></span>
* <span data-ttu-id="9fd5f-971">Se han agregado comandos `network application-gateway waf-policy` para admitir reglas personalizadas de WAF.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-971">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="9fd5f-972">Se agregaron los argumentos `--waf-policy` y `--max-capacity` a `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-972">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="9fd5f-973">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-973">Resource</span></span>
* <span data-ttu-id="9fd5f-974">Se ha mejorado el mensaje de error de `deployment create` cuando TTY no está disponible.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-974">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-975">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-975">Role</span></span>
* <span data-ttu-id="9fd5f-976">Texto de ayuda actualizado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-976">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-977">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-977">Compute</span></span>
* <span data-ttu-id="9fd5f-978">Se ha agregado compatibilidad a `vm create` para máquinas virtuales desde una imagen administrada con LUN de discos de datos que no comienzan en 0 o que omiten los números.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-978">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="9fd5f-979">21 de mayo de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-979">May 21, 2019</span></span>

<span data-ttu-id="9fd5f-980">Versión 2.0.65</span><span class="sxs-lookup"><span data-stu-id="9fd5f-980">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-981">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-981">Core</span></span>
* <span data-ttu-id="9fd5f-982">Se han agregado mejores comentarios para los errores de autenticación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-982">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="9fd5f-983">Se ha corregido un problema por el que la CLI cargaba extensiones que no eran compatibles con su versión principal.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-983">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="9fd5f-984">Se ha corregido un problema con el inicio cuando `clouds.config` estaba dañado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-984">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-985">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-985">ACR</span></span>
* <span data-ttu-id="9fd5f-986">Se ha agregado compatibilidad para identidades administradas a Tareas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-986">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-987">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-987">ACS</span></span>
* <span data-ttu-id="9fd5f-988">Se ha corregido el comando `openshift create` cuando se usa con el cliente AAD.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-988">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-989">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-989">AppService</span></span>
* <span data-ttu-id="9fd5f-990">[EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`; se quitará en la próxima versión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-990">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="9fd5f-991">Se ha cambiado `functionapp devops-pipeline` para recopilar el registro de compilación de Azure DevOps en modo detallado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-991">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="9fd5f-992">[CAMBIO IMPORTANTE] Se ha eliminado la marca `--use_local_settings` del comando `functionapp devops-pipeline`; no era operativa.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-992">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="9fd5f-993">Se ha cambiado `webapp up` para que devuelva la salida JSON si no se usa `--logs`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-993">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="9fd5f-994">Se ha agregado compatibilidad para escribir los recursos predeterminados en la configuración local para `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-994">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="9fd5f-995">Se ha agregado compatibilidad para `webapp up` para volver a implementar una aplicación sin usar el argumento `--location`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-995">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="9fd5f-996">Se ha corregido un problema por el que, al crear un ASP en la SKU gratuita de Linux, el valor de SKU "Fee" no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-996">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-997">BotService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-997">BotService</span></span>
* <span data-ttu-id="9fd5f-998">Se ha cambiado para permitir las mayúsculas y minúsculas para los parámetros `--lang` de los comandos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-998">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="9fd5f-999">Se ha actualizado la descripción para el módulo de comandos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-999">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="9fd5f-1000">Consumo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1000">Consumption</span></span>
* <span data-ttu-id="9fd5f-1001">Se ha agregado un parámetro obligatorio que faltaba al ejecutar `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1001">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-1002">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1002">IoT</span></span>
* <span data-ttu-id="9fd5f-1003">Se ha agregado compatibilidad para enumerar todas las claves.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1003">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1004">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1004">Network</span></span>
* [CAMBIO IMPORTANTE]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="9fd5f-1006">Se ha agregado el argumento `--nat-gateway` a `network vnet subnet [create|update]` para adjuntar a una puerta de enlace NAT.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1006">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="9fd5f-1007">Se ha corregido el problema con `dns zone import` por el que los nombres de registro no encontraban un tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1007">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-1008">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1008">RDBMS</span></span>
* <span data-ttu-id="9fd5f-1009">Se ha agregado compatibilidad con replicación geográfica a mysql y postgres.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1009">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-1010">RBAC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1010">RBAC</span></span>
* <span data-ttu-id="9fd5f-1011">Se ha agregado compatibilidad para el ámbito de grupos de administración a `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1011">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1012">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1012">Storage</span></span>
* <span data-ttu-id="9fd5f-1013">`storage blob sync`: se ha agregado el comando sync a Blob Storage.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1013">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="9fd5f-1014">Proceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1014">Compute</span></span>
* <span data-ttu-id="9fd5f-1015">Se ha agregado `--computer-name` a `vm create` para establecer el nombre de equipo de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1015">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="9fd5f-1016">Se ha cambiado el nombre de `--ssh-key-value` a `--ssh-key-values` para `[vm|vmss] create`; ahora pueden aceptar varios valores ssh de clave pública o rutas de acceso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1016">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="9fd5f-1017">__Nota__: Este **no** es un cambio importante. `--ssh-key-value` se analizará correctamente porque solo coincide con `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1017">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="9fd5f-1018">Se ha cambiado el argumento `--type` de `ppg create` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1018">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="9fd5f-1019">6 de mayo de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1019">May 6, 2019</span></span>

<span data-ttu-id="9fd5f-1020">Versión 2.0.64</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1020">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1021">ACS</span></span>
* <span data-ttu-id="9fd5f-1022">[CAMBIO IMPORTANTE] Se ha eliminado la marca `--fqdn` de los comandos `openshift`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1022">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="9fd5f-1023">Se ha cambiado para usar la versión GA de la API Openshift de Azure Red Hat.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1023">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="9fd5f-1024">Se ha agregado la marca `customer-admin-group-id` a `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1024">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="9fd5f-1025">[GA] Se ha quitado `(PREVIEW)` de la opción `--network-policy` de `aks create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1025">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1026">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1026">Appservice</span></span>
* <span data-ttu-id="9fd5f-1027">[EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1027">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="9fd5f-1028">Se ha cambiado el nombre a `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1028">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="9fd5f-1029">Se ha corregido un error por el que no se podía obtener el nombre de usuario correcto para cloudshell, lo que provocaba un error de `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1029">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="9fd5f-1030">Se ha actualziado la documentación de `appservice plan --sku` para incluir la compatibilidad con appserviceplans.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1030">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="9fd5f-1031">Se han agregado argumentos opcionales para el grupo de recursos y el plan a `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1031">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="9fd5f-1032">Se ha agregado compatibilidad a `webapp ssh` para respetar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1032">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="9fd5f-1033">Se ha agregado compatibilidad a `appserviceplan create` con la SKU gratuita de Linux.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1033">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="9fd5f-1034">Se ha cambiado `webapp up` para que haya una suspensión de 30 segundos después de configurar la opción `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para controlar el inicio en frío de kudu.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1034">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="9fd5f-1035">Se ha agregado compatibilidad con el entorno de ejecución `powershell` a `functionapp create` en Windows.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1035">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="9fd5f-1036">Se agregó el comando `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1036">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-1037">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1037">Batch</span></span>
* <span data-ttu-id="9fd5f-1038">Se ha corregido un error en el validador para las opciones de `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1038">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-1039">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1039">Botservice</span></span>
* <span data-ttu-id="9fd5f-1040">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para crear un bot de Web App vacío de forma predeterminada (es decir, el bot no se implementa en App Service).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1040">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="9fd5f-1041">Se ha agregado la marca `--echo` a `bot create` para usar el comportamiento anterior con `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1041">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="9fd5f-1042">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--version` a `v4`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1042">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="9fd5f-1043">__NOTA:__ `bot prepare-publish` sigue usando el valor predeterminado anterior.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1043">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="9fd5f-1044">[CAMBIO IMPORTANTE] Se ha cambiado `--lang` para que su valor predeterminado ya no sea `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1044">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="9fd5f-1045">Si el comando requiere `--lang` y no se proporciona, ahora producirá un error.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1045">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="9fd5f-1046">[CAMBIO IMPORTANTE] Se han cambiado los argumentos `--appid` y `--password` de `bot create` para que sean necesarios y ahora se pueden crear mediante `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1046">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="9fd5f-1047">Se ha agregado la validación de `--appid` y `--password`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1047">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="9fd5f-1048">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4` para que no cree ni use una cuenta de almacenamiento ni Application Insights.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1048">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="9fd5f-1049">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v3` para que requiera una región donde esté disponible Application Insights.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1049">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="9fd5f-1050">[CAMBIO IMPORTANTE] Se ha cambiado `bot update` para que ahora afecte solo a determinadas propiedades de un bot.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1050">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="9fd5f-1051">[CAMBIO IMPORTANTE] Se han cambiado las marcas `--lang` para que acepten `Javascript` en lugar de `Node`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1051">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="9fd5f-1052">[CAMBIO IMPORTANTE] Se ha quitado `Node` como valor de `--lang` permitido.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1052">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="9fd5f-1053">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para que no establezca `SCM_DO_BUILD_DURING_DEPLOYMENT` en true.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1053">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="9fd5f-1054">Todas las implementaciones a través de Kudu actuarán según su comportamiento predeterminado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1054">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="9fd5f-1055">Se ha cambiado `bot download` para los bots sin archivos `.bot` para crear el archivo de configuración específico del idioma con los valores de Application Insights para el bot.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1055">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="9fd5f-1056">Se ha agregado compatibilidad de `Typescript` con `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1056">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9fd5f-1057">Se ha agregado un mensaje de advertencia a `bot prepare-deploy` para los bots `Javascript` y `Typescript` cuando `--code-dir` no contiene `package.json`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1057">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="9fd5f-1058">Se ha cambiado `bot prepare-deploy` para que devuelva `true` si es correcto.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1058">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="9fd5f-1059">Se ha agregado el registro detallado a `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1059">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9fd5f-1060">Se han agregado regiones más disponibles de Application Insights a `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1060">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="9fd5f-1061">Configuración</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1061">Configure</span></span>
* <span data-ttu-id="9fd5f-1062">Se ha agregado compatibilidad para configuraciones de valores predeterminados de argumentos basadas en carpetas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1062">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9fd5f-1063">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1063">Eventhubs</span></span>
* <span data-ttu-id="9fd5f-1064">Se agregaron los comandos `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1064">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9fd5f-1065">Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1065">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1066">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1066">Network</span></span>
* <span data-ttu-id="9fd5f-1067">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--cache` con `--defer` para `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1067">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="9fd5f-1068">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1068">Policy Insights</span></span>
* <span data-ttu-id="9fd5f-1069">Se ha agregado compatibilidad a `--expand PolicyEvaluationDetails` para consultar detalles de evaluación de directivas en el recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1069">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1070">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1070">Role</span></span>
* <span data-ttu-id="9fd5f-1071">[EN DESUSO] Se ha cambiado el argumento `create-for-rbac` hide '--password' y se dejará de dar soporte en mayo de 2019.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1071">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fd5f-1072">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1072">Service Bus</span></span>
* <span data-ttu-id="9fd5f-1073">Se agregaron los comandos `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1073">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9fd5f-1074">Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1074">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="9fd5f-1075">Se ha corregido `topic [create|update]` para que `--max-size` permita valores de 10, 20, 40 y 80 GB con SKU Premium.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1075">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-1076">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1076">SQL</span></span>
* <span data-ttu-id="9fd5f-1077">Se agregaron los comandos `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1077">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1078">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1078">VM</span></span>
* <span data-ttu-id="9fd5f-1079">Se ha agregado `--protect-from-scale-in` y `--protect-from-scale-set-actions` a `vmss update` para habilitar las actualizaciones a la directiva de protección de instancias de máquina virtual de VMSS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1079">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="9fd5f-1080">Se ha agregado `--instance-id` a `vmss update` para habilitar la actualización genérica de instancias de máquina virtual de VMSS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1080">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="9fd5f-1081">Se ha agregado `--instance-id` a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1081">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="9fd5f-1082">Se ha agregado un nuevo grupo de comandos `ppg` para administrar grupos de ubicación de proximidad.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1082">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="9fd5f-1083">Se ha agregado `--ppg` a `[vm|vmss] create` y `vm availability-set create` para administrar grupos de ubicación de proximidad.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1083">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="9fd5f-1084">Se ha agregado el parámetro `--hyper-v-generation` a `image create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1084">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="9fd5f-1085">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1085">April 23, 2019</span></span>

<span data-ttu-id="9fd5f-1086">Versión 2.0.63</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1086">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1087">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1087">ACS</span></span>
* <span data-ttu-id="9fd5f-1088">Se ha cambiado `aks get-credentials` para que pregunte si se desean sobrescribir los valores duplicados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1088">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="9fd5f-1089">Se ha quitado `(PREVIEW)` de los comandos de DevSpaces "aks use-dev-spaces" y "aks remove-dev-spaces".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1089">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-1090">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1090">AMS</span></span>
* <span data-ttu-id="9fd5f-1091">Se ha corregido un error con la actualización de los filtros de cuenta y recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1091">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1092">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1092">AppService</span></span>
* <span data-ttu-id="9fd5f-1093">Se ha agregado compatibilidad para ASE y un tiempo de espera a `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1093">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="9fd5f-1094">Se ha agregado compatibilidad para establecer la integración e implementación continuas a una canalización de Azure DevOps desde un repositorio de Github para aplicaciones de función.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1094">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="9fd5f-1095">Se ha agregado el argumento `--github-pat` a `functionapp devops-build create` para aceptar el token de acceso personal de Github.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1095">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="9fd5f-1096">Se ha agregado el argumento `--github-repository` a `functionapp devops-build create` para aceptar el repositorio de Github que contiene un código de origen de aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1096">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="9fd5f-1097">Se ha corregido el problema por el que `az webapp up --logs` producía un error y actualizaba .NETCORE a la versión 2.1 de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1097">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="9fd5f-1098">Se han quitado las opciones de configuración de aplicaciones de función innecesarias a la hora de crear una aplicación de función con un plan de consumo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1098">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="9fd5f-1099">Se ha cambiado `webapp up` para que la cadena asp predeterminada ahora anexe el número al final para crear un nuevo ASP según las opciones de SKU.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1099">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="9fd5f-1100">Se ha agregado `-b` como opción a `webapp up` para iniciar la aplicación en el explorador.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1100">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="9fd5f-1101">Se ha cambiado `webapp deployment source config zip` para controlar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1101">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="9fd5f-1102">Administrador de implementaciones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1102">Deployment Manager</span></span>
* <span data-ttu-id="9fd5f-1103">[VERSIÓN PRELIMINAR] Creación y administración de artefactos que admiten lanzamientos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1103">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="9fd5f-1104">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1104">Lab</span></span>
* <span data-ttu-id="9fd5f-1105">Se ha corregido el error que provocaba una salida prematura.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1105">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1106">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1106">Network</span></span>
* <span data-ttu-id="9fd5f-1107">Se ha agregado la delegación de servidor nombre automática a `dns zone create` en la zona primaria durante la creación de una zona secundaria.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1107">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1108">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1108">Resource</span></span>
* <span data-ttu-id="9fd5f-1109">[EN DESUSO] Se han dejado de usar los argumentos `--link-id`, `--target-id` y `--filter-string` de `resource link`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1109">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="9fd5f-1110">En su lugar, use los argumentos `--link`, `--target` y `--filter`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1110">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="9fd5f-1111">Se ha corregido el problema por el que los comandos `resource link [create|update]` no funcionaban.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1111">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="9fd5f-1112">Se ha corregido un problema por el que se podía producir un problema al eliminar utilizando un identificador de recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1112">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-1113">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1113">SQL</span></span>
* <span data-ttu-id="9fd5f-1114">Se ha agregado compatibilidad para zonas horarias personalizadas en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1114">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="9fd5f-1115">Se ha cambiado para poder usar un nombre de grupo elástico con `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1115">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="9fd5f-1116">Se ha agregado compatibilidad de `--no-wait` con `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1116">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="9fd5f-1117">Se ha agregado el comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1117">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1118">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1118">Storage</span></span>
* <span data-ttu-id="9fd5f-1119">Se ha corregido un problema con los tokens de SAS de codificación doble en `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1119">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1120">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1120">VM</span></span>
* <span data-ttu-id="9fd5f-1121">Se ha agregado la marca `--skip-shutdown` a `vm|vmss stop` para apagar las máquinas virtuales sin cerrarlas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1121">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="9fd5f-1122">Se ha agregado el argumento `--storage-account-type` a `sig image-version create` para establecer el tipo de cuenta del perfil de publicación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1122">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="9fd5f-1123">Se ha agregado el argumento `--target-regions` a `sig image-version create` para permitir tipos de cuenta de almacenamiento específicos de la región.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1123">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="9fd5f-1124">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1124">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1125">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1125">Core</span></span>
* <span data-ttu-id="9fd5f-1126">Se ha corregido el problema por el que algunas extensiones mostraban una versión `Unknown` y no se podían actualizar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1126">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1127">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1127">ACR</span></span>
* <span data-ttu-id="9fd5f-1128">Se ha agregado compatibilidad con la ejecución de una imagen sin contexto.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1128">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-1129">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1129">AMS</span></span>
* [EN DESUSO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CAMBIO IMPORTANTE]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="9fd5f-1132">Se ha agregado compatibilidad con nuevos parámetros de cifrado a `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1132">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="9fd5f-1133">Se ha agregado un nuevo parámetro `--filters` a `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1133">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1134">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1134">AppService</span></span>
* <span data-ttu-id="9fd5f-1135">Se ha agregado compatibilidad de `--logs` con `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1135">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="9fd5f-1136">En el comando `functionapp devops-build create`, se han corregido los problemas de generación de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1136">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="9fd5f-1137">Se ha mejorado el control de errores y los indicadores de `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1137">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="9fd5f-1138">[CAMBIO IMPORTANTE] Se ha quitado la marca `--local-git` del comando `devops-build`; la detección y administración del repositorio git local son obligatorias para crear canalizaciones de Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1138">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="9fd5f-1139">Se ha agregado compatibilidad para crear planes de funciones Linux</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1139">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="9fd5f-1140">Se ha agregado la posibilidad de cambiar el plan de una aplicación de función mediante `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1140">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="9fd5f-1141">Se ha agregado compatibilidad para las opciones de escalado horizontal del plan Premium de Azure Functions</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1141">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-1142">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1142">CDN</span></span>
* <span data-ttu-id="9fd5f-1143">Se ha agregado compatibilidad para `Microsoft_Standard` y `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1143">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="9fd5f-1144">Comentarios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1144">Feedback</span></span>
* <span data-ttu-id="9fd5f-1145">Se ha cambiado `feedback` para mostrar los metadatos de los comandos ejecutados recientemente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1145">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="9fd5f-1146">Se ha cambiado `feedback` para pedir al usuario que abra un explorador y use una plantilla de incidencia para ayudar en el proceso de creación de la incidencia</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1146">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="9fd5f-1147">Se ha cambiado `feedback` para imprimir el cuerpo de la incidencia cuando se ejecuta con "--verbose"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1147">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-1148">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1148">Monitor</span></span>
* <span data-ttu-id="9fd5f-1149">Se ha corregido un problema por "count" no era un valor permitido en `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1149">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="9fd5f-1150">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1150">Network</span></span>
* <span data-ttu-id="9fd5f-1151">Se ha corregido el formato de tabla que no se mostraba con `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1151">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="9fd5f-1152">Se han agregado los comandos `list-request-headers` y `list-response-headers` a `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1152">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="9fd5f-1153">Se ha agregado el comando `list-server-variables` a `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1153">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="9fd5f-1154">Se ha corregido un problema por el que actualización del estado de un vínculo en un puerto de express-route generaba una excepción de atributo desconocido `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1154">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="9fd5f-1155">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1155">PrivateDNS</span></span>
* <span data-ttu-id="9fd5f-1156">Se ha agregado `network private-dns` para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1156">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1157">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1157">Resource</span></span>
* <span data-ttu-id="9fd5f-1158">Se ha corregido el problema con `deployment create` y `group deployment create` por el que no funcionaba un archivo de parámetros con un conjunto de parámetros vacío</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1158">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1159">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1159">Role</span></span>
* <span data-ttu-id="9fd5f-1160">Se ha corregido `create-for-rbac` para que trate `--years` correctamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1160">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="9fd5f-1161">[CAMBIO IMPORTANTE] Se ha cambiado `role assignment delete` para preguntar cuando se eliminan todas las asignaciones de la suscripción de forma incondicional</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1161">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-1162">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1162">SQL</span></span>
* <span data-ttu-id="9fd5f-1163">Se ha actualizado `sql mi [create|update]` con las propiedades proxyOverride y publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1163">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1164">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1164">Storage</span></span>
* <span data-ttu-id="9fd5f-1165">[CAMBIO IMPORTANTE] Se ha quitado el resultado de `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1165">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="9fd5f-1166">Se ha agregado `--full-uri` a `storage blob generate-sas` para crear el URI completo para el blob con SAS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1166">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="9fd5f-1167">Se ha agregado `--file-snapshot` a `storage file copy start` para copiar el archivo desde la instantánea</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1167">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="9fd5f-1168">Se ha cambiado `storage blob copy cancel` para mostrar solo el error en lugar de la excepción para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1168">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="9fd5f-1169">26 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1169">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="9fd5f-1170">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1170">Core</span></span>
* <span data-ttu-id="9fd5f-1171">Se han corregido problemas con la incompatibilidad de la extensión de desarrollo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1171">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="9fd5f-1172">El control de errores ahora dirige a los clientes a la página de problemas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1172">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="9fd5f-1173">Nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1173">Cloud</span></span>
* <span data-ttu-id="9fd5f-1174">Se ha corregido un error de "suscripción no encontrada" en `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1174">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1175">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1175">ACR</span></span>
* <span data-ttu-id="9fd5f-1176">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1176">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="9fd5f-1177">Se ha agregado `--auth-mode` a los comandos `acr build`, `acr run`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1177">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="9fd5f-1178">Se ha agregado el grupo de comandos "acr task credential" para administrar las credenciales de una tarea.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1178">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="9fd5f-1179">Se ha agregado "--no-wait" al comando `acr build`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1179">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1180">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1180">AppService</span></span>
* <span data-ttu-id="9fd5f-1181">Se ha corregido el error por el que `webapp up` no controlaba correctamente los escenarios de ejecución desde un directorio o de código desconocido.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1181">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="9fd5f-1182">Se ha corregido el error por el que los espacios no funcionaban para `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1182">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="9fd5f-1183">Servicio BOT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1183">BOT Service</span></span>
* <span data-ttu-id="9fd5f-1184">Se ha agregado `bot prepare-deploy` para preparar la implementación de bots mediante `webapp`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1184">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="9fd5f-1185">Se ha cambiado `bot create --kind registration` para que muestre la contraseña si no se proporciona una.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1185">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="9fd5f-1186">[CAMBIO IMPORTANTE] Se ha cambiado `--endpoint` en `bot create --kind registration` a que sea una cadena vacía de forma predeterminada en lugar de que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1186">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="9fd5f-1187">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1187">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-1188">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1188">CDN</span></span>
* <span data-ttu-id="9fd5f-1189">Se agregó compatibilidad para `--no-wait` a `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1189">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="9fd5f-1190">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento de almacenamiento de cadenas de consulta en caché predeterminado de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1190">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="9fd5f-1191">El valor predeterminado ya no es "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1191">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9fd5f-1192">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1192">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-1193">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1193">Cosmosdb</span></span>
* <span data-ttu-id="9fd5f-1194">Se ha agregado compatibilidad con `--enable-multiple-write-locations` al actualizar la cuenta.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1194">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="9fd5f-1195">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1195">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-1196">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1196">Interactive</span></span>
* <span data-ttu-id="9fd5f-1197">Se ha corregido la incompatibilidad con la extensión interactiva instalada mediante azdev.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1197">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-1198">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1198">Monitor</span></span>
* <span data-ttu-id="9fd5f-1199">Se ha cambiado para permitir el valor de dimensión `*` para `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1199">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1200">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1200">Network</span></span>
* <span data-ttu-id="9fd5f-1201">Se ha agregado el grupo de comandos `rewrite-rule` a `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1201">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-1202">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1202">Profile</span></span>
* <span data-ttu-id="9fd5f-1203">Se ha agregado a `login` compatibilidad de la cuenta en el nivel de inquilino para la identidad de servicio administrada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1203">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="9fd5f-1204">Postgres</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1204">Postgres</span></span> 
* <span data-ttu-id="9fd5f-1205">Se han agregado los comandos postgresql `replica` y el comando `restart server`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1205">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="9fd5f-1206">Se ha cambiado para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1206">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1207">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1207">Resource</span></span>
* <span data-ttu-id="9fd5f-1208">Se ha mejorado la salida de tabla de `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1208">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="9fd5f-1209">Se ha corregido el problema con `deployment [create|validate]` por el que no reconocía el tipo secureObject.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1209">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="9fd5f-1210">Grafo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1210">Graph</span></span>
* <span data-ttu-id="9fd5f-1211">Se agregó compatibilidad para `--end-date` a `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1211">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="9fd5f-1212">Se ha agregado compatibilidad para agregar permisos con `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1212">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="9fd5f-1213">Se ha corregido un error con `ad app permission list` cuando no había ningún permiso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1213">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="9fd5f-1214">Se ha cambiado `ad sp delete` para omitir la eliminación de la asignación de roles si la cuenta actual no tiene ninguna suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1214">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="9fd5f-1215">Se ha cambiado `ad app create` para que `--identifier-uris` sea una lista vacía de forma predeterminada si no se proporciona.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1215">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1216">storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1216">storage</span></span>
* <span data-ttu-id="9fd5f-1217">Se ha agregado `--snapshot` a `storage file download-batch` para descargar desde una instantánea de recurso compartido.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1217">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="9fd5f-1218">Se ha cambiado la barra de progreso `storage blob [download-batch|upload-batch]` para que sea menos detallada y que indique el blob actual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1218">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="9fd5f-1219">Se ha corregido el problema con `storage account update` al actualizar los parámetros de cifrado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1219">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="9fd5f-1220">Se ha corregido el problema por el que `storage blob show` producía un error al usar oauth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1220">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1221">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1221">VM</span></span>
* <span data-ttu-id="9fd5f-1222">Se agregó el comando `image update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1222">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="9fd5f-1223">12 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1223">March 12, 2019</span></span>

<span data-ttu-id="9fd5f-1224">Versión 2.0.60</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1224">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1225">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1225">Core</span></span>

* <span data-ttu-id="9fd5f-1226">Se ha corregido un error incorrecto en `cloud set` sobre la suscripción no encontrada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1226">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1227">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1227">ACR</span></span>

* <span data-ttu-id="9fd5f-1228">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1228">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1229">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1229">ACS</span></span>

* <span data-ttu-id="9fd5f-1230">Ahora, se omite el parámetro `--listen-address` de `aks browse` si kubectl no lo admite</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1230">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="9fd5f-1231">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1231">AppService</span></span>

* <span data-ttu-id="9fd5f-1232">Se ha agregado `[webapp|functionapp] deployment list-publishing-credentials` para obtener la dirección URL y sus credenciales de publicación de Kudu.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1232">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="9fd5f-1233">Se ha quitado la instrucción de impresión errónea para `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1233">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="9fd5f-1234">Se ha corregido `functionapp` para establecer la imagen correcta en el entorno de ejecución en los planes de App Service de Linux</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1234">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="9fd5f-1235">Se ha quitado la etiqueta de versión preliminar para `webapp up` y se han agregado mejoras al comando.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1235">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-1236">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1236">Botservice</span></span>

* <span data-ttu-id="9fd5f-1237">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1237">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9fd5f-1238">Se han agregado `Microsoft-BotFramework-AppId` y `Microsoft-BotFramework-AppPassword` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1238">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9fd5f-1239">Se han quitado las comillas simples de la salida del comando `bot publish` al final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1239">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="9fd5f-1240">Se ha cambiado `bot publish` para que sea asincrónico.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1240">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1241">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1241">Container</span></span>

* <span data-ttu-id="9fd5f-1242">Se agregó el argumento `--no-wait` a `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1242">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="9fd5f-1243">EventHub</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1243">EventHub</span></span>

* <span data-ttu-id="9fd5f-1244">Se ha agregado la marca `--skip-empty-archives` a `eventhub create|update` para admitir archivos vacíos en la captura.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1244">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="9fd5f-1245">Buscar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1245">Find</span></span>

* <span data-ttu-id="9fd5f-1246">Actualización de la funcionalidad principal</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1246">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-1247">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1247">HDInsight</span></span>

* <span data-ttu-id="9fd5f-1248">Se ha agregado el parámetro `--storage-account-managed-identity` a `hdinsight create` para admitir MSI de ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1248">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1249">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1249">Network</span></span>

* <span data-ttu-id="9fd5f-1250">Se ha corregido un problema con `vpn-connection update` por el que no se podía actualizar una conexión VPN entre pasarelas de diferentes suscripciones.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1250">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-1251">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1251">Rdbms</span></span>

* <span data-ttu-id="9fd5f-1252">Correcciones menores para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1252">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1253">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1253">Role</span></span>

* <span data-ttu-id="9fd5f-1254">Se ha corregido `role definition update` para usar el identificador para resolver la definición correctamente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1254">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="9fd5f-1255">Se ha cambiado `ad app credential reset` para eliminar la suposición de que la entidad de servicio de la aplicación siempre existe.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1255">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fd5f-1256">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1256">Service Fabric</span></span>

* <span data-ttu-id="9fd5f-1257">Se ha corregido un problema con `sf cluster list` que no se podía iterar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1257">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="9fd5f-1258">26 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1258">February 26, 2019</span></span>

<span data-ttu-id="9fd5f-1259">Versión 2.0.59</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1259">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1260">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1260">Core</span></span>

* <span data-ttu-id="9fd5f-1261">Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1261">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1262">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1262">ACR</span></span>

* <span data-ttu-id="9fd5f-1263">Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1263">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="9fd5f-1264">Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1264">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1265">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1265">ACS</span></span>

* <span data-ttu-id="9fd5f-1266">Se agregó la opción `--listen-address` a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1266">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1267">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1267">AppService</span></span>

* <span data-ttu-id="9fd5f-1268">Se agregó el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1268">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-1269">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1269">Batch</span></span>
* <span data-ttu-id="9fd5f-1270">[CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1270">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="9fd5f-1271">[CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1271">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="9fd5f-1272">Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1272">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="9fd5f-1273">[CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1273">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="9fd5f-1274">Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1274">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="9fd5f-1275">Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1275">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-1276">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1276">CosmosDB</span></span>

* <span data-ttu-id="9fd5f-1277">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1277">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="9fd5f-1278">Kusto</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1278">Kusto</span></span>

* <span data-ttu-id="9fd5f-1279">[CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1279">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1280">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1280">Network</span></span>

* <span data-ttu-id="9fd5f-1281">Se agregó el argumento `--express-route-gateway-bypass` a `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1281">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="9fd5f-1282">Se han agregado grupos de comandos desde extensiones `express-route`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1282">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="9fd5f-1283">Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1283">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="9fd5f-1284">Se agregó el argumento `--legacy-mode` a `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1284">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="9fd5f-1285">Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1285">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="9fd5f-1286">Se agregó el argumento `--gateway-default-site` a `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1286">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="9fd5f-1287">Se han agregado comandos `ipsec-policy` a `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1287">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1288">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1288">Resource</span></span>

* <span data-ttu-id="9fd5f-1289">Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1289">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="9fd5f-1290">Se ha agregado compatibilidad para el archivo de parámetros basado en URI a `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1290">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="9fd5f-1291">Se ha agregado compatibilidad para definiciones y parámetros basados en URI para `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1291">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="9fd5f-1292">Se ha corregido el control de parámetros y reglas para `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1292">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="9fd5f-1293">Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1293">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1294">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1294">Role</span></span>

* <span data-ttu-id="9fd5f-1295">Se ha agregado compatibilidad con roles de aplicación a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1295">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1296">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1296">VM</span></span>

* <span data-ttu-id="9fd5f-1297">Se ha corregido un problema con `vm create where `--acelerated-networking\` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1297">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="9fd5f-1298">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1298">February 12, 2019</span></span>

<span data-ttu-id="9fd5f-1299">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1299">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1300">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1300">Core</span></span>

* <span data-ttu-id="9fd5f-1301">`az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1301">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="9fd5f-1302">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1302">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1303">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1303">ACR</span></span>
* <span data-ttu-id="9fd5f-1304">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1304">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="9fd5f-1305">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1305">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1306">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1306">ACS</span></span>
* <span data-ttu-id="9fd5f-1307">Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1307">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="9fd5f-1308">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1308">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="9fd5f-1309">Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1309">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-1310">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1310">AMS</span></span>
* <span data-ttu-id="9fd5f-1311">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1311">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="9fd5f-1312">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1312">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1313">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1313">Appservice</span></span>
* <span data-ttu-id="9fd5f-1314">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1314">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="9fd5f-1315">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1315">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="9fd5f-1316">Se ha mejorado la ayuda de `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1316">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="9fd5f-1317">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1317">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="9fd5f-1318">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1318">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-1319">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1319">Botservice</span></span>
* <span data-ttu-id="9fd5f-1320">Se ha mejorado la experiencia de usuario de `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1320">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="9fd5f-1321">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1321">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="9fd5f-1322">Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1322">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="9fd5f-1323">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1323">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="9fd5f-1324">[EN DESUSO] Se ha dejado de utilizar el argumento `--proj-name` en favor de `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1324">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="9fd5f-1325">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1325">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="9fd5f-1326">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1326">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="9fd5f-1327">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1327">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="9fd5f-1328">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1328">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="9fd5f-1329">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1329">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-1330">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1330">Key Vault</span></span>
* <span data-ttu-id="9fd5f-1331">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1331">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-1332">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1332">Monitor</span></span>
* <span data-ttu-id="9fd5f-1333">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1333">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1334">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1334">Network</span></span>
* <span data-ttu-id="9fd5f-1335">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1335">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="9fd5f-1336">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1336">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="9fd5f-1337">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1337">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="9fd5f-1338">Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1338">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9fd5f-1339">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1339">Policy Insights</span></span>
* <span data-ttu-id="9fd5f-1340">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1340">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-1341">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1341">RDBMS</span></span>
* <span data-ttu-id="9fd5f-1342">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1342">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="9fd5f-1343">Redis</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1343">Redis</span></span>
* <span data-ttu-id="9fd5f-1344">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1344">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="9fd5f-1345">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1345">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="9fd5f-1346">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1346">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="9fd5f-1347">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1347">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="9fd5f-1348">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1348">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="9fd5f-1349">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1349">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="9fd5f-1350">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1350">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1351">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1351">Role</span></span>
* <span data-ttu-id="9fd5f-1352">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1352">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="9fd5f-1353">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1353">SQL VM</span></span>
* <span data-ttu-id="9fd5f-1354">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1354">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1355">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1355">VM</span></span>
* <span data-ttu-id="9fd5f-1356">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1356">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="9fd5f-1357">Se agregó `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1357">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="9fd5f-1358">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1358">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="9fd5f-1359">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1359">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="9fd5f-1360">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1360">January 31, 2019</span></span>

<span data-ttu-id="9fd5f-1361">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1361">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1362">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1362">Core</span></span>

* <span data-ttu-id="9fd5f-1363">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1363">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="9fd5f-1364">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1364">January 28, 2019</span></span>

<span data-ttu-id="9fd5f-1365">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1365">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1366">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1366">ACR</span></span>
* <span data-ttu-id="9fd5f-1367">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1367">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1368">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1368">ACS</span></span>
* <span data-ttu-id="9fd5f-1369">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1369">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9fd5f-1370">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1370">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="9fd5f-1371">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1371">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-1372">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1372">AMS</span></span>
* <span data-ttu-id="9fd5f-1373">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1373">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="9fd5f-1374">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1374">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1375">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1375">Appservice</span></span>
* <span data-ttu-id="9fd5f-1376">Se ha agregado compatibilidad para App Insights en `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1376">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="9fd5f-1377">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1377">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="9fd5f-1378">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1378">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1379">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1379">Container</span></span>
* <span data-ttu-id="9fd5f-1380">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1380">Added `container start` command</span></span>
* <span data-ttu-id="9fd5f-1381">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1381">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9fd5f-1382">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1382">EventGrid</span></span>
* <span data-ttu-id="9fd5f-1383">Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1383">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="9fd5f-1384">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1384">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="9fd5f-1385">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1385">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="9fd5f-1386">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1386">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="9fd5f-1387">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1387">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-1388">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1388">HDInsight</span></span>
* <span data-ttu-id="9fd5f-1389">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1389">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="9fd5f-1390">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1390">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="9fd5f-1391">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1391">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="9fd5f-1392">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1392">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="9fd5f-1393">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1393">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="9fd5f-1394">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1394">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-1395">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1395">IoT</span></span>
* <span data-ttu-id="9fd5f-1396">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1396">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="9fd5f-1397">Kusto</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1397">Kusto</span></span>
* <span data-ttu-id="9fd5f-1398">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1398">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-1399">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1399">Monitor</span></span>
* <span data-ttu-id="9fd5f-1400">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1400">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-1401">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1401">Profile</span></span>
* <span data-ttu-id="9fd5f-1402">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1402">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1403">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1403">Network</span></span>
* <span data-ttu-id="9fd5f-1404">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1404">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="9fd5f-1405">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1405">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1406">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1406">Resource</span></span>
* <span data-ttu-id="9fd5f-1407">Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1407">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="9fd5f-1408">Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1408">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="9fd5f-1409">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1409">SQL Virtual Machine</span></span>
* <span data-ttu-id="9fd5f-1410">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1410">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1411">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1411">Storage</span></span>
* <span data-ttu-id="9fd5f-1412">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1412">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="9fd5f-1413">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1413">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1414">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1414">VM</span></span>
* <span data-ttu-id="9fd5f-1415">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1415">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="9fd5f-1416">Se ha agregado la marca `--force` a `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1416">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="9fd5f-1417">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1417">January 15, 2019</span></span>

<span data-ttu-id="9fd5f-1418">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1418">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1419">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1419">ACR</span></span>
* <span data-ttu-id="9fd5f-1420">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1420">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="9fd5f-1421">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1421">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="9fd5f-1422">[EN DESUSO] Se ha dejado de usar el parámetro `--resource-group` en los comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1422">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="9fd5f-1423">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1423">ACS</span></span>
* <span data-ttu-id="9fd5f-1424">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1424">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1425">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1425">Appservice</span></span>
* <span data-ttu-id="9fd5f-1426">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1426">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="9fd5f-1427">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1427">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="9fd5f-1428">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1428">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="9fd5f-1429">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1429">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-1430">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1430">Botservice</span></span>
* <span data-ttu-id="9fd5f-1431">Se han agregado actualizaciones al estado de implementación a `bot create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1431">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="9fd5f-1432">Configuración</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1432">Configure</span></span>
* <span data-ttu-id="9fd5f-1433">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1433">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-1434">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1434">CosmosDB</span></span>
* <span data-ttu-id="9fd5f-1435">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1435">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-1436">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1436">HDInsight</span></span>
* <span data-ttu-id="9fd5f-1437">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1437">Added commands for managing applications</span></span>
* <span data-ttu-id="9fd5f-1438">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1438">Added commands for managing script actions</span></span>
* <span data-ttu-id="9fd5f-1439">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1439">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="9fd5f-1440">Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1440">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="9fd5f-1441">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1441">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1442">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1442">Network</span></span>
* <span data-ttu-id="9fd5f-1443">Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1443">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="9fd5f-1444">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1444">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="9fd5f-1445">Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1445">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="9fd5f-1446">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1446">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1447">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1447">Role</span></span>
* <span data-ttu-id="9fd5f-1448">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1448">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="9fd5f-1449">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1449">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="9fd5f-1450">Seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1450">Security</span></span>
* <span data-ttu-id="9fd5f-1451">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1451">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1452">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1452">Storage</span></span>
* <span data-ttu-id="9fd5f-1453">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1453">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="9fd5f-1454">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1454">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="9fd5f-1455">Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1455">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="9fd5f-1456">Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1456">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="9fd5f-1457">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1457">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1458">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1458">VM</span></span>
* <span data-ttu-id="9fd5f-1459">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1459">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="9fd5f-1460">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1460">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fd5f-1461">Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1461">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="9fd5f-1462">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1462">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="9fd5f-1463">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1463">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="9fd5f-1464">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1464">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="9fd5f-1465">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1465">December 20, 2018</span></span>

<span data-ttu-id="9fd5f-1466">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1466">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="9fd5f-1467">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1467">Appservice</span></span>
* <span data-ttu-id="9fd5f-1468">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1468">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="9fd5f-1469">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1469">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="9fd5f-1470">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1470">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9fd5f-1471">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1471">IoTCentral</span></span>
* <span data-ttu-id="9fd5f-1472">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1472">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1473">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1473">Role</span></span>
* <span data-ttu-id="9fd5f-1474">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1474">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-1475">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1475">SQL</span></span>
* <span data-ttu-id="9fd5f-1476">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1476">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1477">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1477">VM</span></span>
* <span data-ttu-id="9fd5f-1478">Se ha agregado el parámetro `---os-type` a `disk create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1478">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="9fd5f-1479">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1479">December 18, 2018</span></span>

<span data-ttu-id="9fd5f-1480">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1480">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="9fd5f-1481">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1481">ACR</span></span>
* <span data-ttu-id="9fd5f-1482">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1482">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="9fd5f-1483">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1483">Condensed the table layout for task list</span></span>
* <span data-ttu-id="9fd5f-1484">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1484">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1485">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1485">ACS</span></span>
* <span data-ttu-id="9fd5f-1486">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1486">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9fd5f-1487">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1487">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="9fd5f-1488">[EN DESUSO] Se han dejado de usar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1488">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="9fd5f-1489">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1489">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="9fd5f-1490">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1490">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="9fd5f-1491">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1491">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1492">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1492">Appservice</span></span>
* <span data-ttu-id="9fd5f-1493">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1493">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="9fd5f-1494">Botservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1494">Botservice</span></span>
* <span data-ttu-id="9fd5f-1495">Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1495">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="9fd5f-1496">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1496">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="9fd5f-1497">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1497">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="9fd5f-1498">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1498">Reduced Kudu network calls</span></span>
* <span data-ttu-id="9fd5f-1499">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1499">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="9fd5f-1500">Consumo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1500">Consumption</span></span>
* <span data-ttu-id="9fd5f-1501">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1501">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-1502">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1502">CosmosDB</span></span>
* <span data-ttu-id="9fd5f-1503">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1503">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="9fd5f-1504">Mapas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1504">Maps</span></span>
* <span data-ttu-id="9fd5f-1505">Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1505">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1506">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1506">Network</span></span>
* <span data-ttu-id="9fd5f-1507">Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1507">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="9fd5f-1508">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1508">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1509">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1509">Resource</span></span>
* <span data-ttu-id="9fd5f-1510">Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1510">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="9fd5f-1511">Se ha agregado un nuevo comando `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1511">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1512">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1512">Storage</span></span>
*  <span data-ttu-id="9fd5f-1513">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1513">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1514">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1514">VM</span></span>
* <span data-ttu-id="9fd5f-1515">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1515">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="9fd5f-1516">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1516">December 4, 2018</span></span>

<span data-ttu-id="9fd5f-1517">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1517">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="9fd5f-1518">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1518">Core</span></span>
* <span data-ttu-id="9fd5f-1519">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1519">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="9fd5f-1520">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1520">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1521">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1521">Appservice</span></span>
* <span data-ttu-id="9fd5f-1522">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1522">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="9fd5f-1523">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1523">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1524">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1524">Network</span></span>
* <span data-ttu-id="9fd5f-1525">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1525">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1526">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1526">Role</span></span>
* <span data-ttu-id="9fd5f-1527">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1527">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="9fd5f-1528">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1528">VM</span></span>
* <span data-ttu-id="9fd5f-1529">[EN DESUSO] Se ha dejado de usar el parámetro `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1529">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="9fd5f-1530">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1530">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="9fd5f-1531">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1531">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="9fd5f-1532">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1532">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="9fd5f-1533">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1533">November 20, 2018</span></span>

<span data-ttu-id="9fd5f-1534">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1534">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="9fd5f-1535">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1535">Core</span></span>
* <span data-ttu-id="9fd5f-1536">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1536">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1537">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1537">ACR</span></span>
* <span data-ttu-id="9fd5f-1538">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1538">Added context token to task step</span></span>
* <span data-ttu-id="9fd5f-1539">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1539">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="9fd5f-1540">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1540">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1541">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1541">Appservice</span></span>
* <span data-ttu-id="9fd5f-1542">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1542">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="9fd5f-1543">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1543">Updated the default `node_version`.</span></span> <span data-ttu-id="9fd5f-1544">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1544">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="9fd5f-1545">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1545">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="9fd5f-1546">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1546">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9fd5f-1547">IotCentral</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1547">IotCentral</span></span>
* <span data-ttu-id="9fd5f-1548">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1548">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-1549">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1549">KeyVault</span></span>
* <span data-ttu-id="9fd5f-1550">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1550">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1551">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1551">Network</span></span>
* <span data-ttu-id="9fd5f-1552">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1552">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="9fd5f-1553">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1553">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="9fd5f-1554">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1554">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="9fd5f-1555">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1555">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-1556">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1556">Rdbms</span></span>
* <span data-ttu-id="9fd5f-1557">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1557">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="9fd5f-1558">Rbac</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1558">Rbac</span></span>
* <span data-ttu-id="9fd5f-1559">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1559">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="9fd5f-1560">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1560">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="9fd5f-1561">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1561">Storage</span></span>
* <span data-ttu-id="9fd5f-1562">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1562">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="9fd5f-1563">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1563">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="9fd5f-1564">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1564">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="9fd5f-1565">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1565">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1566">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1566">VM</span></span>
* <span data-ttu-id="9fd5f-1567">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1567">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="9fd5f-1568">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1568">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="9fd5f-1569">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1569">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="9fd5f-1570">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1570">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="9fd5f-1571">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1571">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="9fd5f-1572">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1572">Added `snapshot wait` command</span></span>
* <span data-ttu-id="9fd5f-1573">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1573">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="9fd5f-1574">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1574">November 6, 2018</span></span>

<span data-ttu-id="9fd5f-1575">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1575">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1576">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1576">Core</span></span>
* <span data-ttu-id="9fd5f-1577">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1577">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1578">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1578">ACR</span></span>
* <span data-ttu-id="9fd5f-1579">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1579">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="9fd5f-1580">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1580">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1581">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1581">ACS</span></span>
* <span data-ttu-id="9fd5f-1582">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1582">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="9fd5f-1583">Advisor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1583">Advisor</span></span>
* <span data-ttu-id="9fd5f-1584">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1584">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-1585">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1585">AMS</span></span>
* <span data-ttu-id="9fd5f-1586">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1586">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="9fd5f-1587">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1587">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="9fd5f-1588">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1588">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="9fd5f-1589">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1589">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="9fd5f-1590">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1590">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="9fd5f-1591">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1591">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="9fd5f-1592">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1592">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="9fd5f-1593">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1593">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="9fd5f-1594">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1594">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="9fd5f-1595">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1595">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="9fd5f-1596">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1596">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="9fd5f-1597">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1597">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="9fd5f-1598">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1598">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="9fd5f-1599">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1599">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="9fd5f-1600">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1600">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="9fd5f-1601">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1601">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="9fd5f-1602">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1602">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1603">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1603">AppService</span></span>
* <span data-ttu-id="9fd5f-1604">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1604">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="9fd5f-1605">Configuración</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1605">Configure</span></span>
* <span data-ttu-id="9fd5f-1606">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1606">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1607">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1607">Container</span></span>
* <span data-ttu-id="9fd5f-1608">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1608">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="9fd5f-1609">EventHub</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1609">EventHub</span></span>
* <span data-ttu-id="9fd5f-1610">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1610">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-1611">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1611">Interactive</span></span>
* <span data-ttu-id="9fd5f-1612">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1612">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-1613">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1613">Monitor</span></span>
* <span data-ttu-id="9fd5f-1614">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1614">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1615">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1615">Network</span></span>
* <span data-ttu-id="9fd5f-1616">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1616">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="9fd5f-1617">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1617">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="9fd5f-1618">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1618">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="9fd5f-1619">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1619">Profile</span></span>
* <span data-ttu-id="9fd5f-1620">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1620">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-1621">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1621">RDBMS</span></span>
* <span data-ttu-id="9fd5f-1622">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1622">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1623">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1623">Resource</span></span>
* <span data-ttu-id="9fd5f-1624">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1624">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1625">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1625">Role</span></span>
* <span data-ttu-id="9fd5f-1626">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1626">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="9fd5f-1627">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1627">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="9fd5f-1628">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1628">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1629">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1629">Storage</span></span>
* <span data-ttu-id="9fd5f-1630">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1630">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1631">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1631">VM</span></span>
* <span data-ttu-id="9fd5f-1632">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1632">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="9fd5f-1633">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1633">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="9fd5f-1634">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1634">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="9fd5f-1635">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1635">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="9fd5f-1636">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1636">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="9fd5f-1637">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1637">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="9fd5f-1638">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1638">October 23, 2018</span></span>

<span data-ttu-id="9fd5f-1639">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1639">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1640">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1640">Core</span></span>
* <span data-ttu-id="9fd5f-1641">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1641">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="9fd5f-1642">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1642">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1643">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1643">ACR</span></span>
* <span data-ttu-id="9fd5f-1644">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1644">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-1645">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1645">CDN</span></span>
* <span data-ttu-id="9fd5f-1646">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1646">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9fd5f-1647">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1647">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1648">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1648">Container</span></span>
* <span data-ttu-id="9fd5f-1649">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1649">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="9fd5f-1650">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1650">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="9fd5f-1651">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1651">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="9fd5f-1652">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1652">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="9fd5f-1653">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1653">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="9fd5f-1654">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1654">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="9fd5f-1655">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1655">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-1656">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1656">CosmosDB</span></span>
* <span data-ttu-id="9fd5f-1657">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1657">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-1658">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1658">Interactive</span></span>
* <span data-ttu-id="9fd5f-1659">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1659">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="9fd5f-1660">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1660">IoT Central</span></span>
* <span data-ttu-id="9fd5f-1661">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1661">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="9fd5f-1662">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1662">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-1663">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1663">Monitor</span></span>
* <span data-ttu-id="9fd5f-1664">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1664">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="9fd5f-1665">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1665">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="9fd5f-1666">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1666">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9fd5f-1667">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1667">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="9fd5f-1668">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1668">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="9fd5f-1669">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1669">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="9fd5f-1670">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1670">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="9fd5f-1671">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1671">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9fd5f-1672">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1672">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="9fd5f-1673">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1673">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1674">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1674">Network</span></span>
* <span data-ttu-id="9fd5f-1675">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1675">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="9fd5f-1676">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1676">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="9fd5f-1677">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1677">ServiceBus</span></span>
* <span data-ttu-id="9fd5f-1678">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1678">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-1679">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1679">SQL</span></span>
* <span data-ttu-id="9fd5f-1680">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1680">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1681">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1681">Storage</span></span>
* <span data-ttu-id="9fd5f-1682">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1682">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="9fd5f-1683">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1683">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1684">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1684">VM</span></span>
* <span data-ttu-id="9fd5f-1685">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1685">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fd5f-1686">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1686">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="9fd5f-1687">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1687">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="9fd5f-1688">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1688">October 16, 2018</span></span>

<span data-ttu-id="9fd5f-1689">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1689">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1690">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1690">VM</span></span>
* <span data-ttu-id="9fd5f-1691">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1691">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="9fd5f-1692">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1692">October 9, 2018</span></span>

<span data-ttu-id="9fd5f-1693">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1693">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1694">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1694">Core</span></span>
* <span data-ttu-id="9fd5f-1695">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1695">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1696">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1696">ACR</span></span>
* <span data-ttu-id="9fd5f-1697">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1697">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1698">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1698">ACS</span></span>
* <span data-ttu-id="9fd5f-1699">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1699">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="9fd5f-1700">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1700">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="9fd5f-1701">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1701">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="9fd5f-1702">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1702">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1703">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1703">Container</span></span>
* <span data-ttu-id="9fd5f-1704">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1704">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="9fd5f-1705">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1705">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="9fd5f-1706">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1706">Event Hub</span></span>
* <span data-ttu-id="9fd5f-1707">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1707">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="9fd5f-1708">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1708">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="9fd5f-1709">Extensiones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1709">Extensions</span></span>
* <span data-ttu-id="9fd5f-1710">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1710">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9fd5f-1711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1711">HDInsight</span></span>
* <span data-ttu-id="9fd5f-1712">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1712">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-1713">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1713">IoT</span></span>
* <span data-ttu-id="9fd5f-1714">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1714">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-1715">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1715">KeyVault</span></span>
* <span data-ttu-id="9fd5f-1716">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1716">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1717">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1717">Network</span></span>
* <span data-ttu-id="9fd5f-1718">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1718">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="9fd5f-1719">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1719">See #6052</span></span>
* <span data-ttu-id="9fd5f-1720">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1720">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="9fd5f-1721">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1721">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="9fd5f-1722">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1722">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="9fd5f-1723">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1723">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="9fd5f-1724">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1724">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="9fd5f-1725">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1725">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1726">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1726">Role</span></span>
* <span data-ttu-id="9fd5f-1727">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1727">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="9fd5f-1728">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1728">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="9fd5f-1729">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1729">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="9fd5f-1730">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1730">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fd5f-1731">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1731">Service Bus</span></span>
* <span data-ttu-id="9fd5f-1732">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1732">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1733">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1733">VM</span></span>
* <span data-ttu-id="9fd5f-1734">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1734">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="9fd5f-1735">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1735">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="9fd5f-1736">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1736">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="9fd5f-1737">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1737">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="9fd5f-1738">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1738">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="9fd5f-1739">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1739">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="9fd5f-1740">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1740">September 21, 2018</span></span>

<span data-ttu-id="9fd5f-1741">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1741">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1742">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1742">ACR</span></span>
* <span data-ttu-id="9fd5f-1743">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1743">Added ACR Task commands</span></span>
* <span data-ttu-id="9fd5f-1744">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1744">Added quick run command</span></span>
* <span data-ttu-id="9fd5f-1745">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1745">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="9fd5f-1746">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1746">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="9fd5f-1747">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1747">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="9fd5f-1748">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1748">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1749">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1749">ACS</span></span>
* <span data-ttu-id="9fd5f-1750">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1750">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="9fd5f-1751">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1751">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1752">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1752">AppService</span></span>

* <span data-ttu-id="9fd5f-1753">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1753">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="9fd5f-1754">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1754">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="9fd5f-1755">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1755">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="9fd5f-1756">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1756">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-1757">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1757">Batch</span></span>
* <span data-ttu-id="9fd5f-1758">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1758">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="9fd5f-1759">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1759">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="9fd5f-1760">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1760">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="9fd5f-1761">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1761">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fd5f-1762">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1762">Batch AI</span></span> 
* <span data-ttu-id="9fd5f-1763">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1763">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fd5f-1764">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1764">Cognitive Services</span></span>
* <span data-ttu-id="9fd5f-1765">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1765">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="9fd5f-1766">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1766">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="9fd5f-1767">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1767">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="9fd5f-1768">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1768">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="9fd5f-1769">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1769">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="9fd5f-1770">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1770">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1771">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1771">Container</span></span>
* <span data-ttu-id="9fd5f-1772">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1772">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="9fd5f-1773">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1773">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="9fd5f-1774">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1774">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="9fd5f-1775">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1775">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="9fd5f-1776">DataLake</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1776">Datalake</span></span>
* <span data-ttu-id="9fd5f-1777">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1777">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="9fd5f-1778">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1778">Interactive Shell</span></span>
* <span data-ttu-id="9fd5f-1779">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1779">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="9fd5f-1780">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1780">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-1781">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1781">IoT</span></span>
* <span data-ttu-id="9fd5f-1782">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1782">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-1783">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1783">Key Vault</span></span>
* <span data-ttu-id="9fd5f-1784">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1784">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1785">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1785">Network</span></span>
* <span data-ttu-id="9fd5f-1786">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1786">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="9fd5f-1787">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1787">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="9fd5f-1788">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1788">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="9fd5f-1789">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1789">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="9fd5f-1790">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1790">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="9fd5f-1791">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1791">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="9fd5f-1792">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1792">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="9fd5f-1793">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1793">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="9fd5f-1794">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1794">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="9fd5f-1795">`network express-route create/update`: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1795">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="9fd5f-1796">`network vnet subnet create/update`: se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1796">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="9fd5f-1797">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1797">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="9fd5f-1798">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1798">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="9fd5f-1799">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1799">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="9fd5f-1800">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1800">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="9fd5f-1801">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1801">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="9fd5f-1802">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1802">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="9fd5f-1803">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1803">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-1804">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1804">RDBMS</span></span>
* <span data-ttu-id="9fd5f-1805">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1805">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="9fd5f-1806">Reserva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1806">Reservation</span></span>
* <span data-ttu-id="9fd5f-1807">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1807">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="9fd5f-1808">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1808">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="9fd5f-1809">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1809">Manage App</span></span>
* <span data-ttu-id="9fd5f-1810">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1810">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="9fd5f-1811">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1811">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1812">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1812">Role</span></span>
* <span data-ttu-id="9fd5f-1813">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1813">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="9fd5f-1814">SignalR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1814">SignalR</span></span>
* <span data-ttu-id="9fd5f-1815">Primera versión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1815">First release</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1816">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1816">Storage</span></span>
* <span data-ttu-id="9fd5f-1817">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1817">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="9fd5f-1818">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1818">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1819">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1819">VM</span></span>
* <span data-ttu-id="9fd5f-1820">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1820">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="9fd5f-1821">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1821">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="9fd5f-1822">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1822">August 28, 2018</span></span>

<span data-ttu-id="9fd5f-1823">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1823">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1824">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1824">Core</span></span>

* <span data-ttu-id="9fd5f-1825">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1825">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="9fd5f-1826">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1826">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1827">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1827">ACR</span></span>

* <span data-ttu-id="9fd5f-1828">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1828">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="9fd5f-1829">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1829">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1830">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1830">ACS</span></span>

* <span data-ttu-id="9fd5f-1831">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1831">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="9fd5f-1832">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1832">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1833">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1833">AppService</span></span>

* <span data-ttu-id="9fd5f-1834">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1834">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="9fd5f-1835">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1835">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="9fd5f-1836">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1836">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-1837">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1837">Backup</span></span>

* <span data-ttu-id="9fd5f-1838">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1838">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="9fd5f-1839">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1839">Bot Service</span></span>

* <span data-ttu-id="9fd5f-1840">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1840">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fd5f-1841">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1841">Cognitive Services</span></span>

* <span data-ttu-id="9fd5f-1842">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1842">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-1843">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1843">IoT</span></span>

* <span data-ttu-id="9fd5f-1844">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1844">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-1845">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1845">Monitor</span></span>

* <span data-ttu-id="9fd5f-1846">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1846">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="9fd5f-1847">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1847">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1848">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1848">Network</span></span>

* <span data-ttu-id="9fd5f-1849">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1849">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-1850">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1850">Resource</span></span>

* <span data-ttu-id="9fd5f-1851">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1851">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1852">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1852">Storage</span></span>

* <span data-ttu-id="9fd5f-1853">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1853">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1854">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1854">VM</span></span>

* <span data-ttu-id="9fd5f-1855">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1855">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="9fd5f-1856">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1856">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="9fd5f-1857">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1857">Auguest 14, 2018</span></span>

<span data-ttu-id="9fd5f-1858">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1858">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1859">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1859">Core</span></span>

* <span data-ttu-id="9fd5f-1860">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1860">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="9fd5f-1861">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1861">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="9fd5f-1862">Telemetría</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1862">Telemetry</span></span>

* <span data-ttu-id="9fd5f-1863">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1863">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1864">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1864">ACR</span></span>

* <span data-ttu-id="9fd5f-1865">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1865">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="9fd5f-1866">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1866">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1867">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1867">ACS</span></span>

* <span data-ttu-id="9fd5f-1868">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1868">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="9fd5f-1869">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1869">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="9fd5f-1870">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1870">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="9fd5f-1871">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1871">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="9fd5f-1872">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1872">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="9fd5f-1873">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1873">AppService</span></span>

* <span data-ttu-id="9fd5f-1874">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1874">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="9fd5f-1875">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1875">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="9fd5f-1876">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1876">BatchAI</span></span>

* <span data-ttu-id="9fd5f-1877">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1877">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="9fd5f-1878">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1878">Container</span></span>

* <span data-ttu-id="9fd5f-1879">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1879">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="9fd5f-1880">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1880">IoT</span></span>

* <span data-ttu-id="9fd5f-1881">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1881">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="9fd5f-1882">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1882">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="9fd5f-1883">Iot Central</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1883">Iot Central</span></span>

* <span data-ttu-id="9fd5f-1884">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1884">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-1885">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1885">KeyVault</span></span>


* <span data-ttu-id="9fd5f-1886">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1886">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="9fd5f-1887">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1887">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="9fd5f-1888">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1888">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="9fd5f-1889">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1889">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="9fd5f-1890">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1890">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="9fd5f-1891">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1891">Relay</span></span>

* <span data-ttu-id="9fd5f-1892">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1892">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-1893">Sql</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1893">Sql</span></span>

* <span data-ttu-id="9fd5f-1894">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1894">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1895">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1895">Storage</span></span>

* <span data-ttu-id="9fd5f-1896">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1896">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="9fd5f-1897">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1897">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="9fd5f-1898">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1898">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="9fd5f-1899">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1899">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="9fd5f-1900">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1900">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1901">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1901">VM</span></span>

* <span data-ttu-id="9fd5f-1902">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1902">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="9fd5f-1903">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1903">July 31, 2018</span></span>

<span data-ttu-id="9fd5f-1904">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1904">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1905">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1905">ACR</span></span>

* <span data-ttu-id="9fd5f-1906">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1906">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="9fd5f-1907">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1907">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1908">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1908">ACS</span></span>

* <span data-ttu-id="9fd5f-1909">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1909">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-1910">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1910">Batch</span></span>

* <span data-ttu-id="9fd5f-1911">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1911">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1912">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1912">Container</span></span>

* <span data-ttu-id="9fd5f-1913">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1913">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1914">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1914">Network</span></span>

* <span data-ttu-id="9fd5f-1915">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1915">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="9fd5f-1916">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1916">Resource</span></span>

* <span data-ttu-id="9fd5f-1917">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1917">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="9fd5f-1918">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1918">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-1919">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1919">Role</span></span>

* <span data-ttu-id="9fd5f-1920">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1920">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="9fd5f-1921">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1921">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="9fd5f-1922">Search</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1922">Search</span></span>

* <span data-ttu-id="9fd5f-1923">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1923">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fd5f-1924">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1924">Service Bus</span></span>

* <span data-ttu-id="9fd5f-1925">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1925">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="9fd5f-1926">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1926">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="9fd5f-1927">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1927">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="9fd5f-1928">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1928">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1929">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1929">Storage</span></span>

* <span data-ttu-id="9fd5f-1930">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1930">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="9fd5f-1931">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1931">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1932">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1932">VM</span></span>

* <span data-ttu-id="9fd5f-1933">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1933">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="9fd5f-1934">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1934">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="9fd5f-1935">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1935">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="9fd5f-1936">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1936">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="9fd5f-1937">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1937">July 18, 2018</span></span>

<span data-ttu-id="9fd5f-1938">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1938">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1939">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1939">Core</span></span>

* <span data-ttu-id="9fd5f-1940">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1940">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="9fd5f-1941">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1941">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="9fd5f-1942">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1942">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1943">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1943">ACR</span></span>

* <span data-ttu-id="9fd5f-1944">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1944">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="9fd5f-1945">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1945">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="9fd5f-1946">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1946">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="9fd5f-1947">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1947">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1948">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1948">ACS</span></span>

* <span data-ttu-id="9fd5f-1949">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1949">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-1950">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1950">AppService</span></span>

* <span data-ttu-id="9fd5f-1951">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1951">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-1952">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1952">Batch</span></span>

* <span data-ttu-id="9fd5f-1953">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1953">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="9fd5f-1954">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1954">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fd5f-1955">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1955">Batch AI</span></span>

* <span data-ttu-id="9fd5f-1956">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1956">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-1957">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1957">Container</span></span>

* <span data-ttu-id="9fd5f-1958">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1958">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="9fd5f-1959">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1959">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-1960">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1960">Network</span></span>

* <span data-ttu-id="9fd5f-1961">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1961">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="9fd5f-1962">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1962">Added `network nic wait`</span></span>
* <span data-ttu-id="9fd5f-1963">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1963">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="9fd5f-1964">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1964">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="9fd5f-1965">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1965">Resource</span></span>

* <span data-ttu-id="9fd5f-1966">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1966">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="9fd5f-1967">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1967">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="9fd5f-1968">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1968">Added `deployment wait` command</span></span>
* <span data-ttu-id="9fd5f-1969">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1969">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-1970">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1970">SQL</span></span>

* <span data-ttu-id="9fd5f-1971">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1971">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="9fd5f-1972">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1972">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="9fd5f-1973">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1973">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-1974">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1974">Storage</span></span>

* <span data-ttu-id="9fd5f-1975">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1975">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-1976">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1976">VM</span></span>

* <span data-ttu-id="9fd5f-1977">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1977">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="9fd5f-1978">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1978">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="9fd5f-1979">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1979">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9fd5f-1980">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1980">July 3, 2018</span></span>

<span data-ttu-id="9fd5f-1981">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1981">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-1982">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1982">AKS</span></span>

* <span data-ttu-id="9fd5f-1983">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1983">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9fd5f-1984">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1984">July 3, 2018</span></span>

<span data-ttu-id="9fd5f-1985">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1985">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-1986">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1986">Core</span></span>

* <span data-ttu-id="9fd5f-1987">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1987">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-1988">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1988">ACR</span></span>

* <span data-ttu-id="9fd5f-1989">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1989">Added polling build status</span></span>
* <span data-ttu-id="9fd5f-1990">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1990">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="9fd5f-1991">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1991">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-1992">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1992">ACS</span></span>

* <span data-ttu-id="9fd5f-1993">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1993">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="9fd5f-1994">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1994">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="9fd5f-1995">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1995">Updated options for `aks browse` command.</span></span> <span data-ttu-id="9fd5f-1996">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1996">Added `--listen-port` support</span></span>
* <span data-ttu-id="9fd5f-1997">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1997">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="9fd5f-1998">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1998">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="9fd5f-1999">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-1999">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2000">AppService</span></span>

* <span data-ttu-id="9fd5f-2001">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2001">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="9fd5f-2002">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2002">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-2003">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2003">Backup</span></span>

* <span data-ttu-id="9fd5f-2004">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2004">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="9fd5f-2005">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2005">BatchAI</span></span>

* <span data-ttu-id="9fd5f-2006">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2006">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="9fd5f-2007">Nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2007">Cloud</span></span>

* <span data-ttu-id="9fd5f-2008">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2008">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2009">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2009">Container</span></span>

* <span data-ttu-id="9fd5f-2010">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2010">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="9fd5f-2011">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2011">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="9fd5f-2012">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2012">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2013">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2013">Extension</span></span>

* <span data-ttu-id="9fd5f-2014">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2014">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2015">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2015">Network</span></span>

* <span data-ttu-id="9fd5f-2016">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2016">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-2017">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2017">Rdbms</span></span>

* <span data-ttu-id="9fd5f-2018">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2018">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2019">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2019">Resource</span></span>

* <span data-ttu-id="9fd5f-2020">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2020">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2021">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2021">VM</span></span>

* <span data-ttu-id="9fd5f-2022">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2022">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="9fd5f-2023">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2023">June 25, 2018</span></span>

<span data-ttu-id="9fd5f-2024">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2024">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="9fd5f-2025">CLI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2025">CLI</span></span>

* <span data-ttu-id="9fd5f-2026">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2026">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="9fd5f-2027">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2027">June 19, 2018</span></span>

<span data-ttu-id="9fd5f-2028">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2028">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2029">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2029">Core</span></span>

* <span data-ttu-id="9fd5f-2030">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2030">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2031">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2031">ACR</span></span>

* <span data-ttu-id="9fd5f-2032">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2032">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="9fd5f-2033">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2033">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2034">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2034">ACS</span></span>

* <span data-ttu-id="9fd5f-2035">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2035">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="9fd5f-2036">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2036">Added `--update` support</span></span>
* <span data-ttu-id="9fd5f-2037">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2037">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="9fd5f-2038">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2038">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="9fd5f-2039">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2039">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="9fd5f-2040">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2040">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="9fd5f-2041">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2041">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="9fd5f-2042">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2042">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2043">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2043">AppService</span></span>

* <span data-ttu-id="9fd5f-2044">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2044">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="9fd5f-2045">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2045">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-2046">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2046">Batch</span></span>

* <span data-ttu-id="9fd5f-2047">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2047">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fd5f-2048">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2048">Batch AI</span></span>

* <span data-ttu-id="9fd5f-2049">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2049">Added support for workspaces.</span></span> <span data-ttu-id="9fd5f-2050">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2050">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="9fd5f-2051">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2051">Added support for experiments.</span></span> <span data-ttu-id="9fd5f-2052">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2052">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="9fd5f-2053">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2053">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="9fd5f-2054">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2054">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="9fd5f-2055">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2055">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="9fd5f-2056">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2056">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="9fd5f-2057">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2057">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="9fd5f-2058">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2058">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="9fd5f-2059">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2059">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="9fd5f-2060">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2060">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="9fd5f-2061">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2061">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="9fd5f-2062">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2062">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="9fd5f-2063">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2063">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="9fd5f-2064">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2064">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="9fd5f-2065">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2065">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="9fd5f-2066">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2066">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="9fd5f-2067">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2067">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="9fd5f-2068">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2068">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9fd5f-2069">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2069">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9fd5f-2070">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2070">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="9fd5f-2071">Mapas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2071">Maps</span></span>

* <span data-ttu-id="9fd5f-2072">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2072">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2073">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2073">Network</span></span>

* <span data-ttu-id="9fd5f-2074">Se ha agregado compatibilidad para `https` a `network lb probe create` [6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2074">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="9fd5f-2075">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2075">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="9fd5f-2076">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2076">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="9fd5f-2077">Reservations</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2077">Reservations</span></span>

* <span data-ttu-id="9fd5f-2078">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2078">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="9fd5f-2079">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2079">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="9fd5f-2080">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2080">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="9fd5f-2081">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2081">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="9fd5f-2082">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2082">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="9fd5f-2083">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2083">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-2084">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2084">Role</span></span>

* <span data-ttu-id="9fd5f-2085">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2085">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2086">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2086">SQL</span></span>

* <span data-ttu-id="9fd5f-2087">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2087">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2088">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2088">Storage</span></span>

* <span data-ttu-id="9fd5f-2089">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2089">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2090">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2090">VM</span></span>

* <span data-ttu-id="9fd5f-2091">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2091">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="9fd5f-2092">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2092">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="9fd5f-2093">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2093">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9fd5f-2094">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2094">June 13, 2018</span></span>

<span data-ttu-id="9fd5f-2095">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2095">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2096">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2096">Core</span></span>

* <span data-ttu-id="9fd5f-2097">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2097">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9fd5f-2098">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2098">June 13, 2018</span></span>

<span data-ttu-id="9fd5f-2099">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2099">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-2100">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2100">AKS</span></span>

* <span data-ttu-id="9fd5f-2101">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2101">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="9fd5f-2102">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2102">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="9fd5f-2103">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2103">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="9fd5f-2104">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2104">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="9fd5f-2105">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2105">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2106">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2106">AppService</span></span>

* <span data-ttu-id="9fd5f-2107">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2107">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9fd5f-2108">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2108">June 5, 2018</span></span>

<span data-ttu-id="9fd5f-2109">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2109">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2110">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2110">Interactive</span></span>

* <span data-ttu-id="9fd5f-2111">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2111">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9fd5f-2112">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2112">June 5, 2018</span></span>

<span data-ttu-id="9fd5f-2113">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2113">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2114">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2114">Core</span></span>

* <span data-ttu-id="9fd5f-2115">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2115">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="9fd5f-2116">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2116">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2117">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2117">ACR</span></span>

* <span data-ttu-id="9fd5f-2118">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2118">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="9fd5f-2119">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2119">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="9fd5f-2120">AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2120">AKS</span></span>

* <span data-ttu-id="9fd5f-2121">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2121">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-2122">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2122">Batch</span></span>

* <span data-ttu-id="9fd5f-2123">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2123">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-2124">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2124">IOT</span></span>

* <span data-ttu-id="9fd5f-2125">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2125">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2126">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2126">Network</span></span>

* <span data-ttu-id="9fd5f-2127">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2127">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9fd5f-2128">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2128">Policy Insights</span></span>

* <span data-ttu-id="9fd5f-2129">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2129">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="9fd5f-2130">ARM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2130">ARM</span></span>

* <span data-ttu-id="9fd5f-2131">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2131">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2132">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2132">SQL</span></span>

* <span data-ttu-id="9fd5f-2133">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2133">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="9fd5f-2134">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2134">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="9fd5f-2135">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2135">Storage</span></span>

* <span data-ttu-id="9fd5f-2136">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2136">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2137">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2137">VM</span></span>

* <span data-ttu-id="9fd5f-2138">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2138">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="9fd5f-2139">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2139">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="9fd5f-2140">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2140">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="9fd5f-2141">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2141">May 22, 2018</span></span>

<span data-ttu-id="9fd5f-2142">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2142">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2143">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2143">Core</span></span>

* <span data-ttu-id="9fd5f-2144">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2144">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2145">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2145">ACS</span></span>

* <span data-ttu-id="9fd5f-2146">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2146">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="9fd5f-2147">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2147">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2148">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2148">AppService</span></span>

* <span data-ttu-id="9fd5f-2149">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2149">Improved generic update commands</span></span>
* <span data-ttu-id="9fd5f-2150">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2150">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2151">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2151">Container</span></span>

* <span data-ttu-id="9fd5f-2152">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2152">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="9fd5f-2153">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2153">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2154">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2154">Extension</span></span>

* <span data-ttu-id="9fd5f-2155">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2155">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2156">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2156">Interactive</span></span>

* <span data-ttu-id="9fd5f-2157">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2157">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="9fd5f-2158">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2158">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-2159">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2159">KeyVault</span></span>

* <span data-ttu-id="9fd5f-2160">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2160">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2161">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2161">Network</span></span>

* <span data-ttu-id="9fd5f-2162">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2162">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="9fd5f-2163">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2163">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2164">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2164">SQL</span></span>

* <span data-ttu-id="9fd5f-2165">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2165">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="9fd5f-2166">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2166">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="9fd5f-2167">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2167">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="9fd5f-2168">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2168">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="9fd5f-2169">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2169">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="9fd5f-2170">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2170">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="9fd5f-2171">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2171">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="9fd5f-2172">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2172">`edition`.</span></span> <span data-ttu-id="9fd5f-2173">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2173">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="9fd5f-2174">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2174">`elasticPoolName`.</span></span> <span data-ttu-id="9fd5f-2175">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2175">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="9fd5f-2176">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2176">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="9fd5f-2177">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2177">`edition`.</span></span> <span data-ttu-id="9fd5f-2178">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2178">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="9fd5f-2179">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2179">`dtu`.</span></span> <span data-ttu-id="9fd5f-2180">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2180">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="9fd5f-2181">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2181">`databaseDtuMin`.</span></span> <span data-ttu-id="9fd5f-2182">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2182">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="9fd5f-2183">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2183">`databaseDtuMax`.</span></span> <span data-ttu-id="9fd5f-2184">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2184">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="9fd5f-2185">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2185">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="9fd5f-2186">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2186">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2187">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2187">Storage</span></span>

* <span data-ttu-id="9fd5f-2188">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2188">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="9fd5f-2189">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2189">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2190">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2190">VM</span></span>

* <span data-ttu-id="9fd5f-2191">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2191">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="9fd5f-2192">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2192">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="9fd5f-2193">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2193">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="9fd5f-2194">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2194">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="9fd5f-2195">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2195">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="9fd5f-2196">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2196">May 7, 2018</span></span>

<span data-ttu-id="9fd5f-2197">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2197">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2198">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2198">Core</span></span>

* <span data-ttu-id="9fd5f-2199">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2199">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="9fd5f-2200">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2200">Added limited support for positional arguments</span></span>
* <span data-ttu-id="9fd5f-2201">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2201">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="9fd5f-2202">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2202">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="9fd5f-2203">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2203">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="9fd5f-2204">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2204">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="9fd5f-2205">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2205">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="9fd5f-2206">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2206">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="9fd5f-2207">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2207">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2208">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2208">ACR</span></span>

* <span data-ttu-id="9fd5f-2209">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2209">Added ACR Build commands</span></span>
* <span data-ttu-id="9fd5f-2210">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2210">Improved resource not found error messages</span></span>
* <span data-ttu-id="9fd5f-2211">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2211">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="9fd5f-2212">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2212">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="9fd5f-2213">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2213">Improved repository commands error messages</span></span>
* <span data-ttu-id="9fd5f-2214">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2214">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2215">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2215">ACS</span></span>

* <span data-ttu-id="9fd5f-2216">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2216">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="9fd5f-2217">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2217">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="9fd5f-2218">AMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2218">AMS</span></span>

* <span data-ttu-id="9fd5f-2219">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2219">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2220">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2220">Appservice</span></span>

* <span data-ttu-id="9fd5f-2221">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2221">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="9fd5f-2222">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2222">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="9fd5f-2223">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2223">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="9fd5f-2224">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2224">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9fd5f-2225">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2225">Batch AI</span></span>

* <span data-ttu-id="9fd5f-2226">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2226">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fd5f-2227">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2227">Cognitive Services</span></span>

* <span data-ttu-id="9fd5f-2228">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2228">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="9fd5f-2229">Consumo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2229">Consumption</span></span>

* <span data-ttu-id="9fd5f-2230">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2230">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2231">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2231">Container</span></span>

* <span data-ttu-id="9fd5f-2232">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2232">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9fd5f-2233">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2233">Cosmos DB</span></span>

* <span data-ttu-id="9fd5f-2234">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2234">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="9fd5f-2235">DMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2235">DMS</span></span>

* <span data-ttu-id="9fd5f-2236">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2236">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2237">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2237">Extension</span></span>

* <span data-ttu-id="9fd5f-2238">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2238">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2239">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2239">Interactive</span></span>

* <span data-ttu-id="9fd5f-2240">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2240">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="9fd5f-2241">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2241">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="9fd5f-2242">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2242">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="9fd5f-2243">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2243">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="9fd5f-2244">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2244">Lab</span></span>

* <span data-ttu-id="9fd5f-2245">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2245">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2246">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2246">Network</span></span>

* <span data-ttu-id="9fd5f-2247">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2247">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="9fd5f-2248">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2248">Profile</span></span>

* <span data-ttu-id="9fd5f-2249">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2249">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="9fd5f-2250">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2250">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="9fd5f-2251">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2251">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="9fd5f-2252">Redis</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2252">Redis</span></span>

* <span data-ttu-id="9fd5f-2253">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2253">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="9fd5f-2254">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2254">Deprecated `redis list-all`.</span></span> <span data-ttu-id="9fd5f-2255">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2255">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="9fd5f-2256">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2256">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="9fd5f-2257">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2257">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-2258">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2258">Role</span></span>

* <span data-ttu-id="9fd5f-2259">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2259">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2260">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2260">Storage</span></span>

* <span data-ttu-id="9fd5f-2261">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2261">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="9fd5f-2262">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2262">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="9fd5f-2263">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2263">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="9fd5f-2264">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2264">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="9fd5f-2265">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2265">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2266">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2266">VM</span></span>

* <span data-ttu-id="9fd5f-2267">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2267">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="9fd5f-2268">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2268">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="9fd5f-2269">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2269">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="9fd5f-2270">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2270">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="9fd5f-2271">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2271">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="9fd5f-2272">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2272">Added write accelerator support</span></span>
* <span data-ttu-id="9fd5f-2273">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2273">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="9fd5f-2274">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2274">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="9fd5f-2275">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2275">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="9fd5f-2276">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2276">April 10, 2018</span></span>

<span data-ttu-id="9fd5f-2277">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2277">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2278">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2278">ACR</span></span>

* <span data-ttu-id="9fd5f-2279">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2279">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2280">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2280">ACS</span></span>

* <span data-ttu-id="9fd5f-2281">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2281">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2282">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2282">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="9fd5f-2284">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2284">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="9fd5f-2285">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2285">BatchAI</span></span>

* <span data-ttu-id="9fd5f-2286">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2286">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="9fd5f-2287">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2287">Job level mounting</span></span>
  - <span data-ttu-id="9fd5f-2288">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2288">Environment variables with secret values</span></span>
  - <span data-ttu-id="9fd5f-2289">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2289">Performance counters settings</span></span>
  - <span data-ttu-id="9fd5f-2290">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2290">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="9fd5f-2291">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2291">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="9fd5f-2292">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2292">Usage and limits reporting</span></span>
  - <span data-ttu-id="9fd5f-2293">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2293">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="9fd5f-2294">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2294">Support for custom images</span></span>
  - <span data-ttu-id="9fd5f-2295">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2295">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="9fd5f-2296">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2296">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="9fd5f-2297">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2297">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="9fd5f-2298">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2298">National clouds are supported</span></span>
* <span data-ttu-id="9fd5f-2299">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2299">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="9fd5f-2300">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2300">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="9fd5f-2301">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2301">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="9fd5f-2302">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2302">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="9fd5f-2303">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2303">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="9fd5f-2304">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2304">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="9fd5f-2305">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2305">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="9fd5f-2306">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2306">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="9fd5f-2307">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2307">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="9fd5f-2308">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2308">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="9fd5f-2309">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2309">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="9fd5f-2310">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2310">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="9fd5f-2311">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2311">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="9fd5f-2312">Facturación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2312">Billing</span></span>

* <span data-ttu-id="9fd5f-2313">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2313">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="9fd5f-2314">Consumo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2314">Consumption</span></span>

* <span data-ttu-id="9fd5f-2315">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2315">Added `marketplace` commands</span></span>
* <span data-ttu-id="9fd5f-2316">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2316">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="9fd5f-2317">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2317">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="9fd5f-2318">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2318">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="9fd5f-2319">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2319">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="9fd5f-2320">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2320">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2321">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2321">Container</span></span>

* <span data-ttu-id="9fd5f-2322">Se han agregado los parámetros de montaje de volúmenes del repositorio de git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` y `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2322">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="9fd5f-2323">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2323">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2324">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2324">Extension</span></span>

* <span data-ttu-id="9fd5f-2325">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2325">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2326">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2326">Interactive</span></span>

* <span data-ttu-id="9fd5f-2327">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2327">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="9fd5f-2328">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2328">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="9fd5f-2329">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2329">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2330">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2330">Network</span></span>

* <span data-ttu-id="9fd5f-2331">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2331">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="9fd5f-2332">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2332">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="9fd5f-2333">4910</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2333">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="9fd5f-2334">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2334">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="9fd5f-2335">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2335">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="9fd5f-2336">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2336">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2337">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2337">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2338">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2338">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-2339">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2339">Profile</span></span>

* <span data-ttu-id="9fd5f-2340">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2340">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="9fd5f-2341">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2341">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-2342">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2342">RDBMS</span></span>

* <span data-ttu-id="9fd5f-2343">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2343">Added `georestore` command</span></span>
* <span data-ttu-id="9fd5f-2344">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2344">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2345">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2345">Resource</span></span>

* <span data-ttu-id="9fd5f-2346">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2346">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="9fd5f-2347">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2347">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2348">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2348">SQL</span></span>

* <span data-ttu-id="9fd5f-2349">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2349">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2350">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2350">Storage</span></span>

* <span data-ttu-id="9fd5f-2351">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2351">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2352">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2352">VM</span></span>

* <span data-ttu-id="9fd5f-2353">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2353">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="9fd5f-2354">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2354">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="9fd5f-2356">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2356">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="9fd5f-2357">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2357">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="9fd5f-2358">5718</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2358">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="9fd5f-2359">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2359">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="9fd5f-2360">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2360">March 27, 2018</span></span>

<span data-ttu-id="9fd5f-2361">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2361">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2362">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2362">Core</span></span>

* <span data-ttu-id="9fd5f-2363">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2363">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2364">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2364">ACS</span></span>

* <span data-ttu-id="9fd5f-2365">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2365">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2366">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2366">Appservice</span></span>

* <span data-ttu-id="9fd5f-2367">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2367">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="9fd5f-2368">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2368">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-2369">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2369">Backup</span></span>

* <span data-ttu-id="9fd5f-2370">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2370">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="9fd5f-2371">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2371">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="9fd5f-2372">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2372">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="9fd5f-2373">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2373">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2374">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2374">Container</span></span>

* <span data-ttu-id="9fd5f-2375">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2375">Added `container exec` command.</span></span> <span data-ttu-id="9fd5f-2376">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2376">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="9fd5f-2377">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2377">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2378">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2378">Extension</span></span>

* <span data-ttu-id="9fd5f-2379">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2379">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="9fd5f-2380">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2380">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="9fd5f-2381">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2381">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2382">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2382">Interactive</span></span>

* <span data-ttu-id="9fd5f-2383">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2383">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="9fd5f-2384">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2384">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="9fd5f-2385">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2385">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="9fd5f-2386">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2386">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="9fd5f-2387">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2387">Lab</span></span>

* <span data-ttu-id="9fd5f-2388">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2388">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-2389">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2389">Monitor</span></span>

* <span data-ttu-id="9fd5f-2390">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2390">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="9fd5f-2391">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2391">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="9fd5f-2392">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2392">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2393">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2393">Network</span></span>

* <span data-ttu-id="9fd5f-2394">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2394">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-2395">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2395">Profile</span></span>

* <span data-ttu-id="9fd5f-2396">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2396">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-2397">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2397">RDBMS</span></span>

* <span data-ttu-id="9fd5f-2398">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2398">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2399">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2399">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="9fd5f-2401">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2401">Role</span></span>

* <span data-ttu-id="9fd5f-2402">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2402">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="9fd5f-2403">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2403">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="9fd5f-2404">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2404">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="9fd5f-2405">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2405">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="9fd5f-2406">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2406">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2407">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2407">Storage</span></span>

* <span data-ttu-id="9fd5f-2408">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2408">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="9fd5f-2409">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2409">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2410">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2410">VM</span></span>

* <span data-ttu-id="9fd5f-2411">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2411">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="9fd5f-2412">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2412">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="9fd5f-2413">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2413">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="9fd5f-2414">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2414">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="9fd5f-2415">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2415">March 13, 2018</span></span>

<span data-ttu-id="9fd5f-2416">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2416">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2417">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2417">ACR</span></span>

* <span data-ttu-id="9fd5f-2418">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2418">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="9fd5f-2419">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2419">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="9fd5f-2420">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2420">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2421">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2421">ACS</span></span>

* <span data-ttu-id="9fd5f-2422">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2422">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="9fd5f-2423">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2423">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="9fd5f-2424">Advisor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2424">Advisor</span></span>

* <span data-ttu-id="9fd5f-2425">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2425">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="9fd5f-2426">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2426">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="9fd5f-2427">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2427">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="9fd5f-2428">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2428">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="9fd5f-2429">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2429">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2430">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2430">Appservice</span></span>

* <span data-ttu-id="9fd5f-2431">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2431">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="9fd5f-2432">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2432">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9fd5f-2433">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2433">Eventhubs</span></span>

* <span data-ttu-id="9fd5f-2434">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2434">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2435">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2435">Extension</span></span>

* <span data-ttu-id="9fd5f-2436">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2436">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2437">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2437">Interactive</span></span>

* <span data-ttu-id="9fd5f-2438">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2438">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="9fd5f-2439">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2439">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="9fd5f-2440">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2440">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="9fd5f-2441">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2441">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-2442">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2442">Monitor</span></span>

* <span data-ttu-id="9fd5f-2443">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2443">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="9fd5f-2444">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2444">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="9fd5f-2445">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2445">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="9fd5f-2446">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2446">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2447">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2447">Network</span></span>

* <span data-ttu-id="9fd5f-2448">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2448">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="9fd5f-2449">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2449">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="9fd5f-2450">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2450">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="9fd5f-2451">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2451">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-2452">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2452">Profile</span></span>

* <span data-ttu-id="9fd5f-2453">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2453">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="9fd5f-2454">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2454">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-2455">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2455">RDBMS</span></span>

* <span data-ttu-id="9fd5f-2456">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2456">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="9fd5f-2457">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2457">Service Bus</span></span>

* <span data-ttu-id="9fd5f-2458">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2458">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2459">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2459">Storage</span></span>

* <span data-ttu-id="9fd5f-2460">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2460">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="9fd5f-2461">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2461">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2462">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2462">VM</span></span>

* <span data-ttu-id="9fd5f-2463">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2463">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="9fd5f-2464">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2464">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="9fd5f-2465">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2465">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="9fd5f-2466">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2466">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="9fd5f-2467">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2467">February 27, 2018</span></span>

<span data-ttu-id="9fd5f-2468">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2468">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2469">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2469">Core</span></span>

* <span data-ttu-id="9fd5f-2470">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2470">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="9fd5f-2471">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2471">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="9fd5f-2472">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2472">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2473">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2473">ACS</span></span>

* <span data-ttu-id="9fd5f-2474">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2474">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="9fd5f-2475">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2475">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="9fd5f-2476">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2476">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="9fd5f-2477">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2477">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2478">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2478">Appservice</span></span>

* <span data-ttu-id="9fd5f-2479">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2479">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="9fd5f-2480">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2480">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9fd5f-2481">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2481">Cognitive Services</span></span>

* <span data-ttu-id="9fd5f-2482">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2482">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="9fd5f-2483">Consumo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2483">Consumption</span></span>

* <span data-ttu-id="9fd5f-2484">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2484">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="9fd5f-2485">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2485">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2486">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2486">Container</span></span>

* <span data-ttu-id="9fd5f-2487">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2487">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2488">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2488">Network</span></span>

* <span data-ttu-id="9fd5f-2489">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2489">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2490">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2490">Resource</span></span>

* <span data-ttu-id="9fd5f-2491">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2491">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-2492">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2492">Role</span></span>

* <span data-ttu-id="9fd5f-2493">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2493">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2494">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2494">SQL</span></span>

* <span data-ttu-id="9fd5f-2495">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2495">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2496">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2496">Storage</span></span>

* <span data-ttu-id="9fd5f-2497">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2497">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2498">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2498">VM</span></span>

* <span data-ttu-id="9fd5f-2499">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2499">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="9fd5f-2500">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2500">February 13, 2018</span></span>

<span data-ttu-id="9fd5f-2501">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2501">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2502">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2502">Core</span></span>

* <span data-ttu-id="9fd5f-2503">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2503">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2504">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2504">ACS</span></span>

* <span data-ttu-id="9fd5f-2505">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2505">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="9fd5f-2506">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2506">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="9fd5f-2507">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2507">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="9fd5f-2508">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2508">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="9fd5f-2509">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2509">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="9fd5f-2510">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2510">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="9fd5f-2511">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2511">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="9fd5f-2512">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2512">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2513">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2513">Appservice</span></span>

* <span data-ttu-id="9fd5f-2514">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2514">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="9fd5f-2515">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2515">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-2516">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2516">CDN</span></span>

* <span data-ttu-id="9fd5f-2517">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2517">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2518">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2518">Container</span></span>

* <span data-ttu-id="9fd5f-2519">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2519">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="9fd5f-2520">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2520">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-2521">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2521">CosmosDB</span></span>

* <span data-ttu-id="9fd5f-2522">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2522">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2523">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2523">Extension</span></span>

* <span data-ttu-id="9fd5f-2524">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2524">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="9fd5f-2525">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2525">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="9fd5f-2526">Comentarios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2526">Feedback</span></span>

* <span data-ttu-id="9fd5f-2527">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2527">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2528">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2528">Interactive</span></span>

* <span data-ttu-id="9fd5f-2529">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2529">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="9fd5f-2530">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2530">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-2531">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2531">IoT</span></span>

* <span data-ttu-id="9fd5f-2532">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2532">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9fd5f-2533">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2533">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9fd5f-2534">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2534">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2535">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2535">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-2536">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2536">Monitor</span></span>

* <span data-ttu-id="9fd5f-2537">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2537">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2538">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2538">Network</span></span>

* <span data-ttu-id="9fd5f-2539">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2539">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="9fd5f-2540">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2540">Profile</span></span>

* <span data-ttu-id="9fd5f-2541">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2541">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2542">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2542">Resource</span></span>

* <span data-ttu-id="9fd5f-2543">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2543">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-2544">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2544">Role</span></span>

* <span data-ttu-id="9fd5f-2545">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2545">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2546">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2546">SQL</span></span>

* <span data-ttu-id="9fd5f-2547">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2547">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="9fd5f-2548">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2548">Added `sql db rename`</span></span>
* <span data-ttu-id="9fd5f-2549">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2549">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2550">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2550">Storage</span></span>

* <span data-ttu-id="9fd5f-2551">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2551">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2552">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2552">VM</span></span>

* <span data-ttu-id="9fd5f-2553">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2553">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="9fd5f-2554">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2554">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="9fd5f-2555">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2555">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="9fd5f-2556">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2556">January 31, 2018</span></span>

<span data-ttu-id="9fd5f-2557">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2557">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2558">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2558">Core</span></span>

* <span data-ttu-id="9fd5f-2559">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2559">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="9fd5f-2560">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2560">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="9fd5f-2561">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2561">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="9fd5f-2562">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2562">Use `--verbose` to see</span></span>
* <span data-ttu-id="9fd5f-2563">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2563">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2564">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2564">ACS</span></span>

* <span data-ttu-id="9fd5f-2565">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2565">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="9fd5f-2566">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2566">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2567">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2567">Appservice</span></span>

* <span data-ttu-id="9fd5f-2568">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2568">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="9fd5f-2569">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2569">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-2570">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2570">CDN</span></span>

* <span data-ttu-id="9fd5f-2571">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2571">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-2572">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2572">CosmosDB</span></span>

* <span data-ttu-id="9fd5f-2573">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2573">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2574">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2574">Interactive</span></span>

* <span data-ttu-id="9fd5f-2575">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2575">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2576">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2576">Network</span></span>

* <span data-ttu-id="9fd5f-2577">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2577">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="9fd5f-2578">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2578">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="9fd5f-2579">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2579">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="9fd5f-2580">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2580">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="9fd5f-2581">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2581">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="9fd5f-2582">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2582">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="9fd5f-2583">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2583">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="9fd5f-2584">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2584">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="9fd5f-2585">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2585">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="9fd5f-2586">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2586">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-2587">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2587">Profile</span></span>

* <span data-ttu-id="9fd5f-2588">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2588">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2589">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2589">Resource</span></span>

* <span data-ttu-id="9fd5f-2590">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2590">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2591">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2591">Storage</span></span>

* <span data-ttu-id="9fd5f-2592">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2592">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="9fd5f-2593">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2593">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="9fd5f-2594">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2594">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="9fd5f-2595">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2595">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="9fd5f-2596">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2596">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2597">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2597">VM</span></span>

* <span data-ttu-id="9fd5f-2598">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2598">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="9fd5f-2599">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2599">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="9fd5f-2600">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2600">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="9fd5f-2601">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2601">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="9fd5f-2602">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2602">January 17, 2018</span></span>

<span data-ttu-id="9fd5f-2603">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2603">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2604">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2604">ACR</span></span>

* <span data-ttu-id="9fd5f-2605">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2605">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="9fd5f-2606">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2606">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2607">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2607">ACS</span></span>

* <span data-ttu-id="9fd5f-2608">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2608">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="9fd5f-2609">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2609">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2610">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2610">Appservice</span></span>

* <span data-ttu-id="9fd5f-2611">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2611">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="9fd5f-2612">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2612">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="9fd5f-2613">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2613">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-2614">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2614">Backup</span></span>

* <span data-ttu-id="9fd5f-2615">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2615">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="9fd5f-2616">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2616">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="9fd5f-2617">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2617">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="9fd5f-2618">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2618">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="9fd5f-2619">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2619">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-2620">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2620">Batch</span></span>

* <span data-ttu-id="9fd5f-2621">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2621">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="9fd5f-2622">Nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2622">Cloud</span></span>

* <span data-ttu-id="9fd5f-2623">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2623">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="9fd5f-2624">Consumo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2624">Consumption</span></span>

* <span data-ttu-id="9fd5f-2625">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2625">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="9fd5f-2626">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2626">Event Grid</span></span>

* <span data-ttu-id="9fd5f-2627">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2627">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9fd5f-2628">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2628">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9fd5f-2629">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2629">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="9fd5f-2630">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2630">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="9fd5f-2631">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2631">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="9fd5f-2632">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2632">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="9fd5f-2633">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2633">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="9fd5f-2634">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2634">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-2635">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2635">Interactive</span></span>

* <span data-ttu-id="9fd5f-2636">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2636">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="9fd5f-2637">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2637">Fixed errors on startup</span></span>
* <span data-ttu-id="9fd5f-2638">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2638">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-2639">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2639">IoT</span></span>

* <span data-ttu-id="9fd5f-2640">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2640">Added support for device provisioning service</span></span>
* <span data-ttu-id="9fd5f-2641">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2641">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="9fd5f-2642">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2642">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-2643">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2643">Monitor</span></span>

* <span data-ttu-id="9fd5f-2644">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2644">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="9fd5f-2645">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2645">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="9fd5f-2646">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2646">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2647">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2647">Network</span></span>

* <span data-ttu-id="9fd5f-2648">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2648">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="9fd5f-2649">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2649">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-2650">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2650">Profile</span></span>

* <span data-ttu-id="9fd5f-2651">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2651">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-2652">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2652">Role</span></span>

* <span data-ttu-id="9fd5f-2653">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2653">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fd5f-2654">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2654">Service Fabric</span></span>

* <span data-ttu-id="9fd5f-2655">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2655">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="9fd5f-2656">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2656">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2657">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2657">VM</span></span>

* <span data-ttu-id="9fd5f-2658">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2658">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="9fd5f-2659">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2659">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="9fd5f-2660">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2660">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="9fd5f-2661">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2661">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="9fd5f-2662">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2662">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="9fd5f-2663">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2663">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fd5f-2664">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2664">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fd5f-2665">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2665">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="9fd5f-2666">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2666">December 19, 2017</span></span>

<span data-ttu-id="9fd5f-2667">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2667">Version 2.0.23</span></span>

* <span data-ttu-id="9fd5f-2668">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2668">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2669">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2669">Container</span></span>

* <span data-ttu-id="9fd5f-2670">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2670">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2671">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2671">Network</span></span>

* <span data-ttu-id="9fd5f-2672">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2672">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2673">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2673">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2674">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2674">Storage</span></span>

* <span data-ttu-id="9fd5f-2675">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2675">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2676">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2676">VM</span></span>

* <span data-ttu-id="9fd5f-2677">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2677">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="9fd5f-2678">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2678">December 5, 2017</span></span>

<span data-ttu-id="9fd5f-2679">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2679">Version 2.0.22</span></span>

* <span data-ttu-id="9fd5f-2680">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2680">Removed `az component` commands.</span></span> <span data-ttu-id="9fd5f-2681">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2681">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2682">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2682">Core</span></span>
* <span data-ttu-id="9fd5f-2683">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2683">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="9fd5f-2684">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2684">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2685">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2685">ACS</span></span>

* <span data-ttu-id="9fd5f-2686">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2686">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="9fd5f-2687">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2687">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="9fd5f-2688">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2688">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="9fd5f-2689">Advisor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2689">Advisor</span></span>

* <span data-ttu-id="9fd5f-2690">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2690">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2691">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2691">Appservice</span></span>

* <span data-ttu-id="9fd5f-2692">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2692">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="9fd5f-2693">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2693">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="9fd5f-2694">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2694">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="9fd5f-2695">Consumo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2695">Consumption</span></span>

* <span data-ttu-id="9fd5f-2696">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2696">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2697">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2697">Container</span></span>

* <span data-ttu-id="9fd5f-2698">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2698">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-2699">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2699">Monitor</span></span>

* <span data-ttu-id="9fd5f-2700">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2700">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2701">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2701">Resource</span></span>

* <span data-ttu-id="9fd5f-2702">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2702">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-2703">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2703">Role</span></span>

* <span data-ttu-id="9fd5f-2704">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2704">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="9fd5f-2705">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2705">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="9fd5f-2706">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2706">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2707">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2707">SQL</span></span>

* <span data-ttu-id="9fd5f-2708">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2708">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="9fd5f-2709">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2709">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2710">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2710">VM</span></span>

* <span data-ttu-id="9fd5f-2711">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2711">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="9fd5f-2712">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2712">November 14, 2017</span></span>

<span data-ttu-id="9fd5f-2713">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2713">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2714">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2714">ACR</span></span>

* <span data-ttu-id="9fd5f-2715">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2715">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="9fd5f-2716">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2716">ACS</span></span>

* <span data-ttu-id="9fd5f-2717">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2717">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="9fd5f-2718">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2718">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="9fd5f-2719">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2719">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="9fd5f-2720">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2720">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="9fd5f-2721">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2721">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2722">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2722">Appservice</span></span>

* <span data-ttu-id="9fd5f-2723">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2723">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="9fd5f-2724">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2724">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="9fd5f-2725">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2725">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="9fd5f-2726">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2726">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="9fd5f-2727">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2727">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="9fd5f-2728">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2728">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-2729">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2729">Batch</span></span>

* <span data-ttu-id="9fd5f-2730">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2730">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="9fd5f-2731">Batchai</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2731">Batchai</span></span>

* <span data-ttu-id="9fd5f-2732">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2732">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="9fd5f-2733">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2733">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="9fd5f-2734">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2734">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="9fd5f-2735">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2735">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="9fd5f-2736">Nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2736">Cloud</span></span>

* <span data-ttu-id="9fd5f-2737">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2737">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2738">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2738">Container</span></span>

* <span data-ttu-id="9fd5f-2739">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2739">Added support to open multiple ports</span></span>
* <span data-ttu-id="9fd5f-2740">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2740">Added container group restart policy</span></span>
* <span data-ttu-id="9fd5f-2741">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2741">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="9fd5f-2742">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2742">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9fd5f-2743">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2743">Data Lake Analytics</span></span>

* <span data-ttu-id="9fd5f-2744">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2744">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9fd5f-2745">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2745">Data Lake Store</span></span>

* <span data-ttu-id="9fd5f-2746">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2746">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2747">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2747">Extension</span></span>

* <span data-ttu-id="9fd5f-2748">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2748">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="9fd5f-2749">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2749">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-2750">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2750">IoT</span></span>

* <span data-ttu-id="9fd5f-2751">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2751">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-2752">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2752">Monitor</span></span>

* <span data-ttu-id="9fd5f-2753">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2753">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2754">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2754">Network</span></span>

* <span data-ttu-id="9fd5f-2755">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2755">Added support for CAA DNS records</span></span>
* <span data-ttu-id="9fd5f-2756">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2756">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="9fd5f-2757">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2757">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="9fd5f-2758">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2758">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="9fd5f-2759">Reservations</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2759">Reservations</span></span>

* <span data-ttu-id="9fd5f-2760">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2760">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2761">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2761">Resource</span></span>

* <span data-ttu-id="9fd5f-2762">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2762">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2763">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2763">SQL</span></span>

* <span data-ttu-id="9fd5f-2764">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2764">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2765">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2765">Storage</span></span>

* <span data-ttu-id="9fd5f-2766">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2766">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="9fd5f-2767">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2767">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="9fd5f-2768">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2768">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="9fd5f-2769">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2769">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="9fd5f-2770">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2770">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="9fd5f-2771">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2771">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="9fd5f-2772">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2772">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2773">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2773">VM</span></span>

* <span data-ttu-id="9fd5f-2774">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2774">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="9fd5f-2775">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2775">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="9fd5f-2776">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2776">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="9fd5f-2777">Cambio de nombre de `vm format-secret` a `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2777">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="9fd5f-2778">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2778">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="9fd5f-2779">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2779">October 24, 2017</span></span>

<span data-ttu-id="9fd5f-2780">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2780">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2781">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2781">Core</span></span>

* <span data-ttu-id="9fd5f-2782">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2782">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-2783">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2783">ACR</span></span>

* <span data-ttu-id="9fd5f-2784">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2784">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="9fd5f-2785">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2785">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="9fd5f-2786">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2786">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2787">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2787">ACS</span></span>

* <span data-ttu-id="9fd5f-2788">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2788">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="9fd5f-2789">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2789">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2790">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2790">Appservice</span></span>

* <span data-ttu-id="9fd5f-2791">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2791">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="9fd5f-2792">Componente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2792">Component</span></span>

* <span data-ttu-id="9fd5f-2793">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2793">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-2794">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2794">Monitor</span></span>

* <span data-ttu-id="9fd5f-2795">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2795">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2796">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2796">Resource</span></span>

* <span data-ttu-id="9fd5f-2797">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2797">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="9fd5f-2798">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2798">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2799">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2799">VM</span></span>

* <span data-ttu-id="9fd5f-2800">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2800">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="9fd5f-2801">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2801">October 9, 2017</span></span>

<span data-ttu-id="9fd5f-2802">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2802">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2803">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2803">Core</span></span>

* <span data-ttu-id="9fd5f-2804">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2804">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2805">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2805">Appservice</span></span>

* <span data-ttu-id="9fd5f-2806">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2806">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-2807">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2807">Batch</span></span>

* <span data-ttu-id="9fd5f-2808">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2808">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="9fd5f-2809">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2809">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="9fd5f-2810">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2810">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="9fd5f-2811">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2811">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="9fd5f-2812">Batchai</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2812">Batchai</span></span>

* <span data-ttu-id="9fd5f-2813">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2813">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-2814">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2814">Keyvault</span></span>

* <span data-ttu-id="9fd5f-2815">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2815">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="9fd5f-2816">(#4448)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2816">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="9fd5f-2817">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2817">Network</span></span>

* <span data-ttu-id="9fd5f-2818">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2818">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="9fd5f-2819">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2819">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2820">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2820">Resource</span></span>

* <span data-ttu-id="9fd5f-2821">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2821">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="9fd5f-2822">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2822">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="9fd5f-2823">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2823">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="9fd5f-2824">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2824">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2825">Sql</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2825">Sql</span></span>

* <span data-ttu-id="9fd5f-2826">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2826">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="9fd5f-2827">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2827">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="9fd5f-2828">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2828">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2829">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2829">Storage</span></span>

* <span data-ttu-id="9fd5f-2830">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2830">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2831">Vm</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2831">Vm</span></span>

* <span data-ttu-id="9fd5f-2832">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2832">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="9fd5f-2833">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2833">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="9fd5f-2834">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2834">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="9fd5f-2835">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2835">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="9fd5f-2836">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2836">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="9fd5f-2837">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2837">September 22, 2017</span></span>

<span data-ttu-id="9fd5f-2838">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2838">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2839">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2839">Resource</span></span>

* <span data-ttu-id="9fd5f-2840">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2840">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="9fd5f-2841">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2841">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="9fd5f-2842">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2842">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="9fd5f-2843">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2843">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2844">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2844">Network</span></span>

* <span data-ttu-id="9fd5f-2845">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2845">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="9fd5f-2846">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2846">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="9fd5f-2847">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2847">Added `asg` application security group commands</span></span>
* <span data-ttu-id="9fd5f-2848">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2848">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="9fd5f-2849">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2849">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2850">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2850">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2851">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2851">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2852">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2852">Storage</span></span>

* <span data-ttu-id="9fd5f-2853">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2853">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9fd5f-2854">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2854">Eventgrid</span></span>

* <span data-ttu-id="9fd5f-2855">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2855">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2856">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2856">SQL</span></span>

* <span data-ttu-id="9fd5f-2857">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2857">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="9fd5f-2858">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2858">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="9fd5f-2859">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2859">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-2860">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2860">Keyvault</span></span>

* <span data-ttu-id="9fd5f-2861">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2861">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2862">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2862">VM</span></span>

* <span data-ttu-id="9fd5f-2863">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2863">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="9fd5f-2864">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2864">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="9fd5f-2865">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2865">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="9fd5f-2866">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2866">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="9fd5f-2867">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2867">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="9fd5f-2868">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2868">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2869">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2869">ACS</span></span>

* <span data-ttu-id="9fd5f-2870">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2870">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2871">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2871">Appservice</span></span>

* <span data-ttu-id="9fd5f-2872">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2872">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9fd5f-2873">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2873">Backup</span></span>

* <span data-ttu-id="9fd5f-2874">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2874">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="9fd5f-2875">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2875">September 11, 2017</span></span>

<span data-ttu-id="9fd5f-2876">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2876">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="9fd5f-2877">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2877">Core</span></span>

* <span data-ttu-id="9fd5f-2878">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2878">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="9fd5f-2879">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2879">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2880">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2880">Acs</span></span>

* <span data-ttu-id="9fd5f-2881">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2881">Added `acs list-locations` command</span></span>
* <span data-ttu-id="9fd5f-2882">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2882">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2883">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2883">Appservice</span></span>

* <span data-ttu-id="9fd5f-2884">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2884">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-2885">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2885">CDN</span></span>

* <span data-ttu-id="9fd5f-2886">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2886">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="9fd5f-2887">Extensión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2887">Extension</span></span>

* <span data-ttu-id="9fd5f-2888">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2888">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-2889">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2889">Keyvault</span></span>

* <span data-ttu-id="9fd5f-2890">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2890">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2891">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2891">Network</span></span>

* <span data-ttu-id="9fd5f-2892">Cambio de nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2892">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9fd5f-2893">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2893">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="9fd5f-2894">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2894">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="9fd5f-2895">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2895">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9fd5f-2896">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2896">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-2897">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2897">Resource</span></span>

* <span data-ttu-id="9fd5f-2898">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2898">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="9fd5f-2899">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2899">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="9fd5f-2900">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2900">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="9fd5f-2901">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2901">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-2902">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2902">SQL</span></span>

* <span data-ttu-id="9fd5f-2903">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2903">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2904">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2904">VM</span></span>

* <span data-ttu-id="9fd5f-2905">Solucionado: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2905">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="9fd5f-2906">Solucionado: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2906">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="9fd5f-2907">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2907">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="9fd5f-2908">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2908">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="9fd5f-2909">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2909">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="9fd5f-2910">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2910">August 31, 2017</span></span>

<span data-ttu-id="9fd5f-2911">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2911">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-2912">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2912">Keyvault</span></span>

* <span data-ttu-id="9fd5f-2913">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2913">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="9fd5f-2914">Sf</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2914">Sf</span></span>

* <span data-ttu-id="9fd5f-2915">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2915">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2916">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2916">Storage</span></span>

* <span data-ttu-id="9fd5f-2917">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2917">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="9fd5f-2918">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2918">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="9fd5f-2919">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2919">August 28, 2017</span></span>

<span data-ttu-id="9fd5f-2920">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2920">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="9fd5f-2921">CLI</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2921">CLI</span></span>

* <span data-ttu-id="9fd5f-2922">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2922">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2923">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2923">ACS</span></span>

* <span data-ttu-id="9fd5f-2924">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2924">Corrected preview regions</span></span>
* <span data-ttu-id="9fd5f-2925">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2925">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="9fd5f-2926">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2926">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2927">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2927">Appservice</span></span>

* <span data-ttu-id="9fd5f-2928">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2928">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="9fd5f-2929">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2929">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="9fd5f-2930">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2930">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="9fd5f-2931">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2931">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="9fd5f-2932">Solucionado: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2932">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-2933">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2933">IoT</span></span>

* <span data-ttu-id="9fd5f-2934">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2934">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2935">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2935">Network</span></span>

* <span data-ttu-id="9fd5f-2936">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2936">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9fd5f-2937">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2937">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2938">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2938">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9fd5f-2939">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2939">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9fd5f-2940">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2940">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-2941">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2941">Profile</span></span>

* <span data-ttu-id="9fd5f-2942">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2942">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fd5f-2943">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2943">Service Fabric</span></span>

* <span data-ttu-id="9fd5f-2944">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2944">Preview release</span></span>
* <span data-ttu-id="9fd5f-2945">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2945">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="9fd5f-2946">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2946">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="9fd5f-2947">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2947">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2948">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2948">Storage</span></span>

* <span data-ttu-id="9fd5f-2949">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2949">Enabled setting blob tier</span></span>
* <span data-ttu-id="9fd5f-2950">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2950">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="9fd5f-2951">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2951">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="9fd5f-2952">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2952">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="9fd5f-2953">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2953">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="9fd5f-2954">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2954">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2955">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2955">VM</span></span>

* <span data-ttu-id="9fd5f-2956">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2956">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="9fd5f-2957">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2957">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="9fd5f-2958">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2958">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="9fd5f-2959">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2959">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="9fd5f-2960">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2960">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="9fd5f-2961">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2961">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="9fd5f-2962">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2962">August 15, 2017</span></span>

<span data-ttu-id="9fd5f-2963">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2963">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2964">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2964">ACS</span></span>

* <span data-ttu-id="9fd5f-2965">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2965">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-2966">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2966">Appservice</span></span>

* <span data-ttu-id="9fd5f-2967">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2967">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="9fd5f-2968">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2968">Event Grid</span></span>

* <span data-ttu-id="9fd5f-2969">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2969">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="9fd5f-2970">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2970">August 11, 2017</span></span>

<span data-ttu-id="9fd5f-2971">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2971">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-2972">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2972">ACS</span></span>

* <span data-ttu-id="9fd5f-2973">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2973">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-2974">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2974">Batch</span></span>

* <span data-ttu-id="9fd5f-2975">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2975">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="9fd5f-2976">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2976">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="9fd5f-2977">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2977">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="9fd5f-2978">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2978">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="9fd5f-2979">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2979">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="9fd5f-2980">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2980">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="9fd5f-2981">Componente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2981">Component</span></span>

* <span data-ttu-id="9fd5f-2982">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2982">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="9fd5f-2983">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2983">Container</span></span>

* <span data-ttu-id="9fd5f-2984">`create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2984">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="9fd5f-2985">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2985">Data Lake Store</span></span>

* <span data-ttu-id="9fd5f-2986">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2986">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="9fd5f-2987">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2987">Event Grid</span></span>

* <span data-ttu-id="9fd5f-2988">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2988">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-2989">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2989">Network</span></span>

* <span data-ttu-id="9fd5f-2990">`lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2990">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="9fd5f-2991">`application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2991">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="9fd5f-2992">`application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2992">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="9fd5f-2993">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2993">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-2994">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2994">Profile</span></span>

* <span data-ttu-id="9fd5f-2995">`account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2995">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-2996">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2996">Storage</span></span>

* <span data-ttu-id="9fd5f-2997">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2997">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-2998">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2998">VM</span></span>

* <span data-ttu-id="9fd5f-2999">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-2999">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="9fd5f-3000">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3000">Exposed `list-skus` command</span></span>
* <span data-ttu-id="9fd5f-3001">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3001">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="9fd5f-3002">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3002">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="9fd5f-3003">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3003">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="9fd5f-3004">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3004">July 28, 2017</span></span>

<span data-ttu-id="9fd5f-3005">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3005">Version 2.0.12</span></span>

* <span data-ttu-id="9fd5f-3006">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3006">Added container commands</span></span>
* <span data-ttu-id="9fd5f-3007">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3007">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="9fd5f-3008">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3008">Core</span></span>

* <span data-ttu-id="9fd5f-3009">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3009">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="9fd5f-3010">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3010">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="9fd5f-3011">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3011">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="9fd5f-3012">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3012">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="9fd5f-3013">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3013">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="9fd5f-3014">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3014">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="9fd5f-3015">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3015">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9fd5f-3016">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3016">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="9fd5f-3017">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3017">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="9fd5f-3018">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3018">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="9fd5f-3019">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3019">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="9fd5f-3020">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3020">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="9fd5f-3021">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3021">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="9fd5f-3022">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3022">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="9fd5f-3023">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3023">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="9fd5f-3024">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3024">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="9fd5f-3025">ACR</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3025">ACR</span></span>

* <span data-ttu-id="9fd5f-3026">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3026">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="9fd5f-3027">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3027">Support SKU update for managed registries</span></span>
* <span data-ttu-id="9fd5f-3028">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3028">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="9fd5f-3029">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3029">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="9fd5f-3030">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3030">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="9fd5f-3031">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3031">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-3032">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3032">ACS</span></span>

* <span data-ttu-id="9fd5f-3033">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3033">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-3034">Appservice</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3034">Appservice</span></span>

* <span data-ttu-id="9fd5f-3035">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3035">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="9fd5f-3036">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3036">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="9fd5f-3037">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3037">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="9fd5f-3038">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3038">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="9fd5f-3039">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3039">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="9fd5f-3040">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3040">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="9fd5f-3041">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3041">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="9fd5f-3042">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3042">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="9fd5f-3043">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3043">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="9fd5f-3044">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3044">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="9fd5f-3045">Batch</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3045">Batch</span></span>

* <span data-ttu-id="9fd5f-3046">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3046">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="9fd5f-3047">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3047">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="9fd5f-3048">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3048">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="9fd5f-3049">CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3049">CDN</span></span>

* <span data-ttu-id="9fd5f-3050">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3050">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="9fd5f-3051">Nube</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3051">Cloud</span></span>

* <span data-ttu-id="9fd5f-3052">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3052">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="9fd5f-3053">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3053">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="9fd5f-3054">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3054">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="9fd5f-3055">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3055">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="9fd5f-3056">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3056">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-3057">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3057">CosmosDB</span></span>

* <span data-ttu-id="9fd5f-3058">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3058">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="9fd5f-3059">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3059">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9fd5f-3060">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3060">Data Lake Analytics</span></span>

* <span data-ttu-id="9fd5f-3061">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3061">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="9fd5f-3062">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3062">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="9fd5f-3063">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3063">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9fd5f-3064">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3064">Data Lake Store</span></span>

* <span data-ttu-id="9fd5f-3065">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3065">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="9fd5f-3066">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3066">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="9fd5f-3067">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3067">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="9fd5f-3068">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3068">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="9fd5f-3069">Interactive</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3069">Interactive</span></span>

* <span data-ttu-id="9fd5f-3070">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3070">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="9fd5f-3071">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3071">Increased test coverage</span></span>
* <span data-ttu-id="9fd5f-3072">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3072">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="9fd5f-3073">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3073">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="9fd5f-3074">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3074">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="9fd5f-3075">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3075">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="9fd5f-3076">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3076">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9fd5f-3077">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3077">Added `--progress` flag</span></span>
* <span data-ttu-id="9fd5f-3078">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3078">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="9fd5f-3079">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3079">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="9fd5f-3080">IoT</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3080">IoT</span></span>

* <span data-ttu-id="9fd5f-3081">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3081">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="9fd5f-3082">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3082">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="9fd5f-3083">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3083">Key vault</span></span>

* <span data-ttu-id="9fd5f-3084">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3084">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="9fd5f-3085">Subcomandos de `keyvault``purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3085">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="9fd5f-3086">Subcomandos de `keyvault secret``backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3086">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9fd5f-3087">Subcomandos de `keyvault certificate``purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3087">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9fd5f-3088">Subcomandos de `keyvault key``purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3088">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="9fd5f-3089">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3089">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="9fd5f-3090">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3090">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="9fd5f-3091">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3091">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="9fd5f-3092">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3092">Lab</span></span>

* <span data-ttu-id="9fd5f-3093">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3093">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="9fd5f-3094">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3094">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-3095">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3095">Monitor</span></span>

* <span data-ttu-id="9fd5f-3096">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3096">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="9fd5f-3097">Cambio de nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3097">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="9fd5f-3098">Cambio de nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3098">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="9fd5f-3099">Cambio de nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3099">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="9fd5f-3100">Cambio de nombre de `monitor alert-rules` a `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3100">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="9fd5f-3101">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3101">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="9fd5f-3102">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3102">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="9fd5f-3103">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3103">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="9fd5f-3104">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3104">`location` no longer required</span></span>
  * <span data-ttu-id="9fd5f-3105">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3105">Add name and ID support for target</span></span>
  * <span data-ttu-id="9fd5f-3106">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3106">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="9fd5f-3107">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3107">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="9fd5f-3108">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3108">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="9fd5f-3109">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3109">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="9fd5f-3110">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3110">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="9fd5f-3111">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3111">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-3112">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3112">Network</span></span>

* <span data-ttu-id="9fd5f-3113">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3113">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="9fd5f-3114">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3114">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="9fd5f-3115">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3115">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="9fd5f-3116">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3116">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="9fd5f-3117">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3117">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="9fd5f-3118">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3118">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="9fd5f-3119">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3119">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="9fd5f-3120">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3120">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="9fd5f-3121">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3121">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="9fd5f-3122">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3122">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="9fd5f-3123">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3123">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="9fd5f-3124">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3124">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="9fd5f-3125">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3125">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="9fd5f-3126">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3126">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="9fd5f-3127">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3127">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="9fd5f-3128">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3128">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="9fd5f-3129">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3129">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="9fd5f-3130">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3130">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="9fd5f-3131">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3131">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="9fd5f-3132">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3132">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="9fd5f-3133">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3133">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="9fd5f-3134">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3134">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="9fd5f-3135">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3135">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="9fd5f-3136">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3136">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="9fd5f-3137">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3137">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="9fd5f-3138">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3138">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="9fd5f-3139">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3139">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-3140">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3140">Profile</span></span>

* <span data-ttu-id="9fd5f-3141">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3141">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="9fd5f-3142">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3142">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="9fd5f-3143">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3143">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="9fd5f-3144">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3144">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="9fd5f-3145">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3145">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="9fd5f-3146">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3146">RDBMS</span></span>

* <span data-ttu-id="9fd5f-3147">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3147">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="9fd5f-3148">Se ha corregido el problema por el que `%s` no se procesaba porque faltaba `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3148">Fixed `%s` not processed because of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="9fd5f-3149">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3149">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="9fd5f-3150">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3150">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-3151">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3151">Resource</span></span>

* <span data-ttu-id="9fd5f-3152">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3152">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="9fd5f-3153">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3153">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="9fd5f-3154">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3154">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="9fd5f-3155">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3155">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="9fd5f-3156">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3156">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="9fd5f-3157">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3157">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="9fd5f-3158">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3158">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="9fd5f-3159">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3159">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-3160">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3160">Role</span></span>

* <span data-ttu-id="9fd5f-3161">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3161">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="9fd5f-3162">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3162">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="9fd5f-3163">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3163">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="9fd5f-3164">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3164">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="9fd5f-3165">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3165">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9fd5f-3166">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3166">Service Fabric</span></span>
* <span data-ttu-id="9fd5f-3167">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3167">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="9fd5f-3168">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3168">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="9fd5f-3169">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3169">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-3170">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3170">SQL</span></span>

* <span data-ttu-id="9fd5f-3171">Se eliminó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3171">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="9fd5f-3172">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3172">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="9fd5f-3173">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3173">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-3174">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3174">Storage</span></span>

* <span data-ttu-id="9fd5f-3175">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3175">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="9fd5f-3176">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3176">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="9fd5f-3177">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3177">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="9fd5f-3178">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3178">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="9fd5f-3179">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3179">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="9fd5f-3180">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3180">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-3181">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3181">VM</span></span>

* <span data-ttu-id="9fd5f-3182">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3182">Support configuring nsg</span></span>
* <span data-ttu-id="9fd5f-3183">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3183">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="9fd5f-3184">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3184">Support managed service identities</span></span>
* <span data-ttu-id="9fd5f-3185">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3185">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="9fd5f-3186">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3186">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="9fd5f-3187">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3187">May 10, 2017</span></span>

<span data-ttu-id="9fd5f-3188">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3188">Version 2.0.6</span></span>

* <span data-ttu-id="9fd5f-3189">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3189">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="9fd5f-3190">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3190">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="9fd5f-3191">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3191">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="9fd5f-3192">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3192">Include Cognitive Services module</span></span>
* <span data-ttu-id="9fd5f-3193">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3193">Include Service Fabric module</span></span>
* <span data-ttu-id="9fd5f-3194">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3194">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="9fd5f-3195">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3195">Add support for CDN commands</span></span>
* <span data-ttu-id="9fd5f-3196">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3196">Remove Container module</span></span>
* <span data-ttu-id="9fd5f-3197">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3197">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="9fd5f-3198">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3198">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="9fd5f-3199">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3199">Core</span></span>

* <span data-ttu-id="9fd5f-3200">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3200">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="9fd5f-3201">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3201">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="9fd5f-3202">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3202">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="9fd5f-3203">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3203">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="9fd5f-3204">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3204">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="9fd5f-3205">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3205">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="9fd5f-3206">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3206">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="9fd5f-3207">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3207">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="9fd5f-3208">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3208">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="9fd5f-3209">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3209">core: Improved performance</span></span>
* <span data-ttu-id="9fd5f-3210">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3210">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="9fd5f-3211">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3211">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-3212">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3212">ACS</span></span>

* <span data-ttu-id="9fd5f-3213">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3213">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="9fd5f-3214">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3214">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="9fd5f-3215">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3215">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="9fd5f-3216">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3216">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-3217">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3217">AppService</span></span>

* <span data-ttu-id="9fd5f-3218">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3218">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="9fd5f-3219">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3219">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="9fd5f-3220">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3220">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="9fd5f-3221">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3221">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="9fd5f-3222">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3222">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="9fd5f-3223">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3223">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="9fd5f-3224">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3224">support slot swap with preview</span></span>
* <span data-ttu-id="9fd5f-3225">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3225">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="9fd5f-3226">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3226">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9fd5f-3227">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3227">CosmosDB</span></span>

* <span data-ttu-id="9fd5f-3228">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3228">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="9fd5f-3229">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3229">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="9fd5f-3230">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3230">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="9fd5f-3231">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3231">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9fd5f-3232">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3232">Data Lake Analytics</span></span>

* <span data-ttu-id="9fd5f-3233">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3233">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="9fd5f-3234">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3234">Add support for new catalog item type: package.</span></span> <span data-ttu-id="9fd5f-3235">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3235">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="9fd5f-3236">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3236">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="9fd5f-3237">Tabla</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3237">Table</span></span>
  * <span data-ttu-id="9fd5f-3238">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3238">Table valued function</span></span>
  * <span data-ttu-id="9fd5f-3239">Ver</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3239">View</span></span>
  * <span data-ttu-id="9fd5f-3240">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3240">Table Statistics.</span></span> <span data-ttu-id="9fd5f-3241">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3241">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9fd5f-3242">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3242">Data Lake Store</span></span>

* <span data-ttu-id="9fd5f-3243">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3243">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="9fd5f-3244">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3244">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="9fd5f-3245">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3245">missed help for access show.</span></span> <span data-ttu-id="9fd5f-3246">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3246">adding it.</span></span> <span data-ttu-id="9fd5f-3247">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3247">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="9fd5f-3248">Buscar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3248">Find</span></span>

* <span data-ttu-id="9fd5f-3249">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3249">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="9fd5f-3250">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3250">KeyVault</span></span>

* <span data-ttu-id="9fd5f-3251">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3251">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="9fd5f-3252">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3252">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="9fd5f-3253">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3253">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="9fd5f-3254">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3254">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="9fd5f-3255">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3255">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="9fd5f-3256">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3256">Lab</span></span>

* <span data-ttu-id="9fd5f-3257">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3257">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="9fd5f-3258">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3258">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="9fd5f-3259">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3259">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="9fd5f-3260">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3260">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="9fd5f-3261">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3261">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="9fd5f-3262">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3262">Monitor</span></span>

* <span data-ttu-id="9fd5f-3263">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3263">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="9fd5f-3264">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3264">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="9fd5f-3265">Red</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3265">Network</span></span>

* <span data-ttu-id="9fd5f-3266">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3266">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="9fd5f-3267">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3267">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="9fd5f-3268">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3268">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="9fd5f-3269">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3269">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="9fd5f-3270">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3270">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="9fd5f-3271">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3271">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="9fd5f-3272">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3272">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="9fd5f-3273">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3273">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="9fd5f-3274">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3274">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="9fd5f-3275">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3275">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="9fd5f-3276">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3276">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="9fd5f-3277">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3277">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="9fd5f-3278">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3278">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="9fd5f-3279">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3279">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="9fd5f-3280">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3280">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="9fd5f-3281">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3281">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="9fd5f-3282">Perfil</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3282">Profile</span></span>

* <span data-ttu-id="9fd5f-3283">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3283">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="9fd5f-3284">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3284">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="9fd5f-3285">Redis</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3285">Redis</span></span>

* <span data-ttu-id="9fd5f-3286">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3286">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="9fd5f-3287">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3287">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="9fd5f-3288">Resource</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3288">Resource</span></span>

* <span data-ttu-id="9fd5f-3289">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3289">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="9fd5f-3290">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3290">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="9fd5f-3291">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3291">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="9fd5f-3292">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3292">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="9fd5f-3293">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3293">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="9fd5f-3294">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3294">Add docs for az lock update.</span></span> <span data-ttu-id="9fd5f-3295">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3295">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="9fd5f-3296">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3296">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="9fd5f-3297">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3297">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="9fd5f-3298">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3298">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="9fd5f-3299">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3299">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="9fd5f-3300">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3300">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="9fd5f-3301">Role</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3301">Role</span></span>

* <span data-ttu-id="9fd5f-3302">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3302">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="9fd5f-3303">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3303">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="9fd5f-3304">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3304">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="9fd5f-3305">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3305">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="9fd5f-3306">SQL</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3306">SQL</span></span>

* <span data-ttu-id="9fd5f-3307">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3307">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="9fd5f-3308">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3308">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="9fd5f-3309">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3309">Storage</span></span>

* <span data-ttu-id="9fd5f-3310">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3310">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="9fd5f-3311">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3311">Add support for incremental blob copy</span></span>
* <span data-ttu-id="9fd5f-3312">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3312">Add support for large block blob upload</span></span>
* <span data-ttu-id="9fd5f-3313">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3313">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-3314">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3314">VM</span></span>

* <span data-ttu-id="9fd5f-3315">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3315">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="9fd5f-3316">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3316">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="9fd5f-3317">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3317">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="9fd5f-3318">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3318">az vm/vmss disk</span></span>
  3. <span data-ttu-id="9fd5f-3319">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3319">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="9fd5f-3320">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3320">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="9fd5f-3321">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3321">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="9fd5f-3322">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3322">April 3, 2017</span></span>

<span data-ttu-id="9fd5f-3323">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3323">Version 2.0.2</span></span>

<span data-ttu-id="9fd5f-3324">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3324">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="9fd5f-3325">Core</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3325">Core</span></span>

* <span data-ttu-id="9fd5f-3326">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3326">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="9fd5f-3327">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3327">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="9fd5f-3328">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3328">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="9fd5f-3329">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3329">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9fd5f-3330">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3330">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="9fd5f-3331">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3331">Add prompting for missing template parameters.</span></span> <span data-ttu-id="9fd5f-3332">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3332">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="9fd5f-3333">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3333">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="9fd5f-3334">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3334">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="9fd5f-3335">ACS</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3335">ACS</span></span>

* <span data-ttu-id="9fd5f-3336">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3336">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="9fd5f-3337">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3337">Add support for ssh key password prompting.</span></span> <span data-ttu-id="9fd5f-3338">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3338">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="9fd5f-3339">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3339">Add support for windows clusters.</span></span> <span data-ttu-id="9fd5f-3340">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3340">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="9fd5f-3341">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3341">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="9fd5f-3342">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3342">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="9fd5f-3343">AppService</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3343">AppService</span></span>

* <span data-ttu-id="9fd5f-3344">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3344">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="9fd5f-3345">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3345">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="9fd5f-3346">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3346">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="9fd5f-3347">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3347">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="9fd5f-3348">DataLake</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3348">DataLake</span></span>

* <span data-ttu-id="9fd5f-3349">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3349">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="9fd5f-3350">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3350">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="9fd5f-3351">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3351">DocuemntDB</span></span>

* <span data-ttu-id="9fd5f-3352">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3352">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="9fd5f-3353">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3353">VM</span></span>

* <span data-ttu-id="9fd5f-3354">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3354">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="9fd5f-3355">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3355">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="9fd5f-3356">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3356">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="9fd5f-3357">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3357">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9fd5f-3358">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3358">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="9fd5f-3359">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3359">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="9fd5f-3360">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3360">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="9fd5f-3361">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3361">February 27, 2017</span></span>

<span data-ttu-id="9fd5f-3362">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3362">Version 2.0.0</span></span>

<span data-ttu-id="9fd5f-3363">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3363">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="9fd5f-3364">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3364">Container Service (acs)</span></span>
- <span data-ttu-id="9fd5f-3365">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3365">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="9fd5f-3366">Redes</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3366">Networking</span></span>
- <span data-ttu-id="9fd5f-3367">Storage</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3367">Storage</span></span>

<span data-ttu-id="9fd5f-3368">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3368">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="9fd5f-3369">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3369">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="9fd5f-3370">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3370">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="9fd5f-3371">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3371">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="9fd5f-3372">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3372">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="9fd5f-3373">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3373">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="9fd5f-3374">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3374">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="9fd5f-3375">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3375">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="9fd5f-3376">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="9fd5f-3376">Provide feedback from the command line with the `az feedback` command</span></span>

