---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/04/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: eafd18344ac4c1c0124ff53864a45510070b6fe7
ms.sourcegitcommit: d0b2763cc856eef44a6ecb78f6b8c64291625750
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/04/2020
ms.locfileid: "77013291"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="9efde-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="9efde-103">Azure CLI release notes</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="9efde-104">4 de febrero de 2020</span><span class="sxs-lookup"><span data-stu-id="9efde-104">February 04, 2020</span></span>

<span data-ttu-id="9efde-105">Versión 2.0.81</span><span class="sxs-lookup"><span data-stu-id="9efde-105">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-106">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-106">ACS</span></span>

* <span data-ttu-id="9efde-107">Se ha agregado compatibilidad para establecer los puertos asignados de salida y los tiempos de espera de inactividad en el equilibrador de carga estándar.</span><span class="sxs-lookup"><span data-stu-id="9efde-107">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="9efde-108">Actualización a la versión de API 2019-11-01</span><span class="sxs-lookup"><span data-stu-id="9efde-108">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-109">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-109">ACR</span></span>

* <span data-ttu-id="9efde-110">[CAMBIO IMPORTANTE]  `az acr delete` mostrará un aviso.</span><span class="sxs-lookup"><span data-stu-id="9efde-110">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="9efde-111">[CAMBIO IMPORTANTE] "az acr task delete" mostrará un aviso.</span><span class="sxs-lookup"><span data-stu-id="9efde-111">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="9efde-112">Se ha agregado un nuevo grupo de comandos "az acr taskrun show/list/delete" para la administración de la ejecución de tareas.</span><span class="sxs-lookup"><span data-stu-id="9efde-112">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-113">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-113">AKS</span></span>

* <span data-ttu-id="9efde-114">Cada clúster obtiene una entidad de servicio independiente para mejorar el aislamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-114">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="9efde-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9efde-115">AppConfig</span></span>

* <span data-ttu-id="9efde-116">Se ha agregado compatibilidad con la importación y exportación de referencias al almacén de claves hacia y desde appservice.</span><span class="sxs-lookup"><span data-stu-id="9efde-116">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="9efde-117">Se ha agregado compatibilidad con la importación y exportación de todas las etiquetas de appconfig a appconfig.</span><span class="sxs-lookup"><span data-stu-id="9efde-117">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="9efde-118">Ahora se validan los nombres de clave y de característica antes de establecerlos e importarlos.</span><span class="sxs-lookup"><span data-stu-id="9efde-118">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="9efde-119">Se ha expuesto la modificación de la SKU para el almacén de configuración.</span><span class="sxs-lookup"><span data-stu-id="9efde-119">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="9efde-120">Se ha agregado el grupo de comandos para identidades administradas.</span><span class="sxs-lookup"><span data-stu-id="9efde-120">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-121">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-121">AppService</span></span>

* <span data-ttu-id="9efde-122">Azure Stack: exposición de los comandos del perfil 2019-03-01-hybrid.</span><span class="sxs-lookup"><span data-stu-id="9efde-122">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="9efde-123">functionapp: se ha incorporado la capacidad de crear aplicaciones de función de Java en Linux.</span><span class="sxs-lookup"><span data-stu-id="9efde-123">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-124">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-124">ARM</span></span>

* <span data-ttu-id="9efde-125">Corrección del problema 10246: `az resource tag` se bloquea cuando el parámetro `--ids` pasado es un identificador de grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-125">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="9efde-126">Corrección del problema 11658: el comando `az group export` no admite los parámetros `--query` y `--output`.</span><span class="sxs-lookup"><span data-stu-id="9efde-126">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="9efde-127">Corrección del problema 10279: el código de salida de `az group deployment validate` es 0 cuando se produce un error en la comprobación.</span><span class="sxs-lookup"><span data-stu-id="9efde-127">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="9efde-128">Corrección del problema 9916: se ha mejorado el mensaje de error del conflicto entre la etiqueta y otras condiciones de filtro del comando `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="9efde-128">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="9efde-129">Se ha agregado un nuevo parámetro `--managed-by` para admitir la adición de información de managedBy para el comando `az group create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-129">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="9efde-130">Red Hat OpenShift en Azure</span><span class="sxs-lookup"><span data-stu-id="9efde-130">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="9efde-131">Se ha agregado el subgrupo `monitor` para administrar la supervisión de Log Analytics en el clúster de Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="9efde-131">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-132">BotService</span><span class="sxs-lookup"><span data-stu-id="9efde-132">BotService</span></span>

* <span data-ttu-id="9efde-133">Corrección del problema 11697: `az bot create` no es idempotente.</span><span class="sxs-lookup"><span data-stu-id="9efde-133">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="9efde-134">Se han cambiado las pruebas de corrección del nombre para que se ejecuten solo en modo activo.</span><span class="sxs-lookup"><span data-stu-id="9efde-134">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-135">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-135">CDN</span></span>

* <span data-ttu-id="9efde-136">Se ha incorporado compatibilidad con la característica rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="9efde-136">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="9efde-137">Se ha agregado un nuevo grupo de comandos "cdn endpoint rule" para administrar reglas.</span><span class="sxs-lookup"><span data-stu-id="9efde-137">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="9efde-138">Se ha actualizado la versión de azure-mgmt-cdn a la 4.0.0 para usar la versión de API 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="9efde-138">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="9efde-139">Administrador de implementaciones</span><span class="sxs-lookup"><span data-stu-id="9efde-139">Deployment Manager</span></span>

* <span data-ttu-id="9efde-140">Se ha agregado la operación de lista para todos los recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-140">Add list operation for all resources.</span></span>
* <span data-ttu-id="9efde-141">Se ha mejorado el recurso de paso para el nuevo tipo de paso.</span><span class="sxs-lookup"><span data-stu-id="9efde-141">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="9efde-142">Se ha actualizado el paquete azure-mgmt-deploymentmanager para usar la versión 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-142">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-143">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-143">IoT</span></span>

* <span data-ttu-id="9efde-144">Los comandos "IoT hub Job" han quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-144">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="9efde-145">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9efde-145">IoT Central</span></span>

* <span data-ttu-id="9efde-146">Se ha agregado compatibilidad con la creación y actualización de aplicaciones con el nuevo nombre de SKU ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="9efde-146">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-147">Key Vault</span></span>

* <span data-ttu-id="9efde-148">Se ha agregado un nuevo comando `az keyvault key download` para descargar claves.</span><span class="sxs-lookup"><span data-stu-id="9efde-148">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="9efde-149">Varios</span><span class="sxs-lookup"><span data-stu-id="9efde-149">Misc</span></span>

* <span data-ttu-id="9efde-150">Corrección 6371: se ha agregado compatibilidad con la finalización de nombres de archivo y variables de entorno en Bash.</span><span class="sxs-lookup"><span data-stu-id="9efde-150">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="9efde-151">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-151">Network</span></span>

* <span data-ttu-id="9efde-152">Fix #2092: az network dns record-set add/remove. Se ha agregado una advertencia cuando no se encuentra el conjunto de registros.</span><span class="sxs-lookup"><span data-stu-id="9efde-152">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="9efde-153">En el futuro, se admitirá un argumento adicional para confirmar esta creación automática.</span><span class="sxs-lookup"><span data-stu-id="9efde-153">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="9efde-154">Directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-154">Policy</span></span>

* <span data-ttu-id="9efde-155">Se ha agregado un nuevo comando `az policy metadata` para recuperar recursos de metadatos de directivas enriquecidos.</span><span class="sxs-lookup"><span data-stu-id="9efde-155">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="9efde-156">`az policy remediation create`: especifica si se debe volver a evaluar la compatibilidad antes de la corrección con el parámetro `--resource-discovery-mode`.</span><span class="sxs-lookup"><span data-stu-id="9efde-156">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-157">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-157">Profile</span></span>

* <span data-ttu-id="9efde-158">`az account get-access-token`: se ha agregado el parámetro `--tenant` para adquirir el token para el inquilino directamente, sin necesidad de especificar una suscripción.</span><span class="sxs-lookup"><span data-stu-id="9efde-158">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-159">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-159">RBAC</span></span>

* <span data-ttu-id="9efde-160">[CAMBIO IMPORTANTE] Corrección 11883: `az role assignment create`: si el ámbito está vacío se mostrará un aviso.</span><span class="sxs-lookup"><span data-stu-id="9efde-160">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="9efde-161">Seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-161">Security</span></span>

* <span data-ttu-id="9efde-162">Se han agregado los nuevos comandos `az atp show` y `az atp update` para ver y administrar la configuración de protección contra amenazas avanzada para las cuentas de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-162">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-163">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-163">SQL</span></span>

* <span data-ttu-id="9efde-164">`sql dw create`: los parámetros `--zone-redundant` y `--read-replica-count` han quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-164">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="9efde-165">Estos parámetros no se aplican a DataWarehouse.</span><span class="sxs-lookup"><span data-stu-id="9efde-165">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="9efde-166">[CAMBIO IMPORTANTE] `az sql db create`: Se han quitado "WideWorldImportersStd" y "WideWorldImportersFull" como valores permitidos documentados de "az sql db create --sample-name".</span><span class="sxs-lookup"><span data-stu-id="9efde-166">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="9efde-167">Estas bases de datos de ejemplo siempre provocarán un error en la creación.</span><span class="sxs-lookup"><span data-stu-id="9efde-167">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="9efde-168">Se han agregado los nuevos comandos `sql db classification show/list/update/delete` y `sql db classification recommendation list/enable/disable` para administrar las clasificaciones de confidencialidad de las bases de datos SQL.</span><span class="sxs-lookup"><span data-stu-id="9efde-168">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="9efde-169">`az sql db audit-policy`: corrección para acciones y grupos de auditoría vacíos.</span><span class="sxs-lookup"><span data-stu-id="9efde-169">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-170">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-170">Storage</span></span>

* <span data-ttu-id="9efde-171">Se ha agregado un nuevo grupo de comandos `az storage share-rm` para usar el proveedor de recursos Microsoft.Storage para las operaciones de administración de recursos compartidos de archivos de Azure.</span><span class="sxs-lookup"><span data-stu-id="9efde-171">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="9efde-172">Corrección del problema 11415: error de permisos para `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-172">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="9efde-173">Se ha integrado Azcopy 10.3.3 y se ha agregado compatibilidad con Win32.</span><span class="sxs-lookup"><span data-stu-id="9efde-173">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="9efde-174">`az storage copy`: se han agregado los parámetros `--include-path`, `--include-pattern`, `--exclude-path` y `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="9efde-174">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="9efde-175">`az storage remove`: se han cambiado los parámetros `--inlcude` y `--exclude` por los parámetros `--include-path`, `--include-pattern`, `--exclude-path` y `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="9efde-175">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="9efde-176">`az storage sync`: se han agregado los parámetros `--include-pattern`, `--exclude-path` y `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="9efde-176">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9efde-177">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9efde-177">ServiceFabric</span></span>

* <span data-ttu-id="9efde-178">Se han agregado nuevos comandos para administrar aplicaciones y servicios.</span><span class="sxs-lookup"><span data-stu-id="9efde-178">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="9efde-179">13 de enero de 2020</span><span class="sxs-lookup"><span data-stu-id="9efde-179">January 13, 2020</span></span>

<span data-ttu-id="9efde-180">Versión 2.0.80</span><span class="sxs-lookup"><span data-stu-id="9efde-180">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-181">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-181">Compute</span></span>

* <span data-ttu-id="9efde-182">disk update: Se han agregado --disk-encryption-set y --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="9efde-182">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="9efde-183">snapshot create/update: Se han agregado --disk-encryption-set y --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="9efde-183">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-184">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-184">Storage</span></span>

* <span data-ttu-id="9efde-185">Se ha actualizado la versión de azure-mgmt-storage a la 7.1.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-185">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="9efde-186">`az storage account create`: Se han agregado `--encryption-key-type-for-table` y `--encryption-key-type-for-queue` para admitir el servicio de cifrado de tablas y colas.</span><span class="sxs-lookup"><span data-stu-id="9efde-186">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="9efde-187">7 de enero de 2020</span><span class="sxs-lookup"><span data-stu-id="9efde-187">January 07, 2020</span></span>

<span data-ttu-id="9efde-188">Versión 2.0.79</span><span class="sxs-lookup"><span data-stu-id="9efde-188">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-189">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-189">ACR</span></span>

* <span data-ttu-id="9efde-190">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro "--os" para "acr build", "acr task create/update", "acr run" y "acr pack".</span><span class="sxs-lookup"><span data-stu-id="9efde-190">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="9efde-191">En su lugar, utilice "--platform".</span><span class="sxs-lookup"><span data-stu-id="9efde-191">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="9efde-192">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9efde-192">AppConfig</span></span>

* <span data-ttu-id="9efde-193">Se ha agregado compatibilidad para la importación y exportación de marcas de características.</span><span class="sxs-lookup"><span data-stu-id="9efde-193">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="9efde-194">Se ha agregado el nuevo comando "az appconfig kv set-keyvault" para crear la referencia de Key Vault.</span><span class="sxs-lookup"><span data-stu-id="9efde-194">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="9efde-195">Compatibilidad con diversas convenciones de nomenclatura al exportar marcas de características a un archivo.</span><span class="sxs-lookup"><span data-stu-id="9efde-195">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-196">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-196">AppService</span></span>

* <span data-ttu-id="9efde-197">Se ha corregido el problema 7154: actualización de la documentación del comando <> para usar acentos invertidos en lugar de comillas simples.</span><span class="sxs-lookup"><span data-stu-id="9efde-197">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="9efde-198">Se ha corregido el problema 11287: webapp up: de forma predeterminada, la aplicación creada con up "debe estar habilitada para SSL".</span><span class="sxs-lookup"><span data-stu-id="9efde-198">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="9efde-199">Se ha corregido el problema 11592: se ha agregado la marca az webapp up para sitios HTML estáticos.</span><span class="sxs-lookup"><span data-stu-id="9efde-199">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-200">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-200">ARM</span></span>

* <span data-ttu-id="9efde-201">Se ha corregido `az resource tag`: no se pueden actualizar las etiquetas del almacén de Recovery Services.</span><span class="sxs-lookup"><span data-stu-id="9efde-201">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-202">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-202">Backup</span></span>

* <span data-ttu-id="9efde-203">Se ha agregado un nuevo comando "backup protection undelete" para habilitar la característica de eliminación temporal para la carga de trabajo de IaasVM.</span><span class="sxs-lookup"><span data-stu-id="9efde-203">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="9efde-204">Se ha agregado el nuevo parámetro "--soft-delete-feature-state" al comando set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="9efde-204">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="9efde-205">Se ha agregado compatibilidad con la exclusión de disco para la carga de trabajo de IaasVM.</span><span class="sxs-lookup"><span data-stu-id="9efde-205">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-206">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-206">Compute</span></span>

* <span data-ttu-id="9efde-207">Se ha corregido el error de `vm create` en el perfil de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9efde-207">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="9efde-208">vm monitor metrics tail/list-definitions: compatibilidad con métricas de consultas y definiciones de lista para una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9efde-208">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="9efde-209">Se ha agregado la nueva acción del comando reapply para az vm.</span><span class="sxs-lookup"><span data-stu-id="9efde-209">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-210">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-210">HDInsight</span></span>

* <span data-ttu-id="9efde-211">Compatibilidad con la creación de un clúster de Kafka con Kafka Rest Proxy.</span><span class="sxs-lookup"><span data-stu-id="9efde-211">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="9efde-212">Se ha actualizado azure-mgmt-hdinsight a la versión 1.3.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-212">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="9efde-213">Varios:</span><span class="sxs-lookup"><span data-stu-id="9efde-213">Misc.</span></span>

* <span data-ttu-id="9efde-214">Se ha agregado el comando en versión preliminar `az version show` para mostrar las versiones de los módulos de la CLI de Azure y las extensiones en formato JSON de forma predeterminada o con el formato configurado con --output.</span><span class="sxs-lookup"><span data-stu-id="9efde-214">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="9efde-215">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9efde-215">Event Hubs</span></span>

* <span data-ttu-id="9efde-216">[CAMBIO IMPORTANTE] Se ha eliminado la opción de estado "ReceiveDisabled" de los comandos "az eventhubs eventhub update" y "az eventhubs eventhub create".</span><span class="sxs-lookup"><span data-stu-id="9efde-216">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="9efde-217">Esta opción no es válida para entidades de Event Hubs.</span><span class="sxs-lookup"><span data-stu-id="9efde-217">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="9efde-218">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9efde-218">Service Bus</span></span>

* <span data-ttu-id="9efde-219">[CAMBIO IMPORTANTE] Se ha eliminado la opción de estado "ReceiveDisabled" de los comandos "az servicebus topic create", "az servicebus topic update", "az servicebus queue create" y "az servicebus queue update".</span><span class="sxs-lookup"><span data-stu-id="9efde-219">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="9efde-220">Esta opción no es válida para temas y colas de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="9efde-220">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-221">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-221">RBAC</span></span>

* <span data-ttu-id="9efde-222">Se ha corregido el error 11712: `az ad app/sp show` no devuelve el código de salida 3 cuando la aplicación o la entidad de servicio no existen.</span><span class="sxs-lookup"><span data-stu-id="9efde-222">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-223">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-223">Storage</span></span>

* <span data-ttu-id="9efde-224">`az storage account create`: se ha eliminado la marca en versión preliminar para el parámetro --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="9efde-224">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="9efde-225">Se ha actualizado la versión de azure-mgmt-storage a la 7.0.0 para usar la versión de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="9efde-225">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="9efde-226">Se han agregado los nuevos parámetros `--enable-delete-retention` y `--delete-retention-days` para admitir la administración de la directiva de retención de eliminación para blob-service-properties de la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-226">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="9efde-227">17 de diciembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-227">December 17, 2019</span></span>

<span data-ttu-id="9efde-228">2.0.78</span><span class="sxs-lookup"><span data-stu-id="9efde-228">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-229">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-229">ACR</span></span>

* <span data-ttu-id="9efde-230">Se ha agregado la compatibilidad con el contexto local en acr task run.</span><span class="sxs-lookup"><span data-stu-id="9efde-230">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-231">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-231">ACS</span></span>

* <span data-ttu-id="9efde-232">[CAMBIO IMPORTANTE] az openshift create: se ha cambiado el nombre de `--workspace-resource-id` a `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="9efde-232">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-233">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-233">AMS</span></span>

* <span data-ttu-id="9efde-234">Se han actualizado los comandos show para devolver un código 3 cuando no se encuentra el recurso.</span><span class="sxs-lookup"><span data-stu-id="9efde-234">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="9efde-235">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9efde-235">AppConfig</span></span>

* <span data-ttu-id="9efde-236">Se ha corregido el error al anexar la versión de la API a la dirección URL de la solicitud.</span><span class="sxs-lookup"><span data-stu-id="9efde-236">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="9efde-237">La solución existente no funciona con la paginación.</span><span class="sxs-lookup"><span data-stu-id="9efde-237">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="9efde-238">Se ha agregado compatibilidad para mostrar idiomas además del inglés, ya que el servicio de back-end admite Unicode para la globalización.</span><span class="sxs-lookup"><span data-stu-id="9efde-238">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-239">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-239">AppService</span></span>

* <span data-ttu-id="9efde-240">Se ha corregido el problema 11217: webapp: az webapp config ssl upload debe admitir el parámetro de ranura.</span><span class="sxs-lookup"><span data-stu-id="9efde-240">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="9efde-241">Se ha corregido el problema 10965: Error: El nombre no puede estar vacío.</span><span class="sxs-lookup"><span data-stu-id="9efde-241">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="9efde-242">Se permite la eliminación por ip_address y subnet (dirección IP y subred).</span><span class="sxs-lookup"><span data-stu-id="9efde-242">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="9efde-243">Se ha agregado compatibilidad con la importación de certificados desde `az webapp config ssl import` de Key Vault.</span><span class="sxs-lookup"><span data-stu-id="9efde-243">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-244">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-244">ARM</span></span>

* <span data-ttu-id="9efde-245">Se ha actualizado el paquete azure-mgmt-resource para usar la versión 6.0.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-245">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="9efde-246">Compatibilidad entre inquilinos para el comando `az group deployment create` mediante la adición del nuevo parámetro `--aux-subs`.</span><span class="sxs-lookup"><span data-stu-id="9efde-246">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="9efde-247">Se ha agregado un nuevo parámetro `--metadata` para admitir la adición de información de metadatos para definiciones de conjuntos de directivas.</span><span class="sxs-lookup"><span data-stu-id="9efde-247">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-248">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-248">Backup</span></span>

* <span data-ttu-id="9efde-249">Se ha agregado compatibilidad con la copia de seguridad para cargas de trabajo de SQL y SAP Hana.</span><span class="sxs-lookup"><span data-stu-id="9efde-249">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-250">BotService</span><span class="sxs-lookup"><span data-stu-id="9efde-250">BotService</span></span>

* <span data-ttu-id="9efde-251">[Cambio importante] Se ha eliminado la marca "--version" del comando en versión preliminar "az bot create".</span><span class="sxs-lookup"><span data-stu-id="9efde-251">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="9efde-252">Solo se admiten los bots del SDK V4.</span><span class="sxs-lookup"><span data-stu-id="9efde-252">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="9efde-253">Se ha agregado la comprobación de disponibilidad del nombre para "az bot create".</span><span class="sxs-lookup"><span data-stu-id="9efde-253">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="9efde-254">Se ha agregado compatibilidad para actualizar la dirección URL del icono de un bot mediante "az bot update".</span><span class="sxs-lookup"><span data-stu-id="9efde-254">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="9efde-255">Se ha agregado compatibilidad para actualizar un canal de Direct Line mediante "az bot directline update".</span><span class="sxs-lookup"><span data-stu-id="9efde-255">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="9efde-256">Se ha agregado compatibilidad con la marca "--enable-enhanced-auth" para "az bot directline create".</span><span class="sxs-lookup"><span data-stu-id="9efde-256">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="9efde-257">Los siguientes grupos de comandos están en disponibilidad general y no en versión preliminar: "az bot authsetting".</span><span class="sxs-lookup"><span data-stu-id="9efde-257">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="9efde-258">Los siguientes comandos de "az bot" están en disponibilidad general y no en versión preliminar: "create", "prepare-deploy", "show", "delete", "update".</span><span class="sxs-lookup"><span data-stu-id="9efde-258">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="9efde-259">Se ha corregido el cambio realizado por "az bot prepare-deploy" del valor de "--proj-file-path" a minúsculas (por ejemplo, de "Test.csproj" a "test.csproj").</span><span class="sxs-lookup"><span data-stu-id="9efde-259">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-260">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-260">Compute</span></span>

* <span data-ttu-id="9efde-261">vmss create/update: Se ha agregado --scale-in-policy, que decide qué máquinas virtuales se eligen para su eliminación cuando se reduce el tamaño de un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="9efde-261">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="9efde-262">vm/vmss update: Se ha agregado --priority.</span><span class="sxs-lookup"><span data-stu-id="9efde-262">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="9efde-263">vm/vmss update: Se ha agregado --max-price.</span><span class="sxs-lookup"><span data-stu-id="9efde-263">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="9efde-264">Se ha agregado el grupo de comandos disk-encryption-set (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="9efde-264">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="9efde-265">disk create: Se han agregado --encryption-type y --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="9efde-265">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="9efde-266">vm/vmss create: Se han agregado --os-disk-encryption-set y --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="9efde-266">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="9efde-267">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-267">Core</span></span>

* <span data-ttu-id="9efde-268">Se eliminó la compatibilidad con Python 3.4.</span><span class="sxs-lookup"><span data-stu-id="9efde-268">Removed support for Python 3.4</span></span>
* <span data-ttu-id="9efde-269">Complemento HaTS survey en varios comandos.</span><span class="sxs-lookup"><span data-stu-id="9efde-269">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="9efde-270">DLS</span><span class="sxs-lookup"><span data-stu-id="9efde-270">DLS</span></span>

* <span data-ttu-id="9efde-271">Se ha actualizado la versión del SDK de ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="9efde-271">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="9efde-272">Instalar</span><span class="sxs-lookup"><span data-stu-id="9efde-272">Install</span></span>

* <span data-ttu-id="9efde-273">El script de instalación admite Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="9efde-273">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-274">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-274">IOT</span></span>

* <span data-ttu-id="9efde-275">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro --failover-region de manual-failover.</span><span class="sxs-lookup"><span data-stu-id="9efde-275">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="9efde-276">Ahora se realizará la conmutación por error a la región secundaria emparejada geográficamente asignada.</span><span class="sxs-lookup"><span data-stu-id="9efde-276">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-277">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-277">Key Vault</span></span>

* <span data-ttu-id="9efde-278">Se ha corregido el error 8095: `az keyvault storage remove`: mejora del mensaje de ayuda.</span><span class="sxs-lookup"><span data-stu-id="9efde-278">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="9efde-279">Se ha corregido el error 8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: se ha corregido el error de validación en el parámetro `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="9efde-279">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="9efde-280">Se ha corregido el error 10512: `az keyvault set-policy`: mejora del mensaje de error cuando no se especifican `--object-id`, `--spn` ni `--upn`.</span><span class="sxs-lookup"><span data-stu-id="9efde-280">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="9efde-281">Se ha corregido el error 10846: `az keyvault secret show-deleted`: cuando se especifica `--id`, no se requiere `--name/-n`.</span><span class="sxs-lookup"><span data-stu-id="9efde-281">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="9efde-282">Se ha corregido el error 11084: `az keyvault secret download`: mejora del mensaje de ayuda del parámetro `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="9efde-282">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-283">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-283">Network</span></span>

* <span data-ttu-id="9efde-284">az network application-gateway probe: se ha agregado compatibilidad con la opción -port para especificar un puerto para sondear servidores de back-end en la creación y actualización.</span><span class="sxs-lookup"><span data-stu-id="9efde-284">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="9efde-285">az network application-gateway url-path-map create/update: se ha corregido el error de `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="9efde-285">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="9efde-286">az network application-gateway: se ha agregado compatibilidad con `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="9efde-286">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="9efde-287">az network list-service-aliases: se ha agregado compatibilidad con los alias de servicio de lista, que se pueden usar para las directivas del punto de conexión de servicio.</span><span class="sxs-lookup"><span data-stu-id="9efde-287">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="9efde-288">az network dns zone import: se ha agregado compatibilidad con .@ en el nombre de registro.</span><span class="sxs-lookup"><span data-stu-id="9efde-288">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="9efde-289">Packaging</span><span class="sxs-lookup"><span data-stu-id="9efde-289">Packaging</span></span>

* <span data-ttu-id="9efde-290">Se han agregado compilaciones de perímetro posterior para la instalación de pip.</span><span class="sxs-lookup"><span data-stu-id="9efde-290">Added back edge builds for pip install</span></span>
* <span data-ttu-id="9efde-291">Se ha agregado el paquete eoan de Ubuntu.</span><span class="sxs-lookup"><span data-stu-id="9efde-291">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="9efde-292">Directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-292">Policy</span></span>

* <span data-ttu-id="9efde-293">Se ha agregado compatibilidad con la versión 2019-09-01 de Policy API.</span><span class="sxs-lookup"><span data-stu-id="9efde-293">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="9efde-294">az policy set-definition: se ha agregado compatibilidad con la agrupación dentro de definiciones de conjuntos de directivas con el parámetro `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="9efde-294">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="9efde-295">Redis</span><span class="sxs-lookup"><span data-stu-id="9efde-295">Redis</span></span>

* <span data-ttu-id="9efde-296">Se ha agregado el parámetro en versión preliminar `--replicas-per-master` al comando `az redis create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-296">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="9efde-297">Se ha actualizado azure-mgmt-redis de la versión 6.0.0 a la 7.0.0rc1.</span><span class="sxs-lookup"><span data-stu-id="9efde-297">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9efde-298">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9efde-298">ServiceFabric</span></span>

* <span data-ttu-id="9efde-299">Se ha corregido la lógica de adición de tipo de nodo, incluido el error 10963: la adición de un nuevo tipo de nodo con el nivel de durabilidad Gold siempre producirá un error de la CLI.</span><span class="sxs-lookup"><span data-stu-id="9efde-299">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="9efde-300">La versión de ServiceFabricNodeVmExt se ha actualizado al a 1.1 en la plantilla de creación.</span><span class="sxs-lookup"><span data-stu-id="9efde-300">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-301">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-301">SQL</span></span>

* <span data-ttu-id="9efde-302">Se han agregado los parámetros "--read-scale" y "--read-replicas" a los comandos create y update de SQL DB para admitir la administración de escalado de lectura.</span><span class="sxs-lookup"><span data-stu-id="9efde-302">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-303">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-303">Storage</span></span>

* <span data-ttu-id="9efde-304">Versión de disponibilidad general de la propiedad de recursos compartidos de archivos grandes para el comando de creación y actualización de la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-304">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="9efde-305">Versión de disponibilidad general de la compatibilidad de los token de SAS para la delegación de usuarios.</span><span class="sxs-lookup"><span data-stu-id="9efde-305">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="9efde-306">Se han agregado los nuevos comandos `az storage account blob-service-properties show` y `az storage account blob-service-properties update --enable-change-feed` para administrar las propiedades de Blob Service para la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-306">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="9efde-307">[PRÓXIMO CAMBIO IMPORTANTE] `az storage copy`: ya no se admite el carácter `*` como comodín en la dirección URL, pero se agregarán nuevos parámetros --include-pattern y --exclude-pattern con compatibilidad con caracteres comodín `*`.</span><span class="sxs-lookup"><span data-stu-id="9efde-307">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="9efde-308">Se ha corregido el problema 11043: se ha agregado compatibilidad para eliminar todo el contenedor o el recurso compartido en el comando `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="9efde-308">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="9efde-309">26 de noviembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-309">November 26, 2019</span></span>

<span data-ttu-id="9efde-310">Versión 2.0.77</span><span class="sxs-lookup"><span data-stu-id="9efde-310">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-311">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-311">ACR</span></span>

* <span data-ttu-id="9efde-312">El parámetro `--branch` de acr task create/update ha quedado en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-312">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="9efde-313">Red Hat OpenShift en Azure</span><span class="sxs-lookup"><span data-stu-id="9efde-313">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="9efde-314">Se ha agregado la marca `--workspace-resource-id` para permitir la creación de un clúster de Red Hat OpenShift en Azure con supervisión.</span><span class="sxs-lookup"><span data-stu-id="9efde-314">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="9efde-315">Se ha agregado `monitor_profile` para crear un clúster de Red Hat OpenShift en Azure con supervisión.</span><span class="sxs-lookup"><span data-stu-id="9efde-315">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-316">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-316">AKS</span></span>

* <span data-ttu-id="9efde-317">Se ha agregado compatibilidad con la operación de rotación de certificados del clúster mediante "az aks rotate-certs".</span><span class="sxs-lookup"><span data-stu-id="9efde-317">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="9efde-318">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9efde-318">AppConfig</span></span>

* <span data-ttu-id="9efde-319">Se ha agregado compatibilidad con el uso de ":" como separador de `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="9efde-319">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="9efde-320">Se ha corregido un problema para enumerar los valores de clave con varias etiquetas que incluyen la etiqueta nula.</span><span class="sxs-lookup"><span data-stu-id="9efde-320">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="9efde-321">Se ha actualizado el SDK del plano de administración, azure-mgmt-appconfiguration, a la versión 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-321">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="9efde-322">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-322">AppService</span></span>

* <span data-ttu-id="9efde-323">Se ha corregido el problema 11100: Error de atributo para az webapp up al crear el plan de servicio</span><span class="sxs-lookup"><span data-stu-id="9efde-323">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="9efde-324">az webapp up: cuando se fuerza la creación o implementación en un sitio para lenguajes admitidos, no se usan los valores predeterminados.</span><span class="sxs-lookup"><span data-stu-id="9efde-324">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="9efde-325">Se ha agregado compatibilidad para App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span><span class="sxs-lookup"><span data-stu-id="9efde-325">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-326">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-326">Backup</span></span>

* <span data-ttu-id="9efde-327">Se ha corregido el problema en los elementos asociados a listas de directivas de az backup.</span><span class="sxs-lookup"><span data-stu-id="9efde-327">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="9efde-328">Se ha agregado el parámetro opcional BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="9efde-328">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-329">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-329">Compute</span></span>

* <span data-ttu-id="9efde-330">Se ha actualizado la versión de la API de proceso, discos e instantáneas a la 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9efde-330">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="9efde-331">vmss create: mejoras para --orchestration-mode</span><span class="sxs-lookup"><span data-stu-id="9efde-331">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="9efde-332">sig image-definition create: se ha agregado --os-state para poder especificar si las máquinas virtuales creadas con esta imagen están "Generalizadas" o "Especializadas".</span><span class="sxs-lookup"><span data-stu-id="9efde-332">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="9efde-333">sig image-definition create: se ha agregado --hyper-v-generation para poder especificar la generación del hipervisor.</span><span class="sxs-lookup"><span data-stu-id="9efde-333">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="9efde-334">sig image-version create: se ha agregado compatibilidad con --os-snapshot y --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="9efde-334">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="9efde-335">image create: se ha agregado --data-disk-caching para poder especificar la configuración de almacenamiento en caché de los discos de datos.</span><span class="sxs-lookup"><span data-stu-id="9efde-335">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="9efde-336">Actualización del SDK de Compute para Python a la versión 10.0.0</span><span class="sxs-lookup"><span data-stu-id="9efde-336">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="9efde-337">vm/vmss create: se ha agregado "Spot" a la propiedad de la enumeración "Priority".</span><span class="sxs-lookup"><span data-stu-id="9efde-337">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="9efde-338">[Cambio importante] Se ha cambiado el nombre del parámetro "--max-billing" a "--max-price" para máquinas virtuales y VMSS, para que sean coherentes con los cmdlets de Swagger y Powershell.</span><span class="sxs-lookup"><span data-stu-id="9efde-338">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="9efde-339">vm monitor log show: se ha agregado compatibilidad para la consulta del registro en el área de trabajo de Log Analytics vinculada.</span><span class="sxs-lookup"><span data-stu-id="9efde-339">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-340">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-340">IOT</span></span>

* <span data-ttu-id="9efde-341">Corrección 2531: se han agregado argumentos de utilidad para la actualización del concentrador.</span><span class="sxs-lookup"><span data-stu-id="9efde-341">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="9efde-342">Corrección 8323: se han agregado los parámetros que faltaban para crear el punto de conexión personalizado de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-342">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="9efde-343">Corrección del error de regresión: se han revertido los cambios que invalidan el punto de conexión de almacenamiento predeterminado.</span><span class="sxs-lookup"><span data-stu-id="9efde-343">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-344">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-344">Key Vault</span></span>

* <span data-ttu-id="9efde-345">Corrección 11121: ahora, con `az keyvault certificate list`, al pasar `--include-pending` no se requiere un valor `true` o `false`.</span><span class="sxs-lookup"><span data-stu-id="9efde-345">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="9efde-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="9efde-346">NetAppFiles</span></span>

* <span data-ttu-id="9efde-347">Se ha actualizado azure-mgmt-netapp a la versión 0.7.0, que incluye algunas propiedades de volumen adicionales asociadas a futuras operaciones de replicación.</span><span class="sxs-lookup"><span data-stu-id="9efde-347">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="9efde-348">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-348">Network</span></span>

* <span data-ttu-id="9efde-349">application-gateway waf-config: en desuso</span><span class="sxs-lookup"><span data-stu-id="9efde-349">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="9efde-350">application-gateway waf-policy: se han agregado reglas administradas de subgrupo para administrar conjuntos de reglas administradas y reglas de exclusión.</span><span class="sxs-lookup"><span data-stu-id="9efde-350">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="9efde-351">application-gateway waf-policy: se ha agregado la configuración de directivas de subgrupo para administrar la configuración global de una directiva de WAF.</span><span class="sxs-lookup"><span data-stu-id="9efde-351">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="9efde-352">[Cambio importante] application-gateway waf-policy: se ha cambiado el nombre de la regla de subgrupo a regla personalizada.</span><span class="sxs-lookup"><span data-stu-id="9efde-352">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="9efde-353">application-gateway http-listener: se ha agregado --firewall-policy en la creación.</span><span class="sxs-lookup"><span data-stu-id="9efde-353">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="9efde-354">application-gateway url-path-map rule: se ha agregado --firewall-policy en la creación.</span><span class="sxs-lookup"><span data-stu-id="9efde-354">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="9efde-355">Packaging</span><span class="sxs-lookup"><span data-stu-id="9efde-355">Packaging</span></span>

* <span data-ttu-id="9efde-356">Se ha reescrito az wrapper en Python.</span><span class="sxs-lookup"><span data-stu-id="9efde-356">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="9efde-357">Se ha agregado compatibilidad para Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="9efde-357">Added support for Python 3.8</span></span>
* <span data-ttu-id="9efde-358">Se ha cambiado a Python 3 para el paquete RPM.</span><span class="sxs-lookup"><span data-stu-id="9efde-358">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-359">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-359">Profile</span></span>

* <span data-ttu-id="9efde-360">Se ha corregido el error al ejecutar `az login -u {} -p {}` con una cuenta Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9efde-360">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="9efde-361">Se ha corregido el error `SSLError` al ejecutar `az login` detrás de un servidor proxy con certificado raíz autofirmado.</span><span class="sxs-lookup"><span data-stu-id="9efde-361">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="9efde-362">Corrección 10578: `az login` se bloquea cuando se inicia más de una instancia al mismo tiempo en Windows o WSL.</span><span class="sxs-lookup"><span data-stu-id="9efde-362">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="9efde-363">Corrección 11059: `az login --allow-no-subscriptions` produce un error si hay suscripciones en el inquilino.</span><span class="sxs-lookup"><span data-stu-id="9efde-363">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="9efde-364">Corrección 11238: después de cambiar el nombre de una suscripción, al iniciar sesión con MSI aparecerá dos veces la misma suscripción.</span><span class="sxs-lookup"><span data-stu-id="9efde-364">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-365">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-365">RBAC</span></span>

* <span data-ttu-id="9efde-366">Corrección 10996: corrección del error para `--force-change-password-next-login` en `az ad user update` cuando no se especifica `--password`.</span><span class="sxs-lookup"><span data-stu-id="9efde-366">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="9efde-367">Redis</span><span class="sxs-lookup"><span data-stu-id="9efde-367">Redis</span></span>

* <span data-ttu-id="9efde-368">Corrección 2902: se impedía establecer configuraciones de memoria al actualizar la memoria caché de la SKU Básica.</span><span class="sxs-lookup"><span data-stu-id="9efde-368">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="9efde-369">Reservations</span><span class="sxs-lookup"><span data-stu-id="9efde-369">Reservations</span></span>

* <span data-ttu-id="9efde-370">Actualización de la versión del SDK a la 0.6.0</span><span class="sxs-lookup"><span data-stu-id="9efde-370">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="9efde-371">Se ha agregado información de detalles del plan de facturación después de llamar a Get-Gatalogs.</span><span class="sxs-lookup"><span data-stu-id="9efde-371">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="9efde-372">Se ha agregado el nuevo comando `az reservations reservation-order calculate` para calcular el precio de una reserva.</span><span class="sxs-lookup"><span data-stu-id="9efde-372">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="9efde-373">Se ha agregado el nuevo comando `az reservations reservation-order purchase` para adquirir una nueva reserva.</span><span class="sxs-lookup"><span data-stu-id="9efde-373">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="9efde-374">Rest</span><span class="sxs-lookup"><span data-stu-id="9efde-374">Rest</span></span>
* <span data-ttu-id="9efde-375">Se ha cambiado `az rest` a Disponibilidad general.</span><span class="sxs-lookup"><span data-stu-id="9efde-375">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-376">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-376">SQL</span></span>

* <span data-ttu-id="9efde-377">Se ha actualizado azure-mgmt-sql a la versión 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-377">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-378">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-378">Storage</span></span>

* <span data-ttu-id="9efde-379">storage account create: se ha agregado --enable-hierarchical-namespace para admitir la semántica del sistema de archivos en Blob Service.</span><span class="sxs-lookup"><span data-stu-id="9efde-379">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="9efde-380">Se ha eliminado la excepción no relacionada del mensaje de error.</span><span class="sxs-lookup"><span data-stu-id="9efde-380">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="9efde-381">Se han corregido problemas con el mensaje de error incorrecto: "No tiene los permisos necesarios para realizar esta operación"</span><span class="sxs-lookup"><span data-stu-id="9efde-381">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="9efde-382">en bloqueos de las reglas de red o en un error de autenticación.</span><span class="sxs-lookup"><span data-stu-id="9efde-382">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="9efde-383">4 de noviembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-383">November 4, 2019</span></span>

<span data-ttu-id="9efde-384">Versión 2.0.76</span><span class="sxs-lookup"><span data-stu-id="9efde-384">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-385">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-385">ACR</span></span>

* <span data-ttu-id="9efde-386">Se ha agregado un parámetro en versión preliminar `--pack-image-tag` al comando `az acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="9efde-386">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="9efde-387">Se ha agregado compatibilidad para habilitar la auditoría al crear un registro.</span><span class="sxs-lookup"><span data-stu-id="9efde-387">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="9efde-388">Se admite RBAC en el ámbito del repositorio.</span><span class="sxs-lookup"><span data-stu-id="9efde-388">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-389">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-389">AKS</span></span>

* <span data-ttu-id="9efde-390">Se han agregado `--enable-cluster-autoscaler`, `--min-count` y `--max-count` al comando `az aks create`, que habilita el escalador automático de clústeres para el grupo de nodos.</span><span class="sxs-lookup"><span data-stu-id="9efde-390">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="9efde-391">Se han agregado las marcas anteriores, así como `--update-cluster-autoscaler` y `--disable-cluster-autoscaler`, al comando `az aks update`, lo que permite actualizar el escalador automático de clústeres.</span><span class="sxs-lookup"><span data-stu-id="9efde-391">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="9efde-392">AppConfig</span><span class="sxs-lookup"><span data-stu-id="9efde-392">AppConfig</span></span>

* <span data-ttu-id="9efde-393">Se ha agregado el grupo de comandos de características appConfig para administrar las marcas de características almacenadas en una configuración de aplicación.</span><span class="sxs-lookup"><span data-stu-id="9efde-393">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="9efde-394">Se ha corregido un error secundario menor del comando de appconfig de exportación de almacén de claves a archivo.</span><span class="sxs-lookup"><span data-stu-id="9efde-394">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="9efde-395">Se deja de leer el contenido del archivo de destino durante la exportación.</span><span class="sxs-lookup"><span data-stu-id="9efde-395">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-396">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-396">AppService</span></span>

* <span data-ttu-id="9efde-397">`az appservice plan create`: Se ha agregado compatibilidad para establecer "persitescaling" en plan create de appservice.</span><span class="sxs-lookup"><span data-stu-id="9efde-397">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="9efde-398">Se ha corregido un problema por el que la operación de enlace de SSL de configuración de aplicación web quitaba las etiquetas existentes del recurso.</span><span class="sxs-lookup"><span data-stu-id="9efde-398">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="9efde-399">Se ha agregado la marca `--build-remote` a `az functionapp deployment source config-zip` para admitir la acción de compilación remota durante la implementación de la aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="9efde-399">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="9efde-400">Se ha cambiado la versión predeterminada del nodo en las aplicaciones de función a ~10 para Windows.</span><span class="sxs-lookup"><span data-stu-id="9efde-400">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="9efde-401">Se ha agregado la propiedad `--runtime-version` a `az functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-401">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-402">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-402">ARM</span></span>

* <span data-ttu-id="9efde-403">`az deployment/group deployment validate`: Se ha agregado el parámetro `--handle-extended-json-format` para admitir varias líneas y comentarios en la plantilla JSON durante la implementación.</span><span class="sxs-lookup"><span data-stu-id="9efde-403">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="9efde-404">Se ha incrementado la versión de azure-mgmt-resource a 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9efde-404">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-405">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-405">Backup</span></span>

* <span data-ttu-id="9efde-406">Se ha agregado compatibilidad con la copia de seguridad de AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="9efde-406">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-407">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-407">Compute</span></span>

* <span data-ttu-id="9efde-408">`az vm create`: Se ha agregado una advertencia al especificar juntas redes aceleradas y una NIC existente.</span><span class="sxs-lookup"><span data-stu-id="9efde-408">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="9efde-409">`az vm create`: Se ha agregado `--vmss` para especificar un conjunto de escalado de máquinas virtuales existente al que se debe asignar la máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9efde-409">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="9efde-410">`az vm/vmss create`: Se ha agregado una copia local del archivo de alias de imagen para poder tener acceso a él en un entorno de red restringido.</span><span class="sxs-lookup"><span data-stu-id="9efde-410">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="9efde-411">`az vmss create`: Se ha agregado `--orchestration-mode` para especificar cómo se administran las máquinas virtuales mediante el conjunto de escalado.</span><span class="sxs-lookup"><span data-stu-id="9efde-411">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="9efde-412">`az vm/vmss update`: Se ha agregado `--ultra-ssd-enabled` para poder actualizar la configuración de SSD.</span><span class="sxs-lookup"><span data-stu-id="9efde-412">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="9efde-413">[CAMBIO IMPORTANTE] `az vm extension set`: Se ha corregido un error por el que los usuarios no podían establecer una extensión en una máquina virtual con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9efde-413">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="9efde-414">Se han agregado nuevos comandos `az vm image terms accept/cancel/show` para administrar los términos de la imagen de Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9efde-414">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="9efde-415">Se ha actualizado VMAccessForLinux a la versión 1.5.</span><span class="sxs-lookup"><span data-stu-id="9efde-415">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-416">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-416">CosmosDB</span></span>

* <span data-ttu-id="9efde-417">[CAMBIO IMPORTANTE] `az sql container create`: Se ha cambiado el parámetro `--partition-key-path` a obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9efde-417">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="9efde-418">[CAMBIO IMPORTANTE] `az gremlin graph create`: Se ha cambiado el parámetro `--partition-key-path` a obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9efde-418">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="9efde-419">`az sql container create`: Se han agregado `--unique-key-policy` y `--conflict-resolution-policy`</span><span class="sxs-lookup"><span data-stu-id="9efde-419">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="9efde-420">`az sql container create/update`: Se ha actualizado el esquema predeterminado `--idx`.</span><span class="sxs-lookup"><span data-stu-id="9efde-420">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="9efde-421">`gremlin graph create`: Se agregó `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="9efde-421">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="9efde-422">`gremlin graph create/update`: Se ha actualizado el esquema predeterminado `--idx`.</span><span class="sxs-lookup"><span data-stu-id="9efde-422">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="9efde-423">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="9efde-423">Fixed typo in help message</span></span>
* <span data-ttu-id="9efde-424">base de datos: Se ha agregado la información de desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-424">database: Added deprecation infomation</span></span>
* <span data-ttu-id="9efde-425">colección: Se ha agregado la información de desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-425">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-426">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-426">IoT</span></span>

* <span data-ttu-id="9efde-427">Se ha agregado un nuevo tipo de origen de enrutamiento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="9efde-427">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="9efde-428">Se han corregido las características que faltan en `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-428">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-429">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-429">Key Vault</span></span>

* <span data-ttu-id="9efde-430">Se ha corregido un error inesperado cuando el archivo de certificado no existe.</span><span class="sxs-lookup"><span data-stu-id="9efde-430">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="9efde-431">Se ha corregido `az keyvault recover/purge` porque no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9efde-431">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="9efde-432">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="9efde-432">NetAppFiles</span></span>

* <span data-ttu-id="9efde-433">Se ha actualizado azure-mgmt-netapp a 0.6.0 para usar la API versión 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9efde-433">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="9efde-434">Esta nueva versión de API incluye:</span><span class="sxs-lookup"><span data-stu-id="9efde-434">This new API version includes:</span></span>

    - <span data-ttu-id="9efde-435">La creación del volumen `--protocol-types` ahora acepta "NFSv4.1", no "NFSv4".</span><span class="sxs-lookup"><span data-stu-id="9efde-435">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="9efde-436">La propiedad de directiva de exportación de volumen ahora tiene el nombre "nfsv41", no "nfsv4".</span><span class="sxs-lookup"><span data-stu-id="9efde-436">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="9efde-437">Se ha cambiado el nombre del volumen `--creation-token` a `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="9efde-437">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="9efde-438">La fecha de creación de la instantánea ahora se llamada simplemente "created".</span><span class="sxs-lookup"><span data-stu-id="9efde-438">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="9efde-439">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-439">Network</span></span>

* <span data-ttu-id="9efde-440">`az network private-dns link vnet create/update`: Se ha agregado compatibilidad con la vinculación de redes virtuales entre inquilinos.</span><span class="sxs-lookup"><span data-stu-id="9efde-440">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="9efde-441">[CAMBIO IMPORTANTE] `az network vnet subnet list`: Se han cambiado `--resource-group` y `--vnet-name` para que ahora sean obligatorios.</span><span class="sxs-lookup"><span data-stu-id="9efde-441">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="9efde-442">`az network public-ip prefix create`: se ha agregado compatibilidad para especificar la versión de la dirección IP (IPv4, IPv6) durante la creación.</span><span class="sxs-lookup"><span data-stu-id="9efde-442">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="9efde-443">Se ha aumentado la versión de Azure-MGMT-Network a 7.0.0 y la versión de API a 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="9efde-443">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="9efde-444">`az network vrouter`: se ha agregado compatibilidad con un nuevo enrutador virtual de servicio y el emparejamiento de enrutador virtual.</span><span class="sxs-lookup"><span data-stu-id="9efde-444">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="9efde-445">`az network express-route gateway connection`: Se ha agregado compatibilidad con `--internet-security`</span><span class="sxs-lookup"><span data-stu-id="9efde-445">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-446">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-446">Profile</span></span>

* <span data-ttu-id="9efde-447">Se ha corregido `az account get-access-token --resource-type ms-graph` porque no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9efde-447">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="9efde-448">Se ha quitado la advertencia de `az login`.</span><span class="sxs-lookup"><span data-stu-id="9efde-448">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-449">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-449">RBAC</span></span>

* <span data-ttu-id="9efde-450">Se ha corregido `az ad app update --id {} --display-name {}` porque no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9efde-450">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9efde-451">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9efde-451">ServiceFabric</span></span>

* <span data-ttu-id="9efde-452">`az sf cluster create`: Se ha corregido un problema mediante la modificación de VMSS de proceso template.json Windows y Linux de Service Fabric de discos estándar a discos administrados.</span><span class="sxs-lookup"><span data-stu-id="9efde-452">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-453">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-453">SQL</span></span>

* <span data-ttu-id="9efde-454">Se han agregado los parámetros `--compute-model`, `--auto-pause-delay`y `--min-capacity` para admitir las operaciones CRUD para la nueva oferta de SQL Database: Modelo de proceso sin servidor.</span><span class="sxs-lookup"><span data-stu-id="9efde-454">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-455">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-455">Storage</span></span>

* <span data-ttu-id="9efde-456">`az storage account create/update`: Se ha agregado el parámetro --enable-files-adds y el grupo de argumentos de propiedades de Azure Active Directory para admitir la autenticación de AD DS en Azure Files.</span><span class="sxs-lookup"><span data-stu-id="9efde-456">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="9efde-457">Se ha expandido `az storage account keys list/renew` para admitir la enumeración o regeneración de claves Kerberos de la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-457">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="9efde-458">15 de octubre de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-458">October 15, 2019</span></span>

<span data-ttu-id="9efde-459">Versión 2.0.75</span><span class="sxs-lookup"><span data-stu-id="9efde-459">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-460">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-460">AKS</span></span>

* <span data-ttu-id="9efde-461">Se ha cambiado el valor predeterminado de `--load-balancer-sku` a `standard` si es compatible con la versión de Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9efde-461">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="9efde-462">Se ha cambiado el valor predeterminado de `--vm-set-type` a `virtualmachinescalesets` si es compatible con la versión de Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="9efde-462">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-463">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-463">AMS</span></span>

* <span data-ttu-id="9efde-464">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `job start` a `job create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-464">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="9efde-465">[CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--ask` de `content-key-policy create` para que use una cadena hexadecimal de 32 caracteres en lugar de UTF8.</span><span class="sxs-lookup"><span data-stu-id="9efde-465">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-466">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-466">AppService</span></span>

* <span data-ttu-id="9efde-467">Se han agregado comandos `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="9efde-467">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="9efde-468">Se ha agregado un mejor control de errores a `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9efde-468">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="9efde-469">Se ha agregado compatibilidad para la SKU `Isolated` a `appservice plan update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-469">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-470">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-470">ARM</span></span>

* <span data-ttu-id="9efde-471">Se ha agregado el parámetro `--handle-extended-json-format` a `deployment create` para admitir varias líneas y comentarios en la plantilla JSON.</span><span class="sxs-lookup"><span data-stu-id="9efde-471">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-472">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-472">Compute</span></span>

* <span data-ttu-id="9efde-473">Se ha agregado el parámetro `--enable-agent` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-473">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="9efde-474">Se ha cambiado `vm create` para que use SKU de IP pública estándar automáticamente al usar zonas.</span><span class="sxs-lookup"><span data-stu-id="9efde-474">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="9efde-475">Se ha cambiado `vm create` para que cree automáticamente un nombre de equipo válido para una máquina virtual si no se proporciona ninguno.</span><span class="sxs-lookup"><span data-stu-id="9efde-475">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="9efde-476">Se ha agregado el parámetro `--computer-name-prefix` a `vmss create` para admitir el prefijo de nombre de equipo personalizado de las máquinas virtuales en el VMSS.</span><span class="sxs-lookup"><span data-stu-id="9efde-476">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="9efde-477">Agregue el parámetro `--workspace` a `vm create` para habilitar automáticamente el área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="9efde-477">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="9efde-478">Se ha actualizado la versión de API de galerías a 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="9efde-478">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="9efde-479">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-479">Core</span></span>

* <span data-ttu-id="9efde-480">Se ha agregado la comprobación de la sintaxis del parámetro `--set` en el comando de actualización genérico.</span><span class="sxs-lookup"><span data-stu-id="9efde-480">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-481">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-481">IoT</span></span>

* <span data-ttu-id="9efde-482">Se ha corregido un problema por el que `iot hub show` producía un error con el mensaje "recurso no encontrado".</span><span class="sxs-lookup"><span data-stu-id="9efde-482">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-483">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-483">Monitor</span></span>

* <span data-ttu-id="9efde-484">Se ha agregado compatibilidad para CRUD a `monitor log-analytics workspace`.</span><span class="sxs-lookup"><span data-stu-id="9efde-484">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-485">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-485">Network</span></span>

* <span data-ttu-id="9efde-486">Se ha agregado compatibilidad para la vinculación virtual entre inquilinos a `network private-dns link vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-486">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="9efde-487">[CAMBIO IMPORTANTE] Se ha cambiado `network vnet subnet list` para requerir los parámetros `--resource-group` y `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="9efde-487">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-488">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-488">SQL</span></span>

* <span data-ttu-id="9efde-489">Se han agregado comandos a `sql mi ad-admin` que admiten la configuración de un administrador de AAD en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="9efde-489">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-490">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-490">Storage</span></span>

* <span data-ttu-id="9efde-491">Se ha agregado el parámetro `--preserve-s2s-access-tier` a `storage copy` para conservar el nivel de acceso durante la copia de servicio a servicio.</span><span class="sxs-lookup"><span data-stu-id="9efde-491">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="9efde-492">Se ha agregado el parámetro `--enable-large-file-share` a `storage account [create|update]` para admitir recursos compartidos de archivos grandes para la cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-492">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="9efde-493">24 de septiembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-493">September 24, 2019</span></span>

<span data-ttu-id="9efde-494">Versión 2.0.74</span><span class="sxs-lookup"><span data-stu-id="9efde-494">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-495">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-495">ACR</span></span>

* <span data-ttu-id="9efde-496">Se ha agregado un parámetro `--type` obligatorio a `acr config retention update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-496">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="9efde-497">[CAMBIO IMPORTANTE] Se ha cambiado el nombre del parámetro `--name -n` a `--registry -r ` para el grupo de comandos `acr config`.</span><span class="sxs-lookup"><span data-stu-id="9efde-497">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-498">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-498">AKS</span></span>

* <span data-ttu-id="9efde-499">Se ha agregado el parámetro `--load-balancer-sku` al comando `aks create`, lo que permite crear un clúster de AKS con SLB.</span><span class="sxs-lookup"><span data-stu-id="9efde-499">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="9efde-500">Se han agregado los parámetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` y `--load-balancer-outbound-ip-prefixes` a los comandos `aks [create|update]`, lo que permite actualizar el perfil del equilibrador de carga de un clúster de AKS con SLB.</span><span class="sxs-lookup"><span data-stu-id="9efde-500">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="9efde-501">Se ha agregado el parámetro `--vm-set-type` al comando `aks create`, lo que permite especificar los tipos de máquina virtual de un clúster de AKS (vmas o vmss).</span><span class="sxs-lookup"><span data-stu-id="9efde-501">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-502">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-502">ARM</span></span>

* <span data-ttu-id="9efde-503">Se ha agregado el parámetro `--handle-extended-json-format` al comando `group deployment create` para admitir varias líneas y comentarios en la plantilla JSON.</span><span class="sxs-lookup"><span data-stu-id="9efde-503">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-504">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-504">Compute</span></span>

* <span data-ttu-id="9efde-505">Se ha agregado el parámetro `--terminate-notification-time` a los comandos `vmss [create|update]` para poder finalizar la capacidad de configurar eventos programados.</span><span class="sxs-lookup"><span data-stu-id="9efde-505">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="9efde-506">Se ha agregado el parámetro `--enable-terminate-notification` al comando `vmss update` para poder finalizar la capacidad de configurar eventos programados.</span><span class="sxs-lookup"><span data-stu-id="9efde-506">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="9efde-507">Se han agregado los parámetros `--priority,` `--eviction-policy,` `--max-billing` a los comandos `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-507">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="9efde-508">Se ha cambiado `disk create` para permitir especificar el tamaño exacto de la carga del disco.</span><span class="sxs-lookup"><span data-stu-id="9efde-508">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="9efde-509">Se ha agregado compatibilidad para instantáneas incrementales de discos administrados a `snapshot create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-509">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9efde-510">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9efde-510">Cosmos DB</span></span>

* <span data-ttu-id="9efde-511">Se ha agregado el parámetro `--type <key-type>` al comando `cosmosdb keys list` para mostrar la clave, las claves de solo lectura o las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="9efde-511">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="9efde-512">Se agregó el comando `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="9efde-512">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="9efde-513">[EN DESUSO] Se han dejado de usar los comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` y `cosmosdb list-read-only-keys`.</span><span class="sxs-lookup"><span data-stu-id="9efde-513">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9efde-514">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9efde-514">EventGrid</span></span>

* <span data-ttu-id="9efde-515">Se ha corregido el texto de ayuda del punto de conexión para que haga referencia al parámetro correcto.</span><span class="sxs-lookup"><span data-stu-id="9efde-515">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-516">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-516">Key Vault</span></span>

* <span data-ttu-id="9efde-517">Se ha corregido un problema por el que un inquilino (`login -t`) podía producir un error en `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-517">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-518">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-518">Monitor</span></span>

* <span data-ttu-id="9efde-519">Se ha corregido un problema por el que no se permitía el carácter `:` en el argumento `--condition` de `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-519">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="9efde-520">Directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-520">Policy</span></span>

* <span data-ttu-id="9efde-521">Se ha agregado compatibilidad con la versión 2019-06-01 de Policy API.</span><span class="sxs-lookup"><span data-stu-id="9efde-521">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="9efde-522">Se ha agregado el parámetro `--enforcement-mode` al comando `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-522">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-523">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-523">Storage</span></span>

* <span data-ttu-id="9efde-524">Se ha agregado el parámetro `--blob-type` al comando `az storage copy`.</span><span class="sxs-lookup"><span data-stu-id="9efde-524">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="9efde-525">10 de septiembre de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-525">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-526">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-526">ACR</span></span>

* <span data-ttu-id="9efde-527">Se ha agregado el grupo de comandos `acr config retention` para configurar la directiva de retención.</span><span class="sxs-lookup"><span data-stu-id="9efde-527">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-528">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-528">AKS</span></span>

* <span data-ttu-id="9efde-529">Se ha agregado compatibilidad para la integración de ACR con los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-529">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="9efde-530">Se ha agregado el parámetro `--attach-acr` a `aks [create|update]` para asociar un ACR a un clúster de AKS.</span><span class="sxs-lookup"><span data-stu-id="9efde-530">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="9efde-531">Se ha agregado el parámetro `--detach-acr` a `aks update` para desasociar un ACR de un clúster de AKS.</span><span class="sxs-lookup"><span data-stu-id="9efde-531">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-532">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-532">ARM</span></span>

* <span data-ttu-id="9efde-533">Se ha actualizado para usar la versión 2019-05-10 de la API.</span><span class="sxs-lookup"><span data-stu-id="9efde-533">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-534">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-534">Batch</span></span>

* <span data-ttu-id="9efde-535">Se han agregado nuevas opciones de configuración de JSON a `--json-file` para `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="9efde-535">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="9efde-536">Se ha agregado `MountConfigurations` para montajes del sistema de archivos (consulte https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obtener más información).</span><span class="sxs-lookup"><span data-stu-id="9efde-536">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="9efde-537">Se ha agregado la propiedad `publicIPs` opcional en `NetworkConfiguration` para las direcciones IP públicas en grupos (consulte https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obtener más información).</span><span class="sxs-lookup"><span data-stu-id="9efde-537">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="9efde-538">Se ha agregado compatibilidad para la galería de imágenes compartidas a `--image`.</span><span class="sxs-lookup"><span data-stu-id="9efde-538">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="9efde-539">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--start-task-wait-for-success` en `batch pool create` a `true`.</span><span class="sxs-lookup"><span data-stu-id="9efde-539">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="9efde-540">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `Scope` en `AutoUserSpecification` para que siempre sea Pool (era `Task` en los nodos Windows, `Pool` en los nodos Linux).</span><span class="sxs-lookup"><span data-stu-id="9efde-540">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="9efde-541">Este argumento solo se puede establecer desde una configuración de JSON con `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="9efde-541">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-542">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-542">HDInsight</span></span>

* <span data-ttu-id="9efde-543">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="9efde-543">GA release</span></span>
* <span data-ttu-id="9efde-544">[CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--workernode-count/-c` de `az hdinsight resize` para que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9efde-544">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-545">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-545">Key Vault</span></span>

* <span data-ttu-id="9efde-546">Se ha corregido un problema por el que no se podían eliminar las subredes de las reglas de red.</span><span class="sxs-lookup"><span data-stu-id="9efde-546">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="9efde-547">Se ha corregido un problema por el que se podían agregar subredes y direcciones IP duplicadas a las reglas de red.</span><span class="sxs-lookup"><span data-stu-id="9efde-547">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="9efde-548">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-548">Network</span></span>

* <span data-ttu-id="9efde-549">Se ha agregado el parámetro `--interval` a `network watcher flow-log` para establecer el valor del intervalo de análisis del tráfico.</span><span class="sxs-lookup"><span data-stu-id="9efde-549">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="9efde-550">Se ha agregado `network application-gateway identity` para administrar la identidad de puerta de enlace.</span><span class="sxs-lookup"><span data-stu-id="9efde-550">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="9efde-551">Se ha agregado compatibilidad para establecer el identificador del almacén de claves en `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="9efde-551">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="9efde-552">Se agregó `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-552">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="9efde-553">Directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-553">Policy</span></span>

* <span data-ttu-id="9efde-554">Se ha actualizado para usar la versión 2019-01-01 de la API.</span><span class="sxs-lookup"><span data-stu-id="9efde-554">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="9efde-555">27 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-555">August 27, 2019</span></span>

<span data-ttu-id="9efde-556">Versión 2.0.72</span><span class="sxs-lookup"><span data-stu-id="9efde-556">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-557">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-557">ACR</span></span>

* <span data-ttu-id="9efde-558">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para la SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="9efde-558">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="9efde-559">API Management</span><span class="sxs-lookup"><span data-stu-id="9efde-559">API Management</span></span>

* <span data-ttu-id="9efde-560">[VERSIÓN PRELIMINAR] Se ha agregado el grupo de comandos `apim`</span><span class="sxs-lookup"><span data-stu-id="9efde-560">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-561">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-561">AppService</span></span>

* <span data-ttu-id="9efde-562">Se ha corregido un problema con el comando `webapp webjob continuous start` al especificar una ranura</span><span class="sxs-lookup"><span data-stu-id="9efde-562">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="9efde-563">Se ha cambiado `webapp up` para detectar la carpeta `env` y quitarla del archivo usado para la implementación</span><span class="sxs-lookup"><span data-stu-id="9efde-563">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-564">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9efde-564">Keyvault</span></span>

* <span data-ttu-id="9efde-565">Se ha corregido un error en `keyvault secret set` que hacía que se ignorara el argumento `--expires`</span><span class="sxs-lookup"><span data-stu-id="9efde-565">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="9efde-566">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-566">Network</span></span>

* <span data-ttu-id="9efde-567">Se ha agregado compatibilidad para las direcciones IPv6 con argumentos `--private-ip-address-version`</span><span class="sxs-lookup"><span data-stu-id="9efde-567">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="9efde-568">Se han agregado nuevos comandos `network private-endpoint [create|update|list-types]` para la administración de un punto de conexión privado</span><span class="sxs-lookup"><span data-stu-id="9efde-568">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="9efde-569">Se ha agregado el grupo de comandos `network private-link-service`</span><span class="sxs-lookup"><span data-stu-id="9efde-569">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="9efde-570">Se agregaron los argumentos `--private-endpoint-network-policies` y `--private-link-service-network-policies` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9efde-570">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-571">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-571">RBAC</span></span>

* <span data-ttu-id="9efde-572">Se ha corregido el problema con `ad app update --homepage` por el cual la página principal no se actualizaba</span><span class="sxs-lookup"><span data-stu-id="9efde-572">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9efde-573">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9efde-573">ServiceFabric</span></span>

* <span data-ttu-id="9efde-574">Se ha agregado compatibilidad con los nombres de Key Vault que combinan mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="9efde-574">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="9efde-575">Se ha solucionado el problema que se producía al usar certificados en Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-575">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="9efde-576">Se ha solucionado el problema con el uso de archivos de certificado de PFX</span><span class="sxs-lookup"><span data-stu-id="9efde-576">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="9efde-577">Se ha solucionado el problema con `sf cluster certificate add` que se producía cuando no se especificaba el grupo de recursos de Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-577">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="9efde-578">Se ha corregido el problema con `sf cluster set` que no funcionaba</span><span class="sxs-lookup"><span data-stu-id="9efde-578">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="9efde-579">SignalR</span><span class="sxs-lookup"><span data-stu-id="9efde-579">SignalR</span></span>

* <span data-ttu-id="9efde-580">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-580">Added new commands:</span></span>
  * <span data-ttu-id="9efde-581">`signalr cors`: Administración de SignalR CORS</span><span class="sxs-lookup"><span data-stu-id="9efde-581">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="9efde-582">`signalr restart`: Reinicio de una instancia de SignalR Service</span><span class="sxs-lookup"><span data-stu-id="9efde-582">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="9efde-583">`signalr update`: Actualización de una instancia de SignalR Service</span><span class="sxs-lookup"><span data-stu-id="9efde-583">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="9efde-584">Se agregó el argumento `--service-mode` a `signalr create`</span><span class="sxs-lookup"><span data-stu-id="9efde-584">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-585">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-585">Storage</span></span>

* <span data-ttu-id="9efde-586">Se agregó el comando `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="9efde-586">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="9efde-587">13 de agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-587">August 13, 2019</span></span>

<span data-ttu-id="9efde-588">Versión 2.0.71</span><span class="sxs-lookup"><span data-stu-id="9efde-588">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-589">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-589">AppService</span></span>

* <span data-ttu-id="9efde-590">Se ha corregido un problema por el que se producían errores con los comandos `webapp webjob continuous` en los espacios</span><span class="sxs-lookup"><span data-stu-id="9efde-590">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-591">BotService</span><span class="sxs-lookup"><span data-stu-id="9efde-591">BotService</span></span>

* <span data-ttu-id="9efde-592">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para crear bots con el SDK v3.</span><span class="sxs-lookup"><span data-stu-id="9efde-592">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="9efde-593">CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9efde-593">CognitiveServices</span></span>

* <span data-ttu-id="9efde-594">Se agregaron los comandos `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-594">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9efde-595">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9efde-595">Cosmos DB</span></span>

* <span data-ttu-id="9efde-596">Se ha quitado la advertencia al actualizar varias ubicaciones de escritura.</span><span class="sxs-lookup"><span data-stu-id="9efde-596">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="9efde-597">Se han agregado comandos CRUD para recursos de CosmosDB SQL, MongoDB, Cassandra, Gremlin y Table, así como capacidad de proceso para los recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-597">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-598">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-598">HDInsight</span></span>

<span data-ttu-id="9efde-599">Esta versión contiene un gran número de cambios importantes.</span><span class="sxs-lookup"><span data-stu-id="9efde-599">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="9efde-600">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="9efde-600">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="9efde-601">Cambio de nombre de `--storage-default-container` a `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="9efde-601">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="9efde-602">Cambio de nombre de `--storage-default-filesystem` a `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="9efde-602">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="9efde-603">[CAMBIO IMPORTANTE] Se ha cambiado el argumento `--name` de `application create` para que represente el nombre de la aplicación en lugar del nombre del clúster.</span><span class="sxs-lookup"><span data-stu-id="9efde-603">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="9efde-604">Se ha agregado el argumento `--cluster-name` a `application create` para reemplazar la funcionalidad de `--name` antigua.</span><span class="sxs-lookup"><span data-stu-id="9efde-604">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="9efde-605">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `application create`:</span><span class="sxs-lookup"><span data-stu-id="9efde-605">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="9efde-606">Cambio de nombre de `--application-type` a `--type`</span><span class="sxs-lookup"><span data-stu-id="9efde-606">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="9efde-607">Cambio de nombre de `--marketplace-identifier` a `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="9efde-607">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="9efde-608">Cambio de nombre de `--https-endpoint-access-mode` a `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="9efde-608">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="9efde-609">Se cambió el nombre de `--https-endpoint-destination-port` a `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="9efde-609">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="9efde-610">[CAMBIO IMPORTANTE] Se han quitado los parámetros de `application create`:</span><span class="sxs-lookup"><span data-stu-id="9efde-610">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="9efde-611">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--target-instance-count` a `--workernode-count` para `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="9efde-611">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="9efde-612">[CAMBIO IMPORTANTE] Se han cambiado todos los comandos del grupo `hdinsight script-action` para que usen el parámetro `--name` como nombre de la acción de script.</span><span class="sxs-lookup"><span data-stu-id="9efde-612">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="9efde-613">Se ha agregado el argumento `--cluster-name` a todos los comandos `hdinsight script-action` para reemplazar la funcionalidad de `--name` antigua.</span><span class="sxs-lookup"><span data-stu-id="9efde-613">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="9efde-614">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--script-execution-id` a `--execution-id` para todos los comandos `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="9efde-614">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="9efde-615">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `hdinsight script-action show` a `hdinsight script-action show-execution-details`</span><span class="sxs-lookup"><span data-stu-id="9efde-615">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="9efde-616">[CAMBIO IMPORTANTE] Se han cambiado los parámetros a `hdinsight script-action execute --roles` para que estén separados por espacios en lugar de por comas.</span><span class="sxs-lookup"><span data-stu-id="9efde-616">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="9efde-617">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--persisted` de `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="9efde-617">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="9efde-618">Se ha cambiado el parámetro `hdinsight create --cluster-configurations` para aceptar una ruta a un archivo JSON local o una cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="9efde-618">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="9efde-619">Se ha agregado el comando `hdinsight script-action list-execution-history`</span><span class="sxs-lookup"><span data-stu-id="9efde-619">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="9efde-620">Se ha cambiado `hdinsight monitor enable --workspace` para aceptar un identificador o un nombre de área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="9efde-620">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="9efde-621">Se ha agregado el argumento `hdinsight monitor enable --primary-key`, que es necesario si se proporciona un identificador de área de trabajo como parámetro.</span><span class="sxs-lookup"><span data-stu-id="9efde-621">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="9efde-622">Se han agregado más ejemplos y se han actualizado las descripciones para los mensajes de ayuda.</span><span class="sxs-lookup"><span data-stu-id="9efde-622">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-623">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-623">Interactive</span></span>

* <span data-ttu-id="9efde-624">Se ha corregido un error de carga.</span><span class="sxs-lookup"><span data-stu-id="9efde-624">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="9efde-625">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9efde-625">Kubernetes</span></span>

* <span data-ttu-id="9efde-626">Se ha cambiado para usar `https` si el puerto del contenedor del panel usa `https`.</span><span class="sxs-lookup"><span data-stu-id="9efde-626">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-627">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-627">Network</span></span>

* <span data-ttu-id="9efde-628">Se ha agregado el argumento `network dns record-set cname delete` a `--yes`.</span><span class="sxs-lookup"><span data-stu-id="9efde-628">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-629">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-629">Profile</span></span>

* <span data-ttu-id="9efde-630">Se ha agregado el argumento `--resource-type` a `account get-access-token` para obtener los tokens de acceso a recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-630">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="9efde-631">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9efde-631">ServiceFabric</span></span>

* <span data-ttu-id="9efde-632">Se han agregado todas las versiones del sistema operativo compatible para la creación de clústeres SF.</span><span class="sxs-lookup"><span data-stu-id="9efde-632">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="9efde-633">Se ha corregido el error de validación de certificado principal.</span><span class="sxs-lookup"><span data-stu-id="9efde-633">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-634">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-634">Storage</span></span>

* <span data-ttu-id="9efde-635">Se ha agregado el comando `storage copy`</span><span class="sxs-lookup"><span data-stu-id="9efde-635">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="9efde-636">30 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-636">July 30, 2019</span></span>

<span data-ttu-id="9efde-637">Versión 2.0.70</span><span class="sxs-lookup"><span data-stu-id="9efde-637">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-638">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-638">ACR</span></span>

* <span data-ttu-id="9efde-639">Se ha corregido el problema 9952 (una regresión en el comando `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="9efde-639">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="9efde-640">Se ha quitado el nombre predeterminado de la imagen del generador en `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="9efde-640">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-641">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-641">Appservice</span></span>

* <span data-ttu-id="9efde-642">Se ha cambiado `webapp config ssl` para que muestre un mensaje si no se encuentra un recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-642">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="9efde-643">Se ha corregido un problema por el que `functionapp create` no acepta el tipo de cuenta de almacenamiento `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="9efde-643">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="9efde-644">Se ha corregido un problema por el que `webapp up` producía un error si se ejecutaba con versiones anteriores de Python.</span><span class="sxs-lookup"><span data-stu-id="9efde-644">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="9efde-645">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-645">Network</span></span>

* <span data-ttu-id="9efde-646">Se ha quitado un parámetro no válido `--ids` de `network nic ip-config add` (corrige el problema 9861).</span><span class="sxs-lookup"><span data-stu-id="9efde-646">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="9efde-647">Corrige el problema 9604.</span><span class="sxs-lookup"><span data-stu-id="9efde-647">Fixes #9604.</span></span> <span data-ttu-id="9efde-648">Se ha agregado el parámetro `--root-certs` a `network application-gateway http-settings [create|update]` para admitir los certificados raíz de confianza de los usuarios asociados.</span><span class="sxs-lookup"><span data-stu-id="9efde-648">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="9efde-649">Se ha corregido el argumento `--subscription` para `network dns record-set ns create` (9965).</span><span class="sxs-lookup"><span data-stu-id="9efde-649">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-650">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-650">RBAC</span></span>

* <span data-ttu-id="9efde-651">Se agregó el comando `user update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-651">Added `user update` command</span></span>
* <span data-ttu-id="9efde-652">[EN DESUSO] Se ha dejado de usar `--upn-or-object-id` en los comandos relacionados con el usuario.</span><span class="sxs-lookup"><span data-stu-id="9efde-652">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="9efde-653">Use el nuevo argumento `--id`.</span><span class="sxs-lookup"><span data-stu-id="9efde-653">Use replacement argument `--id`</span></span>
* <span data-ttu-id="9efde-654">Se ha agregado el argumento `--id` a los comandos relacionados con el usuario.</span><span class="sxs-lookup"><span data-stu-id="9efde-654">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-655">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-655">SQL</span></span>

* <span data-ttu-id="9efde-656">Se han agregado comandos de administración para claves de instancia administrada y protector de TDE.</span><span class="sxs-lookup"><span data-stu-id="9efde-656">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-657">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-657">Storage</span></span>

* <span data-ttu-id="9efde-658">Se agregó el comando `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="9efde-658">Added `storage remove` command</span></span>
* <span data-ttu-id="9efde-659">Se ha corregido un error con `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-659">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-660">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-660">VM</span></span>

* <span data-ttu-id="9efde-661">Se ha cambiado `list-skus` para que use la versión más reciente de la API para generar los detalles de la zona.</span><span class="sxs-lookup"><span data-stu-id="9efde-661">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="9efde-662">Se ha cambiado el valor predeterminado de `--single-placement-group` a `false` para `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-662">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="9efde-663">Se ha agregado la posibilidad de seleccionar SKU de almacenamiento ZRS para `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-663">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="9efde-664">Se ha agregado un nuevo grupo de comandos `vm host` para admitir hosts dedicados.</span><span class="sxs-lookup"><span data-stu-id="9efde-664">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="9efde-665">Se han agregado los parámetros `--host` y `--host-group` en `vm create` para establecer un host dedicado de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9efde-665">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="9efde-666">16 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-666">July 16, 2019</span></span>

<span data-ttu-id="9efde-667">Versión 2.0.69</span><span class="sxs-lookup"><span data-stu-id="9efde-667">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-668">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-668">Appservice</span></span>

* <span data-ttu-id="9efde-669">Se han cambiado los comandos de `webapp identity` para devolver un mensaje de error adecuado si el nombre del grupo de recursos o la aplicación no es válido.</span><span class="sxs-lookup"><span data-stu-id="9efde-669">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="9efde-670">Se ha corregido `webapp list` para devolver el valor correcto de numberOfSites si no se ha proporcionado ningún grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-670">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="9efde-671">Se han corregido los efectos secundarios de `appservice plan create` y `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-671">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="9efde-672">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-672">Core</span></span>

* <span data-ttu-id="9efde-673">Se ha corregido el problema por el que `--subscription` aparecía a pesar de no ser aplicable.</span><span class="sxs-lookup"><span data-stu-id="9efde-673">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-674">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-674">Batch</span></span>

* <span data-ttu-id="9efde-675">[CAMBIO IMPORTANTE] Se ha reemplazado `batch pool node-agent-skus list` por `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="9efde-675">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="9efde-676">Se ha agregado compatibilidad con las reglas de seguridad que bloquea el acceso de red a un grupo basado en el puerto de origen del tráfico cuando se usa la opción `--json-file` de `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="9efde-676">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="9efde-677">Agrega compatibilidad para ejecutar la tarea en el directorio de trabajo del contenedor o en el directorio de trabajo de la tarea por lotes cuando se usa la opción `--json-file` de `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-677">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="9efde-678">Se ha corregido el error en la opción `--application-package-references` de `batch pool create` por el que solo funcionaba con los valores predeterminados.</span><span class="sxs-lookup"><span data-stu-id="9efde-678">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9efde-679">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9efde-679">Eventhubs</span></span>

* <span data-ttu-id="9efde-680">Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-680">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-681">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-681">RDBMS</span></span>

* <span data-ttu-id="9efde-682">Se ha agregado un parámetro opcional para especificar la SKU de réplica para crear comandos de réplica.</span><span class="sxs-lookup"><span data-stu-id="9efde-682">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="9efde-683">Se ha corregido el problema con el error de prueba de CI al crear la réplica de MySQL.</span><span class="sxs-lookup"><span data-stu-id="9efde-683">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="9efde-684">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="9efde-684">Relay</span></span>

* <span data-ttu-id="9efde-685">Se ha corregido el problema con la conexión híbrida cuando la autorización del cliente está deshabilitada [n.º 8775](https://github.com/azure/azure-cli/issues/8775)</span><span class="sxs-lookup"><span data-stu-id="9efde-685">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="9efde-686">Se ha agregado el parámetro `--requires-transport-security` a `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-686">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9efde-687">Servicebus</span><span class="sxs-lookup"><span data-stu-id="9efde-687">Servicebus</span></span>

* <span data-ttu-id="9efde-688">Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-688">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-689">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-689">Storage</span></span>

* <span data-ttu-id="9efde-690">Habilitar archivos AADDS para la actualización de la cuenta de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="9efde-690">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="9efde-691">Se ha corregido el problema `storage blob service-properties update --set`</span><span class="sxs-lookup"><span data-stu-id="9efde-691">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="9efde-692">2 de julio de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-692">July 2, 2019</span></span>

<span data-ttu-id="9efde-693">Versión 2.0.68</span><span class="sxs-lookup"><span data-stu-id="9efde-693">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="9efde-694">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-694">Core</span></span>

* <span data-ttu-id="9efde-695">Los módulos de comandos ahora se consolidan en un único paquete distribuible de Python.</span><span class="sxs-lookup"><span data-stu-id="9efde-695">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="9efde-696">Esto reemplaza el uso directo de muchos paquetes `azure-cli-` en PyPI.</span><span class="sxs-lookup"><span data-stu-id="9efde-696">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="9efde-697">Esto reducirá el tamaño de la instalación y solo afecta a los usuarios que hayan instalado directamente mediante `pip`.</span><span class="sxs-lookup"><span data-stu-id="9efde-697">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-698">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-698">ACR</span></span>

* <span data-ttu-id="9efde-699">Se ha agregado compatibilidad para los desencadenadores de temporizador para las tareas.</span><span class="sxs-lookup"><span data-stu-id="9efde-699">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-700">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-700">Appservice</span></span>

* <span data-ttu-id="9efde-701">Se ha cambiado `functionapp create` para habilitar Application Insights de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9efde-701">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="9efde-702">[CAMBIO IMPORTANTE] Se ha dejado de utilizar el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="9efde-702">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="9efde-703">Use el nuevo comando `az functionapp devops-pipeline` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="9efde-703">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="9efde-704">Se ha agregado compatibilidad con el plan de aplicación de funciones Consumo para Linux a `functionapp deployment config-zip`.</span><span class="sxs-lookup"><span data-stu-id="9efde-704">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9efde-705">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9efde-705">Cosmos DB</span></span>

* <span data-ttu-id="9efde-706">Se ha agregado compatibilidad para deshabilitar TTL.</span><span class="sxs-lookup"><span data-stu-id="9efde-706">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="9efde-707">DLS</span><span class="sxs-lookup"><span data-stu-id="9efde-707">DLS</span></span>

* <span data-ttu-id="9efde-708">Se ha actualizado la versión de ADLS (0.0.45).</span><span class="sxs-lookup"><span data-stu-id="9efde-708">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="9efde-709">Comentarios</span><span class="sxs-lookup"><span data-stu-id="9efde-709">Feedback</span></span>

* <span data-ttu-id="9efde-710">Al informar de un error de comando de extensión, `az feedback` ahora intenta abrir el explorador en la dirección URL del repositorio del proyecto de la extensión desde el índice.</span><span class="sxs-lookup"><span data-stu-id="9efde-710">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-711">HDInsight</span></span>

* <span data-ttu-id="9efde-712">[CAMBIO IMPORTANTE] Se ha cambiado el nombre del grupo de comandos `oms` por `monitor`.</span><span class="sxs-lookup"><span data-stu-id="9efde-712">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="9efde-713">[CAMBIO IMPORTANTE] Ahora `--http-password/-p` es un parámetro necesario.</span><span class="sxs-lookup"><span data-stu-id="9efde-713">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="9efde-714">Se han agregado completadores para los parámetros `--cluster-admin-account` y `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="9efde-714">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="9efde-715">Se ha cambiado el parámetro `cluster-users-group-dns` para que sea necesario cuando `—esp` está presente.</span><span class="sxs-lookup"><span data-stu-id="9efde-715">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="9efde-716">Se ha agregado un tiempo de espera para todos los autocompletadores de argumentos existentes.</span><span class="sxs-lookup"><span data-stu-id="9efde-716">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="9efde-717">Se ha agregado un tiempo de espera para transformar el nombre de recurso en un identificador de recurso.</span><span class="sxs-lookup"><span data-stu-id="9efde-717">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="9efde-718">Se han cambiado los autocompletadores para seleccionar recursos de cualquier grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-718">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="9efde-719">Puede ser un grupo de recursos diferente a que se especifica con `-g`.</span><span class="sxs-lookup"><span data-stu-id="9efde-719">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="9efde-720">Se ha agregado compatibilidad con los parámetros `--sub-domain-suffix` y `--disable_gateway_auth` en el comando `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-720">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="9efde-721">Servicios administrados</span><span class="sxs-lookup"><span data-stu-id="9efde-721">Managed Services</span></span>

* <span data-ttu-id="9efde-722">Se ha introducido un módulo de comandos de servicios administrados en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="9efde-722">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-723">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-723">Profile</span></span>
* <span data-ttu-id="9efde-724">Se ha suprimido el argumento `--subscription` del comando de cierre de sesión.</span><span class="sxs-lookup"><span data-stu-id="9efde-724">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-725">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-725">RBAC</span></span>

* <span data-ttu-id="9efde-726">[CAMBIO IMPORTANTE] Se ha quitado el argumento `--password` de `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="9efde-726">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="9efde-727">Se ha agregado el parámetro `--assignee-principal-type` al comando `create` para evitar errores intermitentes causados por la latencia de replicación del servidor de grafos de AAD.</span><span class="sxs-lookup"><span data-stu-id="9efde-727">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="9efde-728">Se ha corregido un bloqueo en `ad signed-in-user` al enumerar los objetos que posee.</span><span class="sxs-lookup"><span data-stu-id="9efde-728">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="9efde-729">Se ha corregido el problema por el que `ad sp` no encontraba la aplicación correcta en una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="9efde-729">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-730">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-730">RDBMS</span></span>

* <span data-ttu-id="9efde-731">Se ha agregado compatibilidad para la replicación a MariaDB.</span><span class="sxs-lookup"><span data-stu-id="9efde-731">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-732">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-732">SQL</span></span>

* <span data-ttu-id="9efde-733">Se han documentado los valores permitidos para `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="9efde-733">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-734">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-734">Storage</span></span>

* <span data-ttu-id="9efde-735">Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9efde-735">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="9efde-736">Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9efde-736">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="9efde-737">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-737">VM</span></span>

* <span data-ttu-id="9efde-738">Se ha corregido un error por el que `vmss create` devuelve un mensaje de error cuando se ejecuta con `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-738">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="9efde-739">Se ha quitado la validación del lado cliente para `vmss create --single-placement-group`.</span><span class="sxs-lookup"><span data-stu-id="9efde-739">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="9efde-740">No genera ningún error si `--single-placement-group` está establecido en `true` y `--instance-count` es mayor que 100 o se especifican zonas de disponibilidad, y deja esta validación al servicio de proceso.</span><span class="sxs-lookup"><span data-stu-id="9efde-740">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="9efde-741">Se ha corregido el error por el que `[vm|vmss] extension image list` produce un error cuando se usa con `--latest`.</span><span class="sxs-lookup"><span data-stu-id="9efde-741">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="9efde-742">18 de junio de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-742">June 18, 2019</span></span>

<span data-ttu-id="9efde-743">Versión 2.0.67</span><span class="sxs-lookup"><span data-stu-id="9efde-743">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="9efde-744">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-744">Core</span></span>

<span data-ttu-id="9efde-745">Esta versión introduce una nueva etiqueta [Preview] para indicar con mayor claridad a los clientes si un grupo de comandos, un comando o un argumento está en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="9efde-745">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="9efde-746">Antes esto se comunicaba en el texto de ayuda o se indicaba explícitamente en el número de versión del módulo de comandos.</span><span class="sxs-lookup"><span data-stu-id="9efde-746">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="9efde-747">La CLI eliminará los números de versión de los paquetes individuales en el futuro.</span><span class="sxs-lookup"><span data-stu-id="9efde-747">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="9efde-748">Si un comando está en versión preliminar, todos sus argumentos también lo están.</span><span class="sxs-lookup"><span data-stu-id="9efde-748">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="9efde-749">Si un grupo de comandos está etiquetado como versión preliminar, se consideran que todos los comandos y argumentos también están en versión preliminar.</span><span class="sxs-lookup"><span data-stu-id="9efde-749">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="9efde-750">Como resultado de este cambio, pueden parecer que varios grupos de comandos están "repentinamente" en versión preliminar con esta versión.</span><span class="sxs-lookup"><span data-stu-id="9efde-750">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="9efde-751">Lo que realmente ha sucede es que la mayoría de los paquetes estaban en versión preliminar, pero se considera que están disponibles con carácter general con esta versión.</span><span class="sxs-lookup"><span data-stu-id="9efde-751">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-752">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-752">ACR</span></span>
* <span data-ttu-id="9efde-753">Se ha agregado el comando "acr check-health".</span><span class="sxs-lookup"><span data-stu-id="9efde-753">Added 'acr check-health' command</span></span>
* <span data-ttu-id="9efde-754">Mejor control de los errores para los tokens AAD y para recuperar los comandos externos.</span><span class="sxs-lookup"><span data-stu-id="9efde-754">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-755">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-755">ACS</span></span>
* <span data-ttu-id="9efde-756">Los comandos en desuso de ACS ya no se muestran en la vista de la ayuda.</span><span class="sxs-lookup"><span data-stu-id="9efde-756">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-757">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-757">AMS</span></span>
* <span data-ttu-id="9efde-758">[CAMBIO IMPORTANTE] Las cadenas de hora ISO 8601 se han cambiado para volver a archive-window-length y key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="9efde-758">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-759">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-759">AppService</span></span>
* <span data-ttu-id="9efde-760">Se ha agregado el enrutamiento basado en la ubicación para `webapp deleted list` y `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="9efde-760">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="9efde-761">Se ha corregido el problema por el que no se podía hacer clic la dirección URL de destino registrada de la aplicación web ("Puede iniciar la aplicación en...") en Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="9efde-761">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="9efde-762">Se ha corregido el problema por el que, al crear aplicaciones con algunas SKU, se producía un error de AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="9efde-762">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="9efde-763">Se ha agregado validación previa a `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-763">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="9efde-764">Se ha corregido `[webapp|functionapp] traffic-routing` para usar el valor correcto de actionHostName.</span><span class="sxs-lookup"><span data-stu-id="9efde-764">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="9efde-765">Se ha agregado compatibilidad con ranuras a los comandos `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="9efde-765">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-766">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-766">Batch</span></span>
* <span data-ttu-id="9efde-767">Se ha corregido la regresión de autenticación de AAD causada por una notificación demasiado agresiva de errores de autenticación de clave compartida.</span><span class="sxs-lookup"><span data-stu-id="9efde-767">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="9efde-768">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9efde-768">BatchAI</span></span>
* <span data-ttu-id="9efde-769">Los comandos de BatchAI han dejado de usarse y están ocultos.</span><span class="sxs-lookup"><span data-stu-id="9efde-769">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-770">BotService</span><span class="sxs-lookup"><span data-stu-id="9efde-770">BotService</span></span>
* <span data-ttu-id="9efde-771">Se ha agregado un aviso de advertencia "compatibilidad descontinuada" o "modo de mantenimiento" a los comandos que admiten el SDK v3.</span><span class="sxs-lookup"><span data-stu-id="9efde-771">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-772">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-772">CosmosDB</span></span>
* <span data-ttu-id="9efde-773">[EN DESUSO] Se ha dejado de usar el comando `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="9efde-773">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="9efde-774">Se ha agregado el comando `cosmosdb keys list`, que reemplaza a `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="9efde-774">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="9efde-775">`cosmsodb create/update`: Se ha agregado el nuevo formato a --location para poder establecer la propiedad "isZoneRedundant".</span><span class="sxs-lookup"><span data-stu-id="9efde-775">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="9efde-776">Formato antiguo en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-776">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9efde-777">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9efde-777">EventGrid</span></span>
* <span data-ttu-id="9efde-778">Se han agregado comandos `eventgrid domain` para las operaciones CRUD de dominios.</span><span class="sxs-lookup"><span data-stu-id="9efde-778">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="9efde-779">Se han agregado comandos `eventgrid domain topic` para las operaciones CRUD de temas de dominio.</span><span class="sxs-lookup"><span data-stu-id="9efde-779">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="9efde-780">Se ha agregado el argumento `--odata-query` a `eventgrid [topic|event-subscription] list` para filtrar los resultados mediante la sintaxis de OData.</span><span class="sxs-lookup"><span data-stu-id="9efde-780">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="9efde-781">`event-subscription create/update`: Se ha agregado servicebusqueue como nuevos valores para el parámetro `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="9efde-781">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="9efde-782">[CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para `--included-event-types All` con `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-782">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-783">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-783">HDInsight</span></span>
* <span data-ttu-id="9efde-784">Se ha agregado compatibilidad con el parámetro `--ssh-public-key` al comando `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-784">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-785">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-785">IoT</span></span>
* <span data-ttu-id="9efde-786">Se ha agregado compatibilidad para volver a generar las claves de directiva de autorización.</span><span class="sxs-lookup"><span data-stu-id="9efde-786">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="9efde-787">Se ha agregado un SDK y compatibilidad con el servicio de aprovisionamiento de repositorio de DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="9efde-787">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="9efde-788">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-788">Network</span></span>
* <span data-ttu-id="9efde-789">Se ha agregado compatibilidad de las zonas con puertas de enlace NAT.</span><span class="sxs-lookup"><span data-stu-id="9efde-789">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="9efde-790">Se ha agregado el comando `network list-service-tags`</span><span class="sxs-lookup"><span data-stu-id="9efde-790">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="9efde-791">Se ha corregido el problema con `dns zone import` por el que los usuarios no podían importar registros A con caracteres comodín.</span><span class="sxs-lookup"><span data-stu-id="9efde-791">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="9efde-792">Se ha corregido el problema con `watcher flow-log configure` por el que no se podía habilitar el registro de flujos en determinadas regiones.</span><span class="sxs-lookup"><span data-stu-id="9efde-792">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-793">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-793">Resource</span></span>
* <span data-ttu-id="9efde-794">Se ha agregado el comando `az rest` para hacer llamadas de REST.</span><span class="sxs-lookup"><span data-stu-id="9efde-794">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="9efde-795">Se ha corregido el error al usar `policy assignment list` con un grupo de recursos o un nivel de suscripción `--scope`.</span><span class="sxs-lookup"><span data-stu-id="9efde-795">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="9efde-796">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9efde-796">ServiceBus</span></span>
* <span data-ttu-id="9efde-797">Se ha corregido el error con `servicebus topic create --max-size` [9319](https://github.com/azure/azure-cli/issues/9319).</span><span class="sxs-lookup"><span data-stu-id="9efde-797">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-798">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-798">SQL</span></span>
* <span data-ttu-id="9efde-799">Se ha cambiado `--location` para que sea opcionalpara `sql [server|mi] create`; usa la ubicación del grupo de recursos si no se especifica.</span><span class="sxs-lookup"><span data-stu-id="9efde-799">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="9efde-800">Se ha corregido el error "No se puede iterar en el objeto NoneType" para `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="9efde-800">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="9efde-801">SQLVm</span><span class="sxs-lookup"><span data-stu-id="9efde-801">SQLVm</span></span>
* <span data-ttu-id="9efde-802">[CAMBIO IMPORTANTE] Se ha cambiado `sql vm create` para requerir el parámetro `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="9efde-802">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="9efde-803">Se ha cambiado para poder establecer el SKU de la imagen de SQL al crear o actualizar una máquina virtual de SQL.</span><span class="sxs-lookup"><span data-stu-id="9efde-803">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-804">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-804">Storage</span></span>
* <span data-ttu-id="9efde-805">Se ha corregido un problema con una clave de cuenta que falta para `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9efde-805">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="9efde-806">Se ha corregido un problema con `storage blob sync` en Linux.</span><span class="sxs-lookup"><span data-stu-id="9efde-806">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-807">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-807">VM</span></span>
* <span data-ttu-id="9efde-808">[VERSIÓN PRELIMINAR] Se han agregado los comandos `vm image template` para compilar imágenes de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9efde-808">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="9efde-809">4 de junio de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-809">June 4, 2019</span></span>

<span data-ttu-id="9efde-810">Versión 2.0.66</span><span class="sxs-lookup"><span data-stu-id="9efde-810">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="9efde-811">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-811">Core</span></span>
* <span data-ttu-id="9efde-812">Se ha corregido el problema por el que los comandos generan un error si `--output yaml` se usa con `--query`.</span><span class="sxs-lookup"><span data-stu-id="9efde-812">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-813">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-813">ACR</span></span>
* <span data-ttu-id="9efde-814">Se ha agregado el grupo de comandos "acr pack" para crear tareas de compilación rápida mediante Buildpacks.</span><span class="sxs-lookup"><span data-stu-id="9efde-814">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-815">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-815">ACS</span></span>
* <span data-ttu-id="9efde-816">Se permite habilitar o deshabilitar el complemento kube-dashboard de AKS.</span><span class="sxs-lookup"><span data-stu-id="9efde-816">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="9efde-817">Se imprime un mensaje descriptivo cuando la suscripción no está en la lista de permitidos para usar Azure Red Hat OpenShift.</span><span class="sxs-lookup"><span data-stu-id="9efde-817">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-818">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-818">Batch</span></span>
* <span data-ttu-id="9efde-819">Se ha mejorado el control de errores cuando no se ha iniciado sesión en una cuenta \[[9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="9efde-819">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-820">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-820">IoT</span></span>
* <span data-ttu-id="9efde-821">Se ha agregado compatibilidad para la conmutación por error manual.</span><span class="sxs-lookup"><span data-stu-id="9efde-821">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="9efde-822">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-822">Network</span></span>
* <span data-ttu-id="9efde-823">Se han agregado comandos `network application-gateway waf-policy` para admitir reglas personalizadas de WAF.</span><span class="sxs-lookup"><span data-stu-id="9efde-823">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="9efde-824">Se agregaron los argumentos `--waf-policy` y `--max-capacity` a `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-824">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="9efde-825">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-825">Resource</span></span>
* <span data-ttu-id="9efde-826">Se ha mejorado el mensaje de error de `deployment create` cuando TTY no está disponible.</span><span class="sxs-lookup"><span data-stu-id="9efde-826">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="9efde-827">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-827">Role</span></span>
* <span data-ttu-id="9efde-828">Texto de ayuda actualizado.</span><span class="sxs-lookup"><span data-stu-id="9efde-828">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-829">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-829">Compute</span></span>
* <span data-ttu-id="9efde-830">Se ha agregado compatibilidad a `vm create` para máquinas virtuales desde una imagen administrada con LUN de discos de datos que no comienzan en 0 o que omiten los números.</span><span class="sxs-lookup"><span data-stu-id="9efde-830">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="9efde-831">21 de mayo de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-831">May 21, 2019</span></span>

<span data-ttu-id="9efde-832">Versión 2.0.65</span><span class="sxs-lookup"><span data-stu-id="9efde-832">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="9efde-833">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-833">Core</span></span>
* <span data-ttu-id="9efde-834">Se han agregado mejores comentarios para los errores de autenticación.</span><span class="sxs-lookup"><span data-stu-id="9efde-834">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="9efde-835">Se ha corregido un problema por el que la CLI cargaba extensiones que no eran compatibles con su versión principal.</span><span class="sxs-lookup"><span data-stu-id="9efde-835">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="9efde-836">Se ha corregido un problema con el inicio cuando `clouds.config` estaba dañado.</span><span class="sxs-lookup"><span data-stu-id="9efde-836">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-837">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-837">ACR</span></span>
* <span data-ttu-id="9efde-838">Se ha agregado compatibilidad para identidades administradas a Tareas.</span><span class="sxs-lookup"><span data-stu-id="9efde-838">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-839">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-839">ACS</span></span>
* <span data-ttu-id="9efde-840">Se ha corregido el comando `openshift create` cuando se usa con el cliente AAD.</span><span class="sxs-lookup"><span data-stu-id="9efde-840">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-841">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-841">AppService</span></span>
* <span data-ttu-id="9efde-842">[EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`; se quitará en la próxima versión.</span><span class="sxs-lookup"><span data-stu-id="9efde-842">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="9efde-843">Se ha cambiado `functionapp devops-pipeline` para recopilar el registro de compilación de Azure DevOps en modo detallado.</span><span class="sxs-lookup"><span data-stu-id="9efde-843">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="9efde-844">[CAMBIO IMPORTANTE] Se ha eliminado la marca `--use_local_settings` del comando `functionapp devops-pipeline`; no era operativa.</span><span class="sxs-lookup"><span data-stu-id="9efde-844">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="9efde-845">Se ha cambiado `webapp up` para que devuelva la salida JSON si no se usa `--logs`.</span><span class="sxs-lookup"><span data-stu-id="9efde-845">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="9efde-846">Se ha agregado compatibilidad para escribir los recursos predeterminados en la configuración local para `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9efde-846">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="9efde-847">Se ha agregado compatibilidad para `webapp up` para volver a implementar una aplicación sin usar el argumento `--location`.</span><span class="sxs-lookup"><span data-stu-id="9efde-847">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="9efde-848">Se ha corregido un problema por el que, al crear un ASP en la SKU gratuita de Linux, el valor de SKU "Fee" no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9efde-848">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-849">BotService</span><span class="sxs-lookup"><span data-stu-id="9efde-849">BotService</span></span>
* <span data-ttu-id="9efde-850">Se ha cambiado para permitir las mayúsculas y minúsculas para los parámetros `--lang` de los comandos.</span><span class="sxs-lookup"><span data-stu-id="9efde-850">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="9efde-851">Se ha actualizado la descripción para el módulo de comandos.</span><span class="sxs-lookup"><span data-stu-id="9efde-851">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="9efde-852">Consumo</span><span class="sxs-lookup"><span data-stu-id="9efde-852">Consumption</span></span>
* <span data-ttu-id="9efde-853">Se ha agregado un parámetro obligatorio que faltaba al ejecutar `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="9efde-853">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-854">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-854">IoT</span></span>
* <span data-ttu-id="9efde-855">Se ha agregado compatibilidad para enumerar todas las claves.</span><span class="sxs-lookup"><span data-stu-id="9efde-855">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="9efde-856">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-856">Network</span></span>
* [CAMBIO IMPORTANTE]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="9efde-858">Se ha agregado el argumento `--nat-gateway` a `network vnet subnet [create|update]` para adjuntar a una puerta de enlace NAT.</span><span class="sxs-lookup"><span data-stu-id="9efde-858">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="9efde-859">Se ha corregido el problema con `dns zone import` por el que los nombres de registro no encontraban un tipo de registro.</span><span class="sxs-lookup"><span data-stu-id="9efde-859">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-860">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-860">RDBMS</span></span>
* <span data-ttu-id="9efde-861">Se ha agregado compatibilidad con replicación geográfica a mysql y postgres.</span><span class="sxs-lookup"><span data-stu-id="9efde-861">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-862">RBAC</span><span class="sxs-lookup"><span data-stu-id="9efde-862">RBAC</span></span>
* <span data-ttu-id="9efde-863">Se ha agregado compatibilidad para el ámbito de grupos de administración a `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="9efde-863">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-864">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-864">Storage</span></span>
* <span data-ttu-id="9efde-865">`storage blob sync`: se ha agregado el comando sync a Blob Storage.</span><span class="sxs-lookup"><span data-stu-id="9efde-865">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="9efde-866">Proceso</span><span class="sxs-lookup"><span data-stu-id="9efde-866">Compute</span></span>
* <span data-ttu-id="9efde-867">Se ha agregado `--computer-name` a `vm create` para establecer el nombre de equipo de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9efde-867">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="9efde-868">Se ha cambiado el nombre de `--ssh-key-value` a `--ssh-key-values` para `[vm|vmss] create`; ahora pueden aceptar varios valores ssh de clave pública o rutas de acceso.</span><span class="sxs-lookup"><span data-stu-id="9efde-868">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="9efde-869">__Nota__: Este **no** es un cambio importante. `--ssh-key-value` se analizará correctamente porque solo coincide con `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="9efde-869">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="9efde-870">Se ha cambiado el argumento `--type` de `ppg create` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="9efde-870">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="9efde-871">6 de mayo de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-871">May 6, 2019</span></span>

<span data-ttu-id="9efde-872">Versión 2.0.64</span><span class="sxs-lookup"><span data-stu-id="9efde-872">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-873">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-873">ACS</span></span>
* <span data-ttu-id="9efde-874">[CAMBIO IMPORTANTE] Se ha eliminado la marca `--fqdn` de los comandos `openshift`.</span><span class="sxs-lookup"><span data-stu-id="9efde-874">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="9efde-875">Se ha cambiado para usar la versión GA de la API Openshift de Azure Red Hat.</span><span class="sxs-lookup"><span data-stu-id="9efde-875">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="9efde-876">Se ha agregado la marca `customer-admin-group-id` a `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-876">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="9efde-877">[GA] Se ha quitado `(PREVIEW)` de la opción `--network-policy` de `aks create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-877">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-878">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-878">Appservice</span></span>
* <span data-ttu-id="9efde-879">[EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="9efde-879">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="9efde-880">Se ha cambiado el nombre a `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="9efde-880">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="9efde-881">Se ha corregido un error por el que no se podía obtener el nombre de usuario correcto para cloudshell, lo que provocaba un error de `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9efde-881">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="9efde-882">Se ha actualziado la documentación de `appservice plan --sku` para incluir la compatibilidad con appserviceplans.</span><span class="sxs-lookup"><span data-stu-id="9efde-882">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="9efde-883">Se han agregado argumentos opcionales para el grupo de recursos y el plan a `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="9efde-883">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="9efde-884">Se ha agregado compatibilidad a `webapp ssh` para respetar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="9efde-884">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="9efde-885">Se ha agregado compatibilidad a `appserviceplan create` con la SKU gratuita de Linux.</span><span class="sxs-lookup"><span data-stu-id="9efde-885">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="9efde-886">Se ha cambiado `webapp up` para que haya una suspensión de 30 segundos después de configurar la opción `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para controlar el inicio en frío de kudu.</span><span class="sxs-lookup"><span data-stu-id="9efde-886">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="9efde-887">Se ha agregado compatibilidad con el entorno de ejecución `powershell` a `functionapp create` en Windows.</span><span class="sxs-lookup"><span data-stu-id="9efde-887">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="9efde-888">Se agregó el comando `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="9efde-888">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-889">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-889">Batch</span></span>
* <span data-ttu-id="9efde-890">Se ha corregido un error en el validador para las opciones de `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="9efde-890">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-891">Botservice</span><span class="sxs-lookup"><span data-stu-id="9efde-891">Botservice</span></span>
* <span data-ttu-id="9efde-892">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para crear un bot de Web App vacío de forma predeterminada (es decir, el bot no se implementa en App Service).</span><span class="sxs-lookup"><span data-stu-id="9efde-892">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="9efde-893">Se ha agregado la marca `--echo` a `bot create` para usar el comportamiento anterior con `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="9efde-893">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="9efde-894">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--version` a `v4`.</span><span class="sxs-lookup"><span data-stu-id="9efde-894">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="9efde-895">__NOTA:__ `bot prepare-publish` sigue usando el valor predeterminado anterior.</span><span class="sxs-lookup"><span data-stu-id="9efde-895">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="9efde-896">[CAMBIO IMPORTANTE] Se ha cambiado `--lang` para que su valor predeterminado ya no sea `Csharp`.</span><span class="sxs-lookup"><span data-stu-id="9efde-896">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="9efde-897">Si el comando requiere `--lang` y no se proporciona, ahora producirá un error.</span><span class="sxs-lookup"><span data-stu-id="9efde-897">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="9efde-898">[CAMBIO IMPORTANTE] Se han cambiado los argumentos `--appid` y `--password` de `bot create` para que sean necesarios y ahora se pueden crear mediante `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-898">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="9efde-899">Se ha agregado la validación de `--appid` y `--password`.</span><span class="sxs-lookup"><span data-stu-id="9efde-899">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="9efde-900">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4` para que no cree ni use una cuenta de almacenamiento ni Application Insights.</span><span class="sxs-lookup"><span data-stu-id="9efde-900">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="9efde-901">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v3` para que requiera una región donde esté disponible Application Insights.</span><span class="sxs-lookup"><span data-stu-id="9efde-901">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="9efde-902">[CAMBIO IMPORTANTE] Se ha cambiado `bot update` para que ahora afecte solo a determinadas propiedades de un bot.</span><span class="sxs-lookup"><span data-stu-id="9efde-902">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="9efde-903">[CAMBIO IMPORTANTE] Se han cambiado las marcas `--lang` para que acepten `Javascript` en lugar de `Node`.</span><span class="sxs-lookup"><span data-stu-id="9efde-903">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="9efde-904">[CAMBIO IMPORTANTE] Se ha quitado `Node` como valor de `--lang` permitido.</span><span class="sxs-lookup"><span data-stu-id="9efde-904">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="9efde-905">[CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para que no establezca `SCM_DO_BUILD_DURING_DEPLOYMENT` en true.</span><span class="sxs-lookup"><span data-stu-id="9efde-905">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="9efde-906">Todas las implementaciones a través de Kudu actuarán según su comportamiento predeterminado.</span><span class="sxs-lookup"><span data-stu-id="9efde-906">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="9efde-907">Se ha cambiado `bot download` para los bots sin archivos `.bot` para crear el archivo de configuración específico del idioma con los valores de Application Insights para el bot.</span><span class="sxs-lookup"><span data-stu-id="9efde-907">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="9efde-908">Se ha agregado compatibilidad de `Typescript` con `bot prepare-deploy`</span><span class="sxs-lookup"><span data-stu-id="9efde-908">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9efde-909">Se ha agregado un mensaje de advertencia a `bot prepare-deploy` para los bots `Javascript` y `Typescript` cuando `--code-dir` no contiene `package.json`.</span><span class="sxs-lookup"><span data-stu-id="9efde-909">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="9efde-910">Se ha cambiado `bot prepare-deploy` para que devuelva `true` si es correcto.</span><span class="sxs-lookup"><span data-stu-id="9efde-910">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="9efde-911">Se ha agregado el registro detallado a `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="9efde-911">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="9efde-912">Se han agregado regiones más disponibles de Application Insights a `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="9efde-912">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="9efde-913">Configuración</span><span class="sxs-lookup"><span data-stu-id="9efde-913">Configure</span></span>
* <span data-ttu-id="9efde-914">Se ha agregado compatibilidad para configuraciones de valores predeterminados de argumentos basadas en carpetas.</span><span class="sxs-lookup"><span data-stu-id="9efde-914">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9efde-915">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9efde-915">Eventhubs</span></span>
* <span data-ttu-id="9efde-916">Se agregaron los comandos `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-916">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9efde-917">Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-917">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-918">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-918">Network</span></span>
* <span data-ttu-id="9efde-919">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--cache` con `--defer` para `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-919">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="9efde-920">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-920">Policy Insights</span></span>
* <span data-ttu-id="9efde-921">Se ha agregado compatibilidad a `--expand PolicyEvaluationDetails` para consultar detalles de evaluación de directivas en el recurso.</span><span class="sxs-lookup"><span data-stu-id="9efde-921">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="9efde-922">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-922">Role</span></span>
* <span data-ttu-id="9efde-923">[EN DESUSO] Se ha cambiado el argumento `create-for-rbac` hide '--password' y se dejará de dar soporte en mayo de 2019.</span><span class="sxs-lookup"><span data-stu-id="9efde-923">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="9efde-924">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9efde-924">Service Bus</span></span>
* <span data-ttu-id="9efde-925">Se agregaron los comandos `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-925">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="9efde-926">Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-926">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="9efde-927">Se ha corregido `topic [create|update]` para que `--max-size` permita valores de 10, 20, 40 y 80 GB con SKU Premium.</span><span class="sxs-lookup"><span data-stu-id="9efde-927">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-928">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-928">SQL</span></span>
* <span data-ttu-id="9efde-929">Se agregaron los comandos `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-929">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-930">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-930">VM</span></span>
* <span data-ttu-id="9efde-931">Se ha agregado `--protect-from-scale-in` y `--protect-from-scale-set-actions` a `vmss update` para habilitar las actualizaciones a la directiva de protección de instancias de máquina virtual de VMSS.</span><span class="sxs-lookup"><span data-stu-id="9efde-931">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="9efde-932">Se ha agregado `--instance-id` a `vmss update` para habilitar la actualización genérica de instancias de máquina virtual de VMSS.</span><span class="sxs-lookup"><span data-stu-id="9efde-932">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="9efde-933">Se ha agregado `--instance-id` a `vmss wait`</span><span class="sxs-lookup"><span data-stu-id="9efde-933">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="9efde-934">Se ha agregado un nuevo grupo de comandos `ppg` para administrar grupos de ubicación de proximidad.</span><span class="sxs-lookup"><span data-stu-id="9efde-934">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="9efde-935">Se ha agregado `--ppg` a `[vm|vmss] create` y `vm availability-set create` para administrar grupos de ubicación de proximidad.</span><span class="sxs-lookup"><span data-stu-id="9efde-935">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="9efde-936">Se ha agregado el parámetro `--hyper-v-generation` a `image create`</span><span class="sxs-lookup"><span data-stu-id="9efde-936">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="9efde-937">23 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-937">April 23, 2019</span></span>

<span data-ttu-id="9efde-938">Versión 2.0.63</span><span class="sxs-lookup"><span data-stu-id="9efde-938">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-939">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-939">ACS</span></span>
* <span data-ttu-id="9efde-940">Se ha cambiado `aks get-credentials` para que pregunte si se desean sobrescribir los valores duplicados.</span><span class="sxs-lookup"><span data-stu-id="9efde-940">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="9efde-941">Se ha quitado `(PREVIEW)` de los comandos de DevSpaces "aks use-dev-spaces" y "aks remove-dev-spaces".</span><span class="sxs-lookup"><span data-stu-id="9efde-941">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-942">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-942">AMS</span></span>
* <span data-ttu-id="9efde-943">Se ha corregido un error con la actualización de los filtros de cuenta y recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-943">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-944">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-944">AppService</span></span>
* <span data-ttu-id="9efde-945">Se ha agregado compatibilidad para ASE y un tiempo de espera a `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="9efde-945">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="9efde-946">Se ha agregado compatibilidad para establecer la integración e implementación continuas a una canalización de Azure DevOps desde un repositorio de Github para aplicaciones de función.</span><span class="sxs-lookup"><span data-stu-id="9efde-946">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="9efde-947">Se ha agregado el argumento `--github-pat` a `functionapp devops-build create` para aceptar el token de acceso personal de Github.</span><span class="sxs-lookup"><span data-stu-id="9efde-947">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="9efde-948">Se ha agregado el argumento `--github-repository` a `functionapp devops-build create` para aceptar el repositorio de Github que contiene un código de origen de aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="9efde-948">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="9efde-949">Se ha corregido el problema por el que `az webapp up --logs` producía un error y actualizaba .NETCORE a la versión 2.1 de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9efde-949">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="9efde-950">Se han quitado las opciones de configuración de aplicaciones de función innecesarias a la hora de crear una aplicación de función con un plan de consumo.</span><span class="sxs-lookup"><span data-stu-id="9efde-950">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="9efde-951">Se ha cambiado `webapp up` para que la cadena asp predeterminada ahora anexe el número al final para crear un nuevo ASP según las opciones de SKU.</span><span class="sxs-lookup"><span data-stu-id="9efde-951">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="9efde-952">Se ha agregado `-b` como opción a `webapp up` para iniciar la aplicación en el explorador.</span><span class="sxs-lookup"><span data-stu-id="9efde-952">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="9efde-953">Se ha cambiado `webapp deployment source config zip` para controlar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="9efde-953">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="9efde-954">Administrador de implementaciones</span><span class="sxs-lookup"><span data-stu-id="9efde-954">Deployment Manager</span></span>
* <span data-ttu-id="9efde-955">[VERSIÓN PRELIMINAR] Creación y administración de artefactos que admiten lanzamientos.</span><span class="sxs-lookup"><span data-stu-id="9efde-955">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="9efde-956">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-956">Lab</span></span>
* <span data-ttu-id="9efde-957">Se ha corregido el error que provocaba una salida prematura.</span><span class="sxs-lookup"><span data-stu-id="9efde-957">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="9efde-958">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-958">Network</span></span>
* <span data-ttu-id="9efde-959">Se ha agregado la delegación de servidor nombre automática a `dns zone create` en la zona primaria durante la creación de una zona secundaria.</span><span class="sxs-lookup"><span data-stu-id="9efde-959">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-960">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-960">Resource</span></span>
* <span data-ttu-id="9efde-961">[EN DESUSO] Se han dejado de usar los argumentos `--link-id`, `--target-id` y `--filter-string` de `resource link`.</span><span class="sxs-lookup"><span data-stu-id="9efde-961">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="9efde-962">En su lugar, use los argumentos `--link`, `--target` y `--filter`.</span><span class="sxs-lookup"><span data-stu-id="9efde-962">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="9efde-963">Se ha corregido el problema por el que los comandos `resource link [create|update]` no funcionaban.</span><span class="sxs-lookup"><span data-stu-id="9efde-963">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="9efde-964">Se ha corregido un problema por el que se podía producir un problema al eliminar utilizando un identificador de recurso.</span><span class="sxs-lookup"><span data-stu-id="9efde-964">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-965">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-965">SQL</span></span>
* <span data-ttu-id="9efde-966">Se ha agregado compatibilidad para zonas horarias personalizadas en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="9efde-966">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="9efde-967">Se ha cambiado para poder usar un nombre de grupo elástico con `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-967">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="9efde-968">Se ha agregado compatibilidad de `--no-wait` con `sql server [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-968">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="9efde-969">Se ha agregado el comando `sql server wait`</span><span class="sxs-lookup"><span data-stu-id="9efde-969">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-970">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-970">Storage</span></span>
* <span data-ttu-id="9efde-971">Se ha corregido un problema con los tokens de SAS de codificación doble en `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="9efde-971">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-972">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-972">VM</span></span>
* <span data-ttu-id="9efde-973">Se ha agregado la marca `--skip-shutdown` a `vm|vmss stop` para apagar las máquinas virtuales sin cerrarlas.</span><span class="sxs-lookup"><span data-stu-id="9efde-973">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="9efde-974">Se ha agregado el argumento `--storage-account-type` a `sig image-version create` para establecer el tipo de cuenta del perfil de publicación.</span><span class="sxs-lookup"><span data-stu-id="9efde-974">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="9efde-975">Se ha agregado el argumento `--target-regions` a `sig image-version create` para permitir tipos de cuenta de almacenamiento específicos de la región.</span><span class="sxs-lookup"><span data-stu-id="9efde-975">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="9efde-976">9 de abril de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-976">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="9efde-977">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-977">Core</span></span>
* <span data-ttu-id="9efde-978">Se ha corregido el problema por el que algunas extensiones mostraban una versión `Unknown` y no se podían actualizar.</span><span class="sxs-lookup"><span data-stu-id="9efde-978">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-979">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-979">ACR</span></span>
* <span data-ttu-id="9efde-980">Se ha agregado compatibilidad con la ejecución de una imagen sin contexto.</span><span class="sxs-lookup"><span data-stu-id="9efde-980">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-981">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-981">AMS</span></span>
* [EN DESUSO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CAMBIO IMPORTANTE]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="9efde-984">Se ha agregado compatibilidad con nuevos parámetros de cifrado a `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-984">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="9efde-985">Se ha agregado un nuevo parámetro `--filters` a `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-985">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-986">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-986">AppService</span></span>
* <span data-ttu-id="9efde-987">Se ha agregado compatibilidad de `--logs` con `webapp up`</span><span class="sxs-lookup"><span data-stu-id="9efde-987">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="9efde-988">En el comando `functionapp devops-build create`, se han corregido los problemas de generación de `azure-pipelines.yml`</span><span class="sxs-lookup"><span data-stu-id="9efde-988">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="9efde-989">Se ha mejorado el control de errores y los indicadores de `unctionapp devops-build create`</span><span class="sxs-lookup"><span data-stu-id="9efde-989">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="9efde-990">[CAMBIO IMPORTANTE] Se ha quitado la marca `--local-git` del comando `devops-build`; la detección y administración del repositorio git local son obligatorias para crear canalizaciones de Azure DevOps</span><span class="sxs-lookup"><span data-stu-id="9efde-990">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="9efde-991">Se ha agregado compatibilidad para crear planes de funciones Linux</span><span class="sxs-lookup"><span data-stu-id="9efde-991">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="9efde-992">Se ha agregado la posibilidad de cambiar el plan de una aplicación de función mediante `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="9efde-992">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="9efde-993">Se ha agregado compatibilidad para las opciones de escalado horizontal del plan Premium de Azure Functions</span><span class="sxs-lookup"><span data-stu-id="9efde-993">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-994">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-994">CDN</span></span>
* <span data-ttu-id="9efde-995">Se ha agregado compatibilidad para `Microsoft_Standard` y `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="9efde-995">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="9efde-996">Comentarios</span><span class="sxs-lookup"><span data-stu-id="9efde-996">Feedback</span></span>
* <span data-ttu-id="9efde-997">Se ha cambiado `feedback` para mostrar los metadatos de los comandos ejecutados recientemente</span><span class="sxs-lookup"><span data-stu-id="9efde-997">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="9efde-998">Se ha cambiado `feedback` para pedir al usuario que abra un explorador y use una plantilla de incidencia para ayudar en el proceso de creación de la incidencia</span><span class="sxs-lookup"><span data-stu-id="9efde-998">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="9efde-999">Se ha cambiado `feedback` para imprimir el cuerpo de la incidencia cuando se ejecuta con "--verbose"</span><span class="sxs-lookup"><span data-stu-id="9efde-999">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-1000">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1000">Monitor</span></span>
* <span data-ttu-id="9efde-1001">Se ha corregido un problema por "count" no era un valor permitido en `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1001">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="9efde-1002">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1002">Network</span></span>
* <span data-ttu-id="9efde-1003">Se ha corregido el formato de tabla que no se mostraba con `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1003">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="9efde-1004">Se han agregado los comandos `list-request-headers` y `list-response-headers` a `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1004">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="9efde-1005">Se ha agregado el comando `list-server-variables` a `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1005">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="9efde-1006">Se ha corregido un problema por el que actualización del estado de un vínculo en un puerto de express-route generaba una excepción de atributo desconocido `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1006">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="9efde-1007">PrivateDNS</span><span class="sxs-lookup"><span data-stu-id="9efde-1007">PrivateDNS</span></span>
* <span data-ttu-id="9efde-1008">Se ha agregado `network private-dns` para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="9efde-1008">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1009">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1009">Resource</span></span>
* <span data-ttu-id="9efde-1010">Se ha corregido el problema con `deployment create` y `group deployment create` por el que no funcionaba un archivo de parámetros con un conjunto de parámetros vacío</span><span class="sxs-lookup"><span data-stu-id="9efde-1010">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1011">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1011">Role</span></span>
* <span data-ttu-id="9efde-1012">Se ha corregido `create-for-rbac` para que trate `--years` correctamente</span><span class="sxs-lookup"><span data-stu-id="9efde-1012">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="9efde-1013">[CAMBIO IMPORTANTE] Se ha cambiado `role assignment delete` para preguntar cuando se eliminan todas las asignaciones de la suscripción de forma incondicional</span><span class="sxs-lookup"><span data-stu-id="9efde-1013">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-1014">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1014">SQL</span></span>
* <span data-ttu-id="9efde-1015">Se ha actualizado `sql mi [create|update]` con las propiedades proxyOverride y publicDataEndpointEnabled</span><span class="sxs-lookup"><span data-stu-id="9efde-1015">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1016">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1016">Storage</span></span>
* <span data-ttu-id="9efde-1017">[CAMBIO IMPORTANTE] Se ha quitado el resultado de `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1017">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="9efde-1018">Se ha agregado `--full-uri` a `storage blob generate-sas` para crear el URI completo para el blob con SAS</span><span class="sxs-lookup"><span data-stu-id="9efde-1018">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="9efde-1019">Se ha agregado `--file-snapshot` a `storage file copy start` para copiar el archivo desde la instantánea</span><span class="sxs-lookup"><span data-stu-id="9efde-1019">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="9efde-1020">Se ha cambiado `storage blob copy cancel` para mostrar solo el error en lugar de la excepción para NoPendingCopyOperation</span><span class="sxs-lookup"><span data-stu-id="9efde-1020">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="9efde-1021">26 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-1021">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="9efde-1022">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1022">Core</span></span>
* <span data-ttu-id="9efde-1023">Se han corregido problemas con la incompatibilidad de la extensión de desarrollo.</span><span class="sxs-lookup"><span data-stu-id="9efde-1023">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="9efde-1024">El control de errores ahora dirige a los clientes a la página de problemas.</span><span class="sxs-lookup"><span data-stu-id="9efde-1024">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="9efde-1025">Nube</span><span class="sxs-lookup"><span data-stu-id="9efde-1025">Cloud</span></span>
* <span data-ttu-id="9efde-1026">Se ha corregido un error de "suscripción no encontrada" en `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1026">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1027">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1027">ACR</span></span>
* <span data-ttu-id="9efde-1028">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="9efde-1028">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="9efde-1029">Se ha agregado `--auth-mode` a los comandos `acr build`, `acr run`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1029">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="9efde-1030">Se ha agregado el grupo de comandos "acr task credential" para administrar las credenciales de una tarea.</span><span class="sxs-lookup"><span data-stu-id="9efde-1030">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="9efde-1031">Se ha agregado "--no-wait" al comando `acr build`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1031">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1032">AppService</span></span>
* <span data-ttu-id="9efde-1033">Se ha corregido el error por el que `webapp up` no controlaba correctamente los escenarios de ejecución desde un directorio o de código desconocido.</span><span class="sxs-lookup"><span data-stu-id="9efde-1033">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="9efde-1034">Se ha corregido el error por el que los espacios no funcionaban para `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1034">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="9efde-1035">Servicio BOT</span><span class="sxs-lookup"><span data-stu-id="9efde-1035">BOT Service</span></span>
* <span data-ttu-id="9efde-1036">Se ha agregado `bot prepare-deploy` para preparar la implementación de bots mediante `webapp`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1036">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="9efde-1037">Se ha cambiado `bot create --kind registration` para que muestre la contraseña si no se proporciona una.</span><span class="sxs-lookup"><span data-stu-id="9efde-1037">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="9efde-1038">[CAMBIO IMPORTANTE] Se ha cambiado `--endpoint` en `bot create --kind registration` a que sea una cadena vacía de forma predeterminada en lugar de que sea obligatorio.</span><span class="sxs-lookup"><span data-stu-id="9efde-1038">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="9efde-1039">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="9efde-1039">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-1040">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-1040">CDN</span></span>
* <span data-ttu-id="9efde-1041">Se agregó compatibilidad para `--no-wait` a `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1041">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="9efde-1042">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento de almacenamiento de cadenas de consulta en caché predeterminado de `cdn endpoint create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1042">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="9efde-1043">El valor predeterminado ya no es "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="9efde-1043">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9efde-1044">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="9efde-1044">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-1045">Cosmosdb</span><span class="sxs-lookup"><span data-stu-id="9efde-1045">Cosmosdb</span></span>
* <span data-ttu-id="9efde-1046">Se ha agregado compatibilidad con `--enable-multiple-write-locations` al actualizar la cuenta.</span><span class="sxs-lookup"><span data-stu-id="9efde-1046">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="9efde-1047">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="9efde-1047">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-1048">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-1048">Interactive</span></span>
* <span data-ttu-id="9efde-1049">Se ha corregido la incompatibilidad con la extensión interactiva instalada mediante azdev.</span><span class="sxs-lookup"><span data-stu-id="9efde-1049">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-1050">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1050">Monitor</span></span>
* <span data-ttu-id="9efde-1051">Se ha cambiado para permitir el valor de dimensión `*` para `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1051">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1052">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1052">Network</span></span>
* <span data-ttu-id="9efde-1053">Se ha agregado el grupo de comandos `rewrite-rule` a `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1053">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-1054">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-1054">Profile</span></span>
* <span data-ttu-id="9efde-1055">Se ha agregado a `login` compatibilidad de la cuenta en el nivel de inquilino para la identidad de servicio administrada.</span><span class="sxs-lookup"><span data-stu-id="9efde-1055">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="9efde-1056">Postgres</span><span class="sxs-lookup"><span data-stu-id="9efde-1056">Postgres</span></span> 
* <span data-ttu-id="9efde-1057">Se han agregado los comandos postgresql `replica` y el comando `restart server`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1057">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="9efde-1058">Se ha cambiado para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="9efde-1058">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1059">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1059">Resource</span></span>
* <span data-ttu-id="9efde-1060">Se ha mejorado la salida de tabla de `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1060">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="9efde-1061">Se ha corregido el problema con `deployment [create|validate]` por el que no reconocía el tipo secureObject.</span><span class="sxs-lookup"><span data-stu-id="9efde-1061">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="9efde-1062">Grafo</span><span class="sxs-lookup"><span data-stu-id="9efde-1062">Graph</span></span>
* <span data-ttu-id="9efde-1063">Se agregó compatibilidad para `--end-date` a `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1063">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="9efde-1064">Se ha agregado compatibilidad para agregar permisos con `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1064">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="9efde-1065">Se ha corregido un error con `ad app permission list` cuando no había ningún permiso.</span><span class="sxs-lookup"><span data-stu-id="9efde-1065">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="9efde-1066">Se ha cambiado `ad sp delete` para omitir la eliminación de la asignación de roles si la cuenta actual no tiene ninguna suscripción.</span><span class="sxs-lookup"><span data-stu-id="9efde-1066">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="9efde-1067">Se ha cambiado `ad app create` para que `--identifier-uris` sea una lista vacía de forma predeterminada si no se proporciona.</span><span class="sxs-lookup"><span data-stu-id="9efde-1067">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1068">storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1068">storage</span></span>
* <span data-ttu-id="9efde-1069">Se ha agregado `--snapshot` a `storage file download-batch` para descargar desde una instantánea de recurso compartido.</span><span class="sxs-lookup"><span data-stu-id="9efde-1069">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="9efde-1070">Se ha cambiado la barra de progreso `storage blob [download-batch|upload-batch]` para que sea menos detallada y que indique el blob actual.</span><span class="sxs-lookup"><span data-stu-id="9efde-1070">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="9efde-1071">Se ha corregido el problema con `storage account update` al actualizar los parámetros de cifrado.</span><span class="sxs-lookup"><span data-stu-id="9efde-1071">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="9efde-1072">Se ha corregido el problema por el que `storage blob show` producía un error al usar oauth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="9efde-1072">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1073">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1073">VM</span></span>
* <span data-ttu-id="9efde-1074">Se agregó el comando `image update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1074">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="9efde-1075">12 de marzo de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-1075">March 12, 2019</span></span>

<span data-ttu-id="9efde-1076">Versión 2.0.60</span><span class="sxs-lookup"><span data-stu-id="9efde-1076">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1077">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1077">Core</span></span>

* <span data-ttu-id="9efde-1078">Se ha corregido un error incorrecto en `cloud set` sobre la suscripción no encontrada.</span><span class="sxs-lookup"><span data-stu-id="9efde-1078">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1079">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1079">ACR</span></span>

* <span data-ttu-id="9efde-1080">Se han corregido orígenes redundantes en la importación de imágenes.</span><span class="sxs-lookup"><span data-stu-id="9efde-1080">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1081">ACS</span></span>

* <span data-ttu-id="9efde-1082">Ahora, se omite el parámetro `--listen-address` de `aks browse` si kubectl no lo admite</span><span class="sxs-lookup"><span data-stu-id="9efde-1082">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="9efde-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1083">AppService</span></span>

* <span data-ttu-id="9efde-1084">Se ha agregado `[webapp|functionapp] deployment list-publishing-credentials` para obtener la dirección URL y sus credenciales de publicación de Kudu.</span><span class="sxs-lookup"><span data-stu-id="9efde-1084">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="9efde-1085">Se ha quitado la instrucción de impresión errónea para `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1085">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="9efde-1086">Se ha corregido `functionapp` para establecer la imagen correcta en el entorno de ejecución en los planes de App Service de Linux</span><span class="sxs-lookup"><span data-stu-id="9efde-1086">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="9efde-1087">Se ha quitado la etiqueta de versión preliminar para `webapp up` y se han agregado mejoras al comando.</span><span class="sxs-lookup"><span data-stu-id="9efde-1087">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-1088">Botservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1088">Botservice</span></span>

* <span data-ttu-id="9efde-1089">Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.</span><span class="sxs-lookup"><span data-stu-id="9efde-1089">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9efde-1090">Se han agregado `Microsoft-BotFramework-AppId` y `Microsoft-BotFramework-AppPassword` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web</span><span class="sxs-lookup"><span data-stu-id="9efde-1090">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="9efde-1091">Se han quitado las comillas simples de la salida del comando `bot publish` al final de `bot create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1091">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="9efde-1092">Se ha cambiado `bot publish` para que sea asincrónico.</span><span class="sxs-lookup"><span data-stu-id="9efde-1092">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1093">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1093">Container</span></span>

* <span data-ttu-id="9efde-1094">Se agregó el argumento `--no-wait` a `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1094">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="9efde-1095">EventHub</span><span class="sxs-lookup"><span data-stu-id="9efde-1095">EventHub</span></span>

* <span data-ttu-id="9efde-1096">Se ha agregado la marca `--skip-empty-archives` a `eventhub create|update` para admitir archivos vacíos en la captura.</span><span class="sxs-lookup"><span data-stu-id="9efde-1096">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="9efde-1097">Buscar</span><span class="sxs-lookup"><span data-stu-id="9efde-1097">Find</span></span>

* <span data-ttu-id="9efde-1098">Actualización de la funcionalidad principal</span><span class="sxs-lookup"><span data-stu-id="9efde-1098">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-1099">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-1099">HDInsight</span></span>

* <span data-ttu-id="9efde-1100">Se ha agregado el parámetro `--storage-account-managed-identity` a `hdinsight create` para admitir MSI de ADLS Gen2.</span><span class="sxs-lookup"><span data-stu-id="9efde-1100">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1101">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1101">Network</span></span>

* <span data-ttu-id="9efde-1102">Se ha corregido un problema con `vpn-connection update` por el que no se podía actualizar una conexión VPN entre pasarelas de diferentes suscripciones.</span><span class="sxs-lookup"><span data-stu-id="9efde-1102">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-1103">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9efde-1103">Rdbms</span></span>

* <span data-ttu-id="9efde-1104">Correcciones menores para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.</span><span class="sxs-lookup"><span data-stu-id="9efde-1104">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1105">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1105">Role</span></span>

* <span data-ttu-id="9efde-1106">Se ha corregido `role definition update` para usar el identificador para resolver la definición correctamente.</span><span class="sxs-lookup"><span data-stu-id="9efde-1106">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="9efde-1107">Se ha cambiado `ad app credential reset` para eliminar la suposición de que la entidad de servicio de la aplicación siempre existe.</span><span class="sxs-lookup"><span data-stu-id="9efde-1107">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9efde-1108">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9efde-1108">Service Fabric</span></span>

* <span data-ttu-id="9efde-1109">Se ha corregido un problema con `sf cluster list` que no se podía iterar.</span><span class="sxs-lookup"><span data-stu-id="9efde-1109">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="9efde-1110">26 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-1110">February 26, 2019</span></span>

<span data-ttu-id="9efde-1111">Versión 2.0.59</span><span class="sxs-lookup"><span data-stu-id="9efde-1111">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1112">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1112">Core</span></span>

* <span data-ttu-id="9efde-1113">Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.</span><span class="sxs-lookup"><span data-stu-id="9efde-1113">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1114">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1114">ACR</span></span>

* <span data-ttu-id="9efde-1115">Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1115">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="9efde-1116">Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.</span><span class="sxs-lookup"><span data-stu-id="9efde-1116">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1117">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1117">ACS</span></span>

* <span data-ttu-id="9efde-1118">Se agregó la opción `--listen-address` a `aks port-forward`</span><span class="sxs-lookup"><span data-stu-id="9efde-1118">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1119">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1119">AppService</span></span>

* <span data-ttu-id="9efde-1120">Se agregó el comando `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1120">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-1121">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-1121">Batch</span></span>
* <span data-ttu-id="9efde-1122">[CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1122">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="9efde-1123">[CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1123">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="9efde-1124">Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.</span><span class="sxs-lookup"><span data-stu-id="9efde-1124">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="9efde-1125">[CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1125">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="9efde-1126">Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.</span><span class="sxs-lookup"><span data-stu-id="9efde-1126">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="9efde-1127">Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.</span><span class="sxs-lookup"><span data-stu-id="9efde-1127">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-1128">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-1128">CosmosDB</span></span>

* <span data-ttu-id="9efde-1129">Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="9efde-1129">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="9efde-1130">Kusto</span><span class="sxs-lookup"><span data-stu-id="9efde-1130">Kusto</span></span>

* <span data-ttu-id="9efde-1131">[CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.</span><span class="sxs-lookup"><span data-stu-id="9efde-1131">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1132">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1132">Network</span></span>

* <span data-ttu-id="9efde-1133">Se agregó el argumento `--express-route-gateway-bypass` a `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1133">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="9efde-1134">Se han agregado grupos de comandos desde extensiones `express-route`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1134">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="9efde-1135">Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1135">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="9efde-1136">Se agregó el argumento `--legacy-mode` a `express-route peering [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1136">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="9efde-1137">Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1137">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="9efde-1138">Se agregó el argumento `--gateway-default-site` a `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1138">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="9efde-1139">Se han agregado comandos `ipsec-policy` a `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1139">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1140">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1140">Resource</span></span>

* <span data-ttu-id="9efde-1141">Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9efde-1141">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="9efde-1142">Se ha agregado compatibilidad para el archivo de parámetros basado en URI a `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1142">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="9efde-1143">Se ha agregado compatibilidad para definiciones y parámetros basados en URI para `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1143">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="9efde-1144">Se ha corregido el control de parámetros y reglas para `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1144">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="9efde-1145">Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.</span><span class="sxs-lookup"><span data-stu-id="9efde-1145">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1146">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1146">Role</span></span>

* <span data-ttu-id="9efde-1147">Se ha agregado compatibilidad con roles de aplicación a `ad app [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1147">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1148">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1148">VM</span></span>

* <span data-ttu-id="9efde-1149">Se ha corregido un problema con `vm create where `--acelerated-networking\` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-1149">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="9efde-1150">12 de febrero de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-1150">February 12, 2019</span></span>

<span data-ttu-id="9efde-1151">Versión 2.0.58</span><span class="sxs-lookup"><span data-stu-id="9efde-1151">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1152">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1152">Core</span></span>

* <span data-ttu-id="9efde-1153">`az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.</span><span class="sxs-lookup"><span data-stu-id="9efde-1153">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="9efde-1154">Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.</span><span class="sxs-lookup"><span data-stu-id="9efde-1154">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1155">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1155">ACR</span></span>
* <span data-ttu-id="9efde-1156">[CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1156">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="9efde-1157">[CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1157">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1158">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1158">ACS</span></span>
* <span data-ttu-id="9efde-1159">Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.</span><span class="sxs-lookup"><span data-stu-id="9efde-1159">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="9efde-1160">Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1160">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="9efde-1161">Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1161">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-1162">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-1162">AMS</span></span>
* <span data-ttu-id="9efde-1163">Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1163">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="9efde-1164">Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1164">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1165">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1165">Appservice</span></span>
* <span data-ttu-id="9efde-1166">Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.</span><span class="sxs-lookup"><span data-stu-id="9efde-1166">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="9efde-1167">Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.</span><span class="sxs-lookup"><span data-stu-id="9efde-1167">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="9efde-1168">Se ha mejorado la ayuda de `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1168">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="9efde-1169">Se ha agregado compatibilidad para App Insights al crear una aplicación de función.</span><span class="sxs-lookup"><span data-stu-id="9efde-1169">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="9efde-1170">Se han corregido los problemas de SSH con las aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="9efde-1170">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-1171">Botservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1171">Botservice</span></span>
* <span data-ttu-id="9efde-1172">Se ha mejorado la experiencia de usuario de `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1172">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="9efde-1173">Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1173">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="9efde-1174">Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1174">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="9efde-1175">Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.</span><span class="sxs-lookup"><span data-stu-id="9efde-1175">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="9efde-1176">[EN DESUSO] Se ha dejado de utilizar el argumento `--proj-name` en favor de `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1176">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="9efde-1177">Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.</span><span class="sxs-lookup"><span data-stu-id="9efde-1177">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="9efde-1178">Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.</span><span class="sxs-lookup"><span data-stu-id="9efde-1178">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="9efde-1179">Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.</span><span class="sxs-lookup"><span data-stu-id="9efde-1179">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="9efde-1180">El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.</span><span class="sxs-lookup"><span data-stu-id="9efde-1180">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="9efde-1181">Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.</span><span class="sxs-lookup"><span data-stu-id="9efde-1181">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-1182">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-1182">Key Vault</span></span>
* <span data-ttu-id="9efde-1183">Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1183">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-1184">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1184">Monitor</span></span>
* <span data-ttu-id="9efde-1185">Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1185">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1186">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1186">Network</span></span>
* <span data-ttu-id="9efde-1187">Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1187">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="9efde-1188">Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="9efde-1188">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="9efde-1189">Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="9efde-1189">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="9efde-1190">Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1190">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9efde-1191">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-1191">Policy Insights</span></span>
* <span data-ttu-id="9efde-1192">Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1192">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-1193">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-1193">RDBMS</span></span>
* <span data-ttu-id="9efde-1194">Se han mejorado los parámetros de mensajes y comandos de ayuda.</span><span class="sxs-lookup"><span data-stu-id="9efde-1194">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="9efde-1195">Redis</span><span class="sxs-lookup"><span data-stu-id="9efde-1195">Redis</span></span>
* <span data-ttu-id="9efde-1196">Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="9efde-1196">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="9efde-1197">Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).</span><span class="sxs-lookup"><span data-stu-id="9efde-1197">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="9efde-1198">Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).</span><span class="sxs-lookup"><span data-stu-id="9efde-1198">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="9efde-1199">Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".</span><span class="sxs-lookup"><span data-stu-id="9efde-1199">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="9efde-1200">[CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1200">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="9efde-1201">[CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].</span><span class="sxs-lookup"><span data-stu-id="9efde-1201">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="9efde-1202">[EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1202">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1203">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1203">Role</span></span>
* <span data-ttu-id="9efde-1204">[CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1204">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="9efde-1205">VM con SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1205">SQL VM</span></span>
* <span data-ttu-id="9efde-1206">[EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.</span><span class="sxs-lookup"><span data-stu-id="9efde-1206">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1207">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1207">VM</span></span>
* <span data-ttu-id="9efde-1208">Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1208">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="9efde-1209">Se agregó `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1209">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="9efde-1210">Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.</span><span class="sxs-lookup"><span data-stu-id="9efde-1210">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="9efde-1211">[CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1211">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="9efde-1212">31 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-1212">January 31, 2019</span></span>

<span data-ttu-id="9efde-1213">Versión 2.0.57</span><span class="sxs-lookup"><span data-stu-id="9efde-1213">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1214">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1214">Core</span></span>

* <span data-ttu-id="9efde-1215">Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="9efde-1215">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="9efde-1216">28 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-1216">January 28, 2019</span></span>

<span data-ttu-id="9efde-1217">Versión 2.0.56</span><span class="sxs-lookup"><span data-stu-id="9efde-1217">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1218">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1218">ACR</span></span>
* <span data-ttu-id="9efde-1219">Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.</span><span class="sxs-lookup"><span data-stu-id="9efde-1219">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1220">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1220">ACS</span></span>
* <span data-ttu-id="9efde-1221">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="9efde-1221">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9efde-1222">Se han agregado comandos OpenShift administrados.</span><span class="sxs-lookup"><span data-stu-id="9efde-1222">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="9efde-1223">Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1223">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-1224">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-1224">AMS</span></span>
* <span data-ttu-id="9efde-1225">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`</span><span class="sxs-lookup"><span data-stu-id="9efde-1225">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="9efde-1226">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`</span><span class="sxs-lookup"><span data-stu-id="9efde-1226">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1227">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1227">Appservice</span></span>
* <span data-ttu-id="9efde-1228">Se ha agregado compatibilidad para App Insights en `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1228">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="9efde-1229">Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).</span><span class="sxs-lookup"><span data-stu-id="9efde-1229">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="9efde-1230">Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.</span><span class="sxs-lookup"><span data-stu-id="9efde-1230">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1231">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1231">Container</span></span>
* <span data-ttu-id="9efde-1232">Se agregó el comando `container start`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1232">Added `container start` command</span></span>
* <span data-ttu-id="9efde-1233">Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.</span><span class="sxs-lookup"><span data-stu-id="9efde-1233">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9efde-1234">EventGrid</span><span class="sxs-lookup"><span data-stu-id="9efde-1234">EventGrid</span></span>
* <span data-ttu-id="9efde-1235">Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1235">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="9efde-1236">Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".</span><span class="sxs-lookup"><span data-stu-id="9efde-1236">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="9efde-1237">Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1237">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="9efde-1238">Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1238">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="9efde-1239">Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.</span><span class="sxs-lookup"><span data-stu-id="9efde-1239">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-1240">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-1240">HDInsight</span></span>
* <span data-ttu-id="9efde-1241">[CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1241">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="9efde-1242">[CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.</span><span class="sxs-lookup"><span data-stu-id="9efde-1242">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="9efde-1243">Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1243">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="9efde-1244">Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1244">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="9efde-1245">Se agregó el comando `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1245">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="9efde-1246">Se agregó el comando `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1246">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-1247">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-1247">IoT</span></span>
* <span data-ttu-id="9efde-1248">Se ha agregado un formato de codificación al comando routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="9efde-1248">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="9efde-1249">Kusto</span><span class="sxs-lookup"><span data-stu-id="9efde-1249">Kusto</span></span>
* <span data-ttu-id="9efde-1250">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-1250">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-1251">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1251">Monitor</span></span>
* <span data-ttu-id="9efde-1252">Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9efde-1252">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-1253">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-1253">Profile</span></span>
* <span data-ttu-id="9efde-1254">Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1254">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1255">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1255">Network</span></span>
* <span data-ttu-id="9efde-1256">Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1256">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="9efde-1257">Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.</span><span class="sxs-lookup"><span data-stu-id="9efde-1257">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1258">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1258">Resource</span></span>
* <span data-ttu-id="9efde-1259">Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1259">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="9efde-1260">Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1260">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="9efde-1261">Máquina virtual SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1261">SQL Virtual Machine</span></span>
* <span data-ttu-id="9efde-1262">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-1262">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1263">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1263">Storage</span></span>
* <span data-ttu-id="9efde-1264">Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.</span><span class="sxs-lookup"><span data-stu-id="9efde-1264">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="9efde-1265">Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.</span><span class="sxs-lookup"><span data-stu-id="9efde-1265">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1266">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1266">VM</span></span>
* <span data-ttu-id="9efde-1267">Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.</span><span class="sxs-lookup"><span data-stu-id="9efde-1267">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="9efde-1268">Se ha agregado la marca `--force` a `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1268">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="9efde-1269">15 de enero de 2019</span><span class="sxs-lookup"><span data-stu-id="9efde-1269">January 15, 2019</span></span>

<span data-ttu-id="9efde-1270">Versión 2.0.55</span><span class="sxs-lookup"><span data-stu-id="9efde-1270">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1271">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1271">ACR</span></span>
* <span data-ttu-id="9efde-1272">Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.</span><span class="sxs-lookup"><span data-stu-id="9efde-1272">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="9efde-1273">Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.</span><span class="sxs-lookup"><span data-stu-id="9efde-1273">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="9efde-1274">[EN DESUSO] Se ha dejado de usar el parámetro `--resource-group` en los comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-1274">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="9efde-1275">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1275">ACS</span></span>
* <span data-ttu-id="9efde-1276">Se ha agregado compatibilidad para nuevas regiones de ACI.</span><span class="sxs-lookup"><span data-stu-id="9efde-1276">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1277">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1277">Appservice</span></span>
* <span data-ttu-id="9efde-1278">Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.</span><span class="sxs-lookup"><span data-stu-id="9efde-1278">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="9efde-1279">Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.</span><span class="sxs-lookup"><span data-stu-id="9efde-1279">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="9efde-1280">Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación.</span><span class="sxs-lookup"><span data-stu-id="9efde-1280">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="9efde-1281">Se agregó el comando `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1281">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-1282">Botservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1282">Botservice</span></span>
* <span data-ttu-id="9efde-1283">Se han agregado actualizaciones al estado de implementación a `bot create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1283">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="9efde-1284">Configuración</span><span class="sxs-lookup"><span data-stu-id="9efde-1284">Configure</span></span>
* <span data-ttu-id="9efde-1285">Se ha agregado `none` como formato de salida configurable.</span><span class="sxs-lookup"><span data-stu-id="9efde-1285">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-1286">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-1286">CosmosDB</span></span>
* <span data-ttu-id="9efde-1287">Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.</span><span class="sxs-lookup"><span data-stu-id="9efde-1287">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-1288">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-1288">HDInsight</span></span>
* <span data-ttu-id="9efde-1289">Se han agregado comandos para administrar aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="9efde-1289">Added commands for managing applications</span></span>
* <span data-ttu-id="9efde-1290">Se han agregado comandos para administrar acciones de script.</span><span class="sxs-lookup"><span data-stu-id="9efde-1290">Added commands for managing script actions</span></span>
* <span data-ttu-id="9efde-1291">Se han agregado comandos para administrar Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="9efde-1291">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="9efde-1292">Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1292">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="9efde-1293">[CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1293">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1294">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1294">Network</span></span>
* <span data-ttu-id="9efde-1295">Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1295">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="9efde-1296">Se han agregado nuevos tipos enrutamientos: subred y multivalor.</span><span class="sxs-lookup"><span data-stu-id="9efde-1296">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="9efde-1297">Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1297">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="9efde-1298">Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1298">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1299">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1299">Role</span></span>
* <span data-ttu-id="9efde-1300">[EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1300">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="9efde-1301">En su lugar, use contraseñas seguras generadas por la CLI.</span><span class="sxs-lookup"><span data-stu-id="9efde-1301">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="9efde-1302">Seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-1302">Security</span></span>
* <span data-ttu-id="9efde-1303">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-1303">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1304">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1304">Storage</span></span>
* <span data-ttu-id="9efde-1305">[CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000.</span><span class="sxs-lookup"><span data-stu-id="9efde-1305">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="9efde-1306">Use `--num-results *` para el comportamiento original de devolver todos los resultados.</span><span class="sxs-lookup"><span data-stu-id="9efde-1306">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="9efde-1307">Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`</span><span class="sxs-lookup"><span data-stu-id="9efde-1307">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="9efde-1308">Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1308">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="9efde-1309">Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1309">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1310">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1310">VM</span></span>
* <span data-ttu-id="9efde-1311">Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.</span><span class="sxs-lookup"><span data-stu-id="9efde-1311">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="9efde-1312">Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1312">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9efde-1313">Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1313">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="9efde-1314">Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.</span><span class="sxs-lookup"><span data-stu-id="9efde-1314">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="9efde-1315">Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.</span><span class="sxs-lookup"><span data-stu-id="9efde-1315">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="9efde-1316">Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.</span><span class="sxs-lookup"><span data-stu-id="9efde-1316">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="9efde-1317">20 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1317">December 20, 2018</span></span>

<span data-ttu-id="9efde-1318">Versión 2.0.54</span><span class="sxs-lookup"><span data-stu-id="9efde-1318">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="9efde-1319">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1319">Appservice</span></span>
* <span data-ttu-id="9efde-1320">Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.</span><span class="sxs-lookup"><span data-stu-id="9efde-1320">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="9efde-1321">Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.</span><span class="sxs-lookup"><span data-stu-id="9efde-1321">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="9efde-1322">Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.</span><span class="sxs-lookup"><span data-stu-id="9efde-1322">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9efde-1323">IoTCentral</span><span class="sxs-lookup"><span data-stu-id="9efde-1323">IoTCentral</span></span>
* <span data-ttu-id="9efde-1324">Se ha corregido la actualización de la llamada API del comando</span><span class="sxs-lookup"><span data-stu-id="9efde-1324">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1325">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1325">Role</span></span>
* <span data-ttu-id="9efde-1326">[CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9efde-1326">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-1327">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1327">SQL</span></span>
* <span data-ttu-id="9efde-1328">Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.</span><span class="sxs-lookup"><span data-stu-id="9efde-1328">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1329">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1329">VM</span></span>
* <span data-ttu-id="9efde-1330">Se ha agregado el parámetro `---os-type` a `disk create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1330">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="9efde-1331">18 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1331">December 18, 2018</span></span>

<span data-ttu-id="9efde-1332">Versión 2.0.53</span><span class="sxs-lookup"><span data-stu-id="9efde-1332">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="9efde-1333">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1333">ACR</span></span>
* <span data-ttu-id="9efde-1334">Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.</span><span class="sxs-lookup"><span data-stu-id="9efde-1334">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="9efde-1335">Se ha comprimido el diseño de tabla para la lista de tareas.</span><span class="sxs-lookup"><span data-stu-id="9efde-1335">Condensed the table layout for task list</span></span>
* <span data-ttu-id="9efde-1336">Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="9efde-1336">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1337">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1337">ACS</span></span>
* <span data-ttu-id="9efde-1338">Se ha agregado la versión preliminar de nodos virtuales.</span><span class="sxs-lookup"><span data-stu-id="9efde-1338">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="9efde-1339">Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1339">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="9efde-1340">[EN DESUSO] Se han dejado de usar los comandos `az acs`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1340">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="9efde-1341">El servicio de ACS se retirará el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="9efde-1341">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="9efde-1342">Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.</span><span class="sxs-lookup"><span data-stu-id="9efde-1342">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="9efde-1343">Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.</span><span class="sxs-lookup"><span data-stu-id="9efde-1343">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1344">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1344">Appservice</span></span>
* <span data-ttu-id="9efde-1345">Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1345">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="9efde-1346">Botservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1346">Botservice</span></span>
* <span data-ttu-id="9efde-1347">Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1347">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="9efde-1348">Se ha corregido el error de aprovisionamiento de AppInsights.</span><span class="sxs-lookup"><span data-stu-id="9efde-1348">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="9efde-1349">Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.</span><span class="sxs-lookup"><span data-stu-id="9efde-1349">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="9efde-1350">Se han reducido las llamadas de red de Kudu.</span><span class="sxs-lookup"><span data-stu-id="9efde-1350">Reduced Kudu network calls</span></span>
* <span data-ttu-id="9efde-1351">Se ha mejorado la experiencia de usuario de comandos generales.</span><span class="sxs-lookup"><span data-stu-id="9efde-1351">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="9efde-1352">Consumo</span><span class="sxs-lookup"><span data-stu-id="9efde-1352">Consumption</span></span>
* <span data-ttu-id="9efde-1353">Se han corregido errores para que la API de presupuesto muestre notificaciones.</span><span class="sxs-lookup"><span data-stu-id="9efde-1353">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-1354">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-1354">CosmosDB</span></span>
* <span data-ttu-id="9efde-1355">Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.</span><span class="sxs-lookup"><span data-stu-id="9efde-1355">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="9efde-1356">Mapas</span><span class="sxs-lookup"><span data-stu-id="9efde-1356">Maps</span></span>
* <span data-ttu-id="9efde-1357">Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1357">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1358">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1358">Network</span></span>
* <span data-ttu-id="9efde-1359">Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`</span><span class="sxs-lookup"><span data-stu-id="9efde-1359">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="9efde-1360">Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.</span><span class="sxs-lookup"><span data-stu-id="9efde-1360">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1361">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1361">Resource</span></span>
* <span data-ttu-id="9efde-1362">Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1362">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="9efde-1363">Se ha agregado un nuevo comando `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1363">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1364">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1364">Storage</span></span>
*  <span data-ttu-id="9efde-1365">Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1365">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1366">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1366">VM</span></span>
* <span data-ttu-id="9efde-1367">Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.</span><span class="sxs-lookup"><span data-stu-id="9efde-1367">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="9efde-1368">4 de diciembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1368">December 4, 2018</span></span>

<span data-ttu-id="9efde-1369">Versión 2.0.52</span><span class="sxs-lookup"><span data-stu-id="9efde-1369">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="9efde-1370">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1370">Core</span></span>
* <span data-ttu-id="9efde-1371">Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino</span><span class="sxs-lookup"><span data-stu-id="9efde-1371">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="9efde-1372">Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente</span><span class="sxs-lookup"><span data-stu-id="9efde-1372">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1373">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1373">Appservice</span></span>
* <span data-ttu-id="9efde-1374">[VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación</span><span class="sxs-lookup"><span data-stu-id="9efde-1374">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="9efde-1375">Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end</span><span class="sxs-lookup"><span data-stu-id="9efde-1375">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1376">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1376">Network</span></span>
* <span data-ttu-id="9efde-1377">Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF</span><span class="sxs-lookup"><span data-stu-id="9efde-1377">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1378">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1378">Role</span></span>
* <span data-ttu-id="9efde-1379">Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña</span><span class="sxs-lookup"><span data-stu-id="9efde-1379">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="9efde-1380">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1380">VM</span></span>
* <span data-ttu-id="9efde-1381">[EN DESUSO] Se ha dejado de usar el parámetro `vm extension [show|wait] --expand`</span><span class="sxs-lookup"><span data-stu-id="9efde-1381">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="9efde-1382">Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden</span><span class="sxs-lookup"><span data-stu-id="9efde-1382">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="9efde-1383">Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH</span><span class="sxs-lookup"><span data-stu-id="9efde-1383">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="9efde-1384">Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen</span><span class="sxs-lookup"><span data-stu-id="9efde-1384">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="9efde-1385">20 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1385">November 20, 2018</span></span>

<span data-ttu-id="9efde-1386">Versión 2.0.51</span><span class="sxs-lookup"><span data-stu-id="9efde-1386">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="9efde-1387">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1387">Core</span></span>
* <span data-ttu-id="9efde-1388">Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.</span><span class="sxs-lookup"><span data-stu-id="9efde-1388">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1389">ACR</span></span>
* <span data-ttu-id="9efde-1390">Se ha agregado un token de contexto al paso de la tarea.</span><span class="sxs-lookup"><span data-stu-id="9efde-1390">Added context token to task step</span></span>
* <span data-ttu-id="9efde-1391">Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.</span><span class="sxs-lookup"><span data-stu-id="9efde-1391">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="9efde-1392">Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1392">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1393">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-1393">Appservice</span></span>
* <span data-ttu-id="9efde-1394">Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.</span><span class="sxs-lookup"><span data-stu-id="9efde-1394">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="9efde-1395">Se ha actualizado el valor predeterminado `node_version`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1395">Updated the default `node_version`.</span></span> <span data-ttu-id="9efde-1396">El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.</span><span class="sxs-lookup"><span data-stu-id="9efde-1396">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="9efde-1397">Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.</span><span class="sxs-lookup"><span data-stu-id="9efde-1397">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="9efde-1398">Se ha corregido un error al intentar obtener el estado de zipdeploy.</span><span class="sxs-lookup"><span data-stu-id="9efde-1398">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="9efde-1399">IotCentral</span><span class="sxs-lookup"><span data-stu-id="9efde-1399">IotCentral</span></span>
* <span data-ttu-id="9efde-1400">Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central</span><span class="sxs-lookup"><span data-stu-id="9efde-1400">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-1401">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9efde-1401">KeyVault</span></span>
* <span data-ttu-id="9efde-1402">Se ha corregido un error donde se han ignorado los errores.</span><span class="sxs-lookup"><span data-stu-id="9efde-1402">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1403">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1403">Network</span></span>
* <span data-ttu-id="9efde-1404">Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.</span><span class="sxs-lookup"><span data-stu-id="9efde-1404">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="9efde-1405">Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:</span><span class="sxs-lookup"><span data-stu-id="9efde-1405">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="9efde-1406">Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad.</span><span class="sxs-lookup"><span data-stu-id="9efde-1406">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="9efde-1407">Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1407">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-1408">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9efde-1408">Rdbms</span></span>
* <span data-ttu-id="9efde-1409">Se han agregado comandos de red virtual de mariadb.</span><span class="sxs-lookup"><span data-stu-id="9efde-1409">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="9efde-1410">Rbac</span><span class="sxs-lookup"><span data-stu-id="9efde-1410">Rbac</span></span>
* <span data-ttu-id="9efde-1411">Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1411">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="9efde-1412">Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1412">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="9efde-1413">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1413">Storage</span></span>
* <span data-ttu-id="9efde-1414">Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-1414">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="9efde-1415">Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.</span><span class="sxs-lookup"><span data-stu-id="9efde-1415">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="9efde-1416">Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.</span><span class="sxs-lookup"><span data-stu-id="9efde-1416">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="9efde-1417">Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9efde-1417">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1418">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1418">VM</span></span>
* <span data-ttu-id="9efde-1419">Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.</span><span class="sxs-lookup"><span data-stu-id="9efde-1419">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="9efde-1420">Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1420">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="9efde-1421">Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1421">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="9efde-1422">Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1422">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="9efde-1423">Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1423">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="9efde-1424">Se agregó el comando `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1424">Added `snapshot wait` command</span></span>
* <span data-ttu-id="9efde-1425">Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1425">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="9efde-1426">6 de noviembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1426">November 6, 2018</span></span>

<span data-ttu-id="9efde-1427">Versión 2.0.50</span><span class="sxs-lookup"><span data-stu-id="9efde-1427">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1428">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1428">Core</span></span>
* <span data-ttu-id="9efde-1429">Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="9efde-1429">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1430">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1430">ACR</span></span>
* <span data-ttu-id="9efde-1431">Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea</span><span class="sxs-lookup"><span data-stu-id="9efde-1431">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="9efde-1432">Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build</span><span class="sxs-lookup"><span data-stu-id="9efde-1432">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1433">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1433">ACS</span></span>
* <span data-ttu-id="9efde-1434">[CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9efde-1434">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="9efde-1435">Advisor</span><span class="sxs-lookup"><span data-stu-id="9efde-1435">Advisor</span></span>
* <span data-ttu-id="9efde-1436">Versión de disponibilidad general</span><span class="sxs-lookup"><span data-stu-id="9efde-1436">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-1437">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-1437">AMS</span></span>
* <span data-ttu-id="9efde-1438">Se han agregado nuevos grupos de comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-1438">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="9efde-1439">Se han agregado nuevos comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-1439">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="9efde-1440">Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1440">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="9efde-1441">Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-1441">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="9efde-1442">Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`</span><span class="sxs-lookup"><span data-stu-id="9efde-1442">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="9efde-1443">Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`</span><span class="sxs-lookup"><span data-stu-id="9efde-1443">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="9efde-1444">Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url`</span><span class="sxs-lookup"><span data-stu-id="9efde-1444">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="9efde-1445">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`</span><span class="sxs-lookup"><span data-stu-id="9efde-1445">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="9efde-1446">[CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9efde-1446">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="9efde-1447">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`</span><span class="sxs-lookup"><span data-stu-id="9efde-1447">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="9efde-1448">[CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`</span><span class="sxs-lookup"><span data-stu-id="9efde-1448">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="9efde-1449">[CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1449">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="9efde-1450">Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="9efde-1450">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="9efde-1451">Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado</span><span class="sxs-lookup"><span data-stu-id="9efde-1451">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="9efde-1452">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1452">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="9efde-1453">Ahora acepta una lista separada por espacios de recursos en formato "assetName=label".</span><span class="sxs-lookup"><span data-stu-id="9efde-1453">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="9efde-1454">Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="</span><span class="sxs-lookup"><span data-stu-id="9efde-1454">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1455">AppService</span></span>
* <span data-ttu-id="9efde-1456">Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida</span><span class="sxs-lookup"><span data-stu-id="9efde-1456">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="9efde-1457">Configuración</span><span class="sxs-lookup"><span data-stu-id="9efde-1457">Configure</span></span>
* <span data-ttu-id="9efde-1458">Se ha agregado YAML a las opciones de formato de salida</span><span class="sxs-lookup"><span data-stu-id="9efde-1458">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1459">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1459">Container</span></span>
* <span data-ttu-id="9efde-1460">Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML</span><span class="sxs-lookup"><span data-stu-id="9efde-1460">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="9efde-1461">EventHub</span><span class="sxs-lookup"><span data-stu-id="9efde-1461">EventHub</span></span>
* <span data-ttu-id="9efde-1462">Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1462">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-1463">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-1463">Interactive</span></span>
* <span data-ttu-id="9efde-1464">Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico</span><span class="sxs-lookup"><span data-stu-id="9efde-1464">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-1465">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1465">Monitor</span></span>
* <span data-ttu-id="9efde-1466">Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1466">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1467">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1467">Network</span></span>
* <span data-ttu-id="9efde-1468">Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`</span><span class="sxs-lookup"><span data-stu-id="9efde-1468">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="9efde-1469">Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador</span><span class="sxs-lookup"><span data-stu-id="9efde-1469">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="9efde-1470">Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1470">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="9efde-1471">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-1471">Profile</span></span>
* <span data-ttu-id="9efde-1472">Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados</span><span class="sxs-lookup"><span data-stu-id="9efde-1472">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-1473">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-1473">RDBMS</span></span>
* <span data-ttu-id="9efde-1474">Se han agregado los comandos de réplica de mysql</span><span class="sxs-lookup"><span data-stu-id="9efde-1474">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1475">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1475">Resource</span></span>
* <span data-ttu-id="9efde-1476">Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`</span><span class="sxs-lookup"><span data-stu-id="9efde-1476">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1477">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1477">Role</span></span>
* <span data-ttu-id="9efde-1478">Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados</span><span class="sxs-lookup"><span data-stu-id="9efde-1478">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="9efde-1479">Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="9efde-1479">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="9efde-1480">Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD</span><span class="sxs-lookup"><span data-stu-id="9efde-1480">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1481">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1481">Storage</span></span>
* <span data-ttu-id="9efde-1482">Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span><span class="sxs-lookup"><span data-stu-id="9efde-1482">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1483">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1483">VM</span></span>
* <span data-ttu-id="9efde-1484">Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen</span><span class="sxs-lookup"><span data-stu-id="9efde-1484">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="9efde-1485">Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease</span><span class="sxs-lookup"><span data-stu-id="9efde-1485">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="9efde-1486">Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado</span><span class="sxs-lookup"><span data-stu-id="9efde-1486">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="9efde-1487">Se ha cambiado `vm secret format` para requerir la salida json/jsonc.</span><span class="sxs-lookup"><span data-stu-id="9efde-1487">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="9efde-1488">Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado</span><span class="sxs-lookup"><span data-stu-id="9efde-1488">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="9efde-1489">Se ha mejorado la validación de argumentos de `vm create --image`</span><span class="sxs-lookup"><span data-stu-id="9efde-1489">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="9efde-1490">23 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1490">October 23, 2018</span></span>

<span data-ttu-id="9efde-1491">Versión 2.0.49</span><span class="sxs-lookup"><span data-stu-id="9efde-1491">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1492">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1492">Core</span></span>
* <span data-ttu-id="9efde-1493">Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`</span><span class="sxs-lookup"><span data-stu-id="9efde-1493">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="9efde-1494">Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`</span><span class="sxs-lookup"><span data-stu-id="9efde-1494">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1495">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1495">ACR</span></span>
* <span data-ttu-id="9efde-1496">Se ha corregido un problema de codificación de compilación de ACR en Python2</span><span class="sxs-lookup"><span data-stu-id="9efde-1496">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-1497">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-1497">CDN</span></span>
* <span data-ttu-id="9efde-1498">[CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString".</span><span class="sxs-lookup"><span data-stu-id="9efde-1498">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="9efde-1499">Ahora lo establece el servicio</span><span class="sxs-lookup"><span data-stu-id="9efde-1499">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1500">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1500">Container</span></span>
* <span data-ttu-id="9efde-1501">Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"</span><span class="sxs-lookup"><span data-stu-id="9efde-1501">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="9efde-1502">Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-1502">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="9efde-1503">Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos</span><span class="sxs-lookup"><span data-stu-id="9efde-1503">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="9efde-1504">Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-1504">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="9efde-1505">Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="9efde-1505">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="9efde-1506">Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada</span><span class="sxs-lookup"><span data-stu-id="9efde-1506">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="9efde-1507">Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`</span><span class="sxs-lookup"><span data-stu-id="9efde-1507">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-1508">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-1508">CosmosDB</span></span>
* <span data-ttu-id="9efde-1509">Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1509">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-1510">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-1510">Interactive</span></span>
* <span data-ttu-id="9efde-1511">Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros</span><span class="sxs-lookup"><span data-stu-id="9efde-1511">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="9efde-1512">IoT Central</span><span class="sxs-lookup"><span data-stu-id="9efde-1512">IoT Central</span></span>
* <span data-ttu-id="9efde-1513">Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central</span><span class="sxs-lookup"><span data-stu-id="9efde-1513">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="9efde-1514">[CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1</span><span class="sxs-lookup"><span data-stu-id="9efde-1514">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-1515">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1515">Monitor</span></span>
* <span data-ttu-id="9efde-1516">Cambios en `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="9efde-1516">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="9efde-1517">Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="9efde-1517">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="9efde-1518">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="9efde-1518">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9efde-1519">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="9efde-1519">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="9efde-1520">Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`</span><span class="sxs-lookup"><span data-stu-id="9efde-1520">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="9efde-1521">Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas</span><span class="sxs-lookup"><span data-stu-id="9efde-1521">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="9efde-1522">Cambios en `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="9efde-1522">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="9efde-1523">Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente</span><span class="sxs-lookup"><span data-stu-id="9efde-1523">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="9efde-1524">Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos</span><span class="sxs-lookup"><span data-stu-id="9efde-1524">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="9efde-1525">Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1525">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1526">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1526">Network</span></span>
* <span data-ttu-id="9efde-1527">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="9efde-1527">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="9efde-1528">Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC</span><span class="sxs-lookup"><span data-stu-id="9efde-1528">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="9efde-1529">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9efde-1529">ServiceBus</span></span>
* <span data-ttu-id="9efde-1530">Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium</span><span class="sxs-lookup"><span data-stu-id="9efde-1530">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-1531">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1531">SQL</span></span>
* <span data-ttu-id="9efde-1532">Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual</span><span class="sxs-lookup"><span data-stu-id="9efde-1532">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1533">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1533">Storage</span></span>
* <span data-ttu-id="9efde-1534">Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta</span><span class="sxs-lookup"><span data-stu-id="9efde-1534">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="9efde-1535">Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad</span><span class="sxs-lookup"><span data-stu-id="9efde-1535">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1536">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1536">VM</span></span>
* <span data-ttu-id="9efde-1537">Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1537">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="9efde-1538">Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1538">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="9efde-1539">Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1539">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="9efde-1540">16 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1540">October 16, 2018</span></span>

<span data-ttu-id="9efde-1541">Versión 2.0.48</span><span class="sxs-lookup"><span data-stu-id="9efde-1541">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1542">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1542">VM</span></span>
* <span data-ttu-id="9efde-1543">Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="9efde-1543">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="9efde-1544">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1544">October 9, 2018</span></span>

<span data-ttu-id="9efde-1545">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="9efde-1545">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1546">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1546">Core</span></span>
* <span data-ttu-id="9efde-1547">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="9efde-1547">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1548">ACR</span></span>
* <span data-ttu-id="9efde-1549">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="9efde-1549">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1550">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1550">ACS</span></span>
* <span data-ttu-id="9efde-1551">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="9efde-1551">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="9efde-1552">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="9efde-1552">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="9efde-1553">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="9efde-1553">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="9efde-1554">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="9efde-1554">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1555">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1555">Container</span></span>
* <span data-ttu-id="9efde-1556">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="9efde-1556">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="9efde-1557">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="9efde-1557">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="9efde-1558">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="9efde-1558">Event Hub</span></span>
* <span data-ttu-id="9efde-1559">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="9efde-1559">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="9efde-1560">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="9efde-1560">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="9efde-1561">Extensiones</span><span class="sxs-lookup"><span data-stu-id="9efde-1561">Extensions</span></span>
* <span data-ttu-id="9efde-1562">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="9efde-1562">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="9efde-1563">HDInsight</span><span class="sxs-lookup"><span data-stu-id="9efde-1563">HDInsight</span></span>
* <span data-ttu-id="9efde-1564">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-1564">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-1565">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-1565">IoT</span></span>
* <span data-ttu-id="9efde-1566">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="9efde-1566">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-1567">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9efde-1567">KeyVault</span></span>
* <span data-ttu-id="9efde-1568">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="9efde-1568">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1569">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1569">Network</span></span>
* <span data-ttu-id="9efde-1570">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9efde-1570">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="9efde-1571">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="9efde-1571">See #6052</span></span>
* <span data-ttu-id="9efde-1572">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1572">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="9efde-1573">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="9efde-1573">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="9efde-1574">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9efde-1574">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="9efde-1575">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="9efde-1575">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="9efde-1576">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="9efde-1576">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="9efde-1577">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="9efde-1577">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1578">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1578">Role</span></span>
* <span data-ttu-id="9efde-1579">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="9efde-1579">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="9efde-1580">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="9efde-1580">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="9efde-1581">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="9efde-1581">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="9efde-1582">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="9efde-1582">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="9efde-1583">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9efde-1583">Service Bus</span></span>
* <span data-ttu-id="9efde-1584">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="9efde-1584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1585">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1585">VM</span></span>
* <span data-ttu-id="9efde-1586">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="9efde-1586">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="9efde-1587">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="9efde-1587">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="9efde-1588">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="9efde-1588">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="9efde-1589">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="9efde-1589">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="9efde-1590">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="9efde-1590">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="9efde-1591">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="9efde-1591">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="9efde-1592">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1592">September 21, 2018</span></span>

<span data-ttu-id="9efde-1593">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="9efde-1593">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1594">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1594">ACR</span></span>
* <span data-ttu-id="9efde-1595">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1595">Added ACR Task commands</span></span>
* <span data-ttu-id="9efde-1596">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="9efde-1596">Added quick run command</span></span>
* <span data-ttu-id="9efde-1597">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="9efde-1597">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="9efde-1598">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1598">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="9efde-1599">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="9efde-1599">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="9efde-1600">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="9efde-1600">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1601">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1601">ACS</span></span>
* <span data-ttu-id="9efde-1602">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-1602">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="9efde-1603">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="9efde-1603">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1604">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1604">AppService</span></span>

* <span data-ttu-id="9efde-1605">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="9efde-1605">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="9efde-1606">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="9efde-1606">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="9efde-1607">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="9efde-1607">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="9efde-1608">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="9efde-1608">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-1609">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-1609">Batch</span></span>
* <span data-ttu-id="9efde-1610">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="9efde-1610">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="9efde-1611">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="9efde-1611">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="9efde-1612">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1612">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="9efde-1613">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="9efde-1613">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9efde-1614">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9efde-1614">Batch AI</span></span> 
* <span data-ttu-id="9efde-1615">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1615">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9efde-1616">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9efde-1616">Cognitive Services</span></span>
* <span data-ttu-id="9efde-1617">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="9efde-1617">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="9efde-1618">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="9efde-1618">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="9efde-1619">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="9efde-1619">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="9efde-1620">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="9efde-1620">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="9efde-1621">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-1621">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="9efde-1622">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="9efde-1622">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1623">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1623">Container</span></span>
* <span data-ttu-id="9efde-1624">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="9efde-1624">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="9efde-1625">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="9efde-1625">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="9efde-1626">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1626">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="9efde-1627">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-1627">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="9efde-1628">DataLake</span><span class="sxs-lookup"><span data-stu-id="9efde-1628">Datalake</span></span>
* <span data-ttu-id="9efde-1629">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1629">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="9efde-1630">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="9efde-1630">Interactive Shell</span></span>
* <span data-ttu-id="9efde-1631">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="9efde-1631">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="9efde-1632">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="9efde-1632">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-1633">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-1633">IoT</span></span>
* <span data-ttu-id="9efde-1634">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-1634">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-1635">Key Vault</span><span class="sxs-lookup"><span data-stu-id="9efde-1635">Key Vault</span></span>
* <span data-ttu-id="9efde-1636">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="9efde-1636">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1637">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1637">Network</span></span>
* <span data-ttu-id="9efde-1638">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="9efde-1638">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="9efde-1639">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="9efde-1639">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="9efde-1640">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="9efde-1640">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="9efde-1641">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="9efde-1641">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="9efde-1642">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="9efde-1642">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="9efde-1643">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="9efde-1643">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="9efde-1644">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="9efde-1644">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="9efde-1645">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="9efde-1645">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="9efde-1646">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="9efde-1646">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="9efde-1647">`network express-route create/update`: Se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="9efde-1647">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="9efde-1648">`network vnet subnet create/update`: se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="9efde-1648">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="9efde-1649">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1649">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="9efde-1650">`network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="9efde-1650">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="9efde-1651">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="9efde-1651">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="9efde-1652">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="9efde-1652">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="9efde-1653">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="9efde-1653">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="9efde-1654">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="9efde-1654">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="9efde-1655">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="9efde-1655">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-1656">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-1656">RDBMS</span></span>
* <span data-ttu-id="9efde-1657">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="9efde-1657">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="9efde-1658">Reserva</span><span class="sxs-lookup"><span data-stu-id="9efde-1658">Reservation</span></span>
* <span data-ttu-id="9efde-1659">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="9efde-1659">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="9efde-1660">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1660">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="9efde-1661">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="9efde-1661">Manage App</span></span>
* <span data-ttu-id="9efde-1662">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="9efde-1662">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="9efde-1663">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="9efde-1663">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1664">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1664">Role</span></span>
* <span data-ttu-id="9efde-1665">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="9efde-1665">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="9efde-1666">SignalR</span><span class="sxs-lookup"><span data-stu-id="9efde-1666">SignalR</span></span>
* <span data-ttu-id="9efde-1667">Primera versión</span><span class="sxs-lookup"><span data-stu-id="9efde-1667">First release</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1668">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1668">Storage</span></span>
* <span data-ttu-id="9efde-1669">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="9efde-1669">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="9efde-1670">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="9efde-1670">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1671">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1671">VM</span></span>
* <span data-ttu-id="9efde-1672">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="9efde-1672">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="9efde-1673">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="9efde-1673">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="9efde-1674">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1674">August 28, 2018</span></span>

<span data-ttu-id="9efde-1675">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="9efde-1675">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1676">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1676">Core</span></span>

* <span data-ttu-id="9efde-1677">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="9efde-1677">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="9efde-1678">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9efde-1678">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1679">ACR</span></span>

* <span data-ttu-id="9efde-1680">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-1680">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="9efde-1681">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="9efde-1681">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1682">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1682">ACS</span></span>

* <span data-ttu-id="9efde-1683">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="9efde-1683">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="9efde-1684">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="9efde-1684">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1685">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1685">AppService</span></span>

* <span data-ttu-id="9efde-1686">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="9efde-1686">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="9efde-1687">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-1687">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="9efde-1688">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-1688">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-1689">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-1689">Backup</span></span>

* <span data-ttu-id="9efde-1690">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-1690">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="9efde-1691">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="9efde-1691">Bot Service</span></span>

* <span data-ttu-id="9efde-1692">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="9efde-1692">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9efde-1693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9efde-1693">Cognitive Services</span></span>

* <span data-ttu-id="9efde-1694">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="9efde-1694">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-1695">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-1695">IoT</span></span>

* <span data-ttu-id="9efde-1696">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="9efde-1696">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-1697">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1697">Monitor</span></span>

* <span data-ttu-id="9efde-1698">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="9efde-1698">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="9efde-1699">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="9efde-1699">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1700">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1700">Network</span></span>

* <span data-ttu-id="9efde-1701">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-1701">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1702">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1702">Resource</span></span>

* <span data-ttu-id="9efde-1703">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-1703">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1704">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1704">Storage</span></span>

* <span data-ttu-id="9efde-1705">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-1705">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1706">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1706">VM</span></span>

* <span data-ttu-id="9efde-1707">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-1707">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="9efde-1708">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1708">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="9efde-1709">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1709">Auguest 14, 2018</span></span>

<span data-ttu-id="9efde-1710">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="9efde-1710">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1711">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1711">Core</span></span>

* <span data-ttu-id="9efde-1712">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="9efde-1712">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="9efde-1713">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="9efde-1713">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="9efde-1714">Telemetría</span><span class="sxs-lookup"><span data-stu-id="9efde-1714">Telemetry</span></span>

* <span data-ttu-id="9efde-1715">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="9efde-1715">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1716">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1716">ACR</span></span>

* <span data-ttu-id="9efde-1717">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1717">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="9efde-1718">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="9efde-1718">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1719">ACS</span></span>

* <span data-ttu-id="9efde-1720">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="9efde-1720">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="9efde-1721">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="9efde-1721">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="9efde-1722">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="9efde-1722">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="9efde-1723">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="9efde-1723">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="9efde-1724">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="9efde-1724">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="9efde-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1725">AppService</span></span>

* <span data-ttu-id="9efde-1726">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="9efde-1726">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="9efde-1727">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="9efde-1727">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="9efde-1728">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9efde-1728">BatchAI</span></span>

* <span data-ttu-id="9efde-1729">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="9efde-1729">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="9efde-1730">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1730">Container</span></span>

* <span data-ttu-id="9efde-1731">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1731">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="9efde-1732">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-1732">IoT</span></span>

* <span data-ttu-id="9efde-1733">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="9efde-1733">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="9efde-1734">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="9efde-1734">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="9efde-1735">Iot Central</span><span class="sxs-lookup"><span data-stu-id="9efde-1735">Iot Central</span></span>

* <span data-ttu-id="9efde-1736">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="9efde-1736">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-1737">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9efde-1737">KeyVault</span></span>


* <span data-ttu-id="9efde-1738">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="9efde-1738">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="9efde-1739">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="9efde-1739">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="9efde-1740">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="9efde-1740">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="9efde-1741">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="9efde-1741">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="9efde-1742">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="9efde-1742">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="9efde-1743">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="9efde-1743">Relay</span></span>

* <span data-ttu-id="9efde-1744">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-1744">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-1745">Sql</span><span class="sxs-lookup"><span data-stu-id="9efde-1745">Sql</span></span>

* <span data-ttu-id="9efde-1746">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1746">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1747">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1747">Storage</span></span>

* <span data-ttu-id="9efde-1748">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="9efde-1748">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="9efde-1749">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="9efde-1749">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="9efde-1750">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="9efde-1750">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="9efde-1751">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="9efde-1751">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="9efde-1752">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1752">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1753">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1753">VM</span></span>

* <span data-ttu-id="9efde-1754">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="9efde-1754">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="9efde-1755">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1755">July 31, 2018</span></span>

<span data-ttu-id="9efde-1756">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="9efde-1756">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1757">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1757">ACR</span></span>

* <span data-ttu-id="9efde-1758">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1758">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="9efde-1759">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1759">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1760">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1760">ACS</span></span>

* <span data-ttu-id="9efde-1761">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="9efde-1761">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-1762">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-1762">Batch</span></span>

* <span data-ttu-id="9efde-1763">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="9efde-1763">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1764">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1764">Container</span></span>

* <span data-ttu-id="9efde-1765">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="9efde-1765">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1766">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1766">Network</span></span>

* <span data-ttu-id="9efde-1767">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9efde-1767">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="9efde-1768">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1768">Resource</span></span>

* <span data-ttu-id="9efde-1769">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="9efde-1769">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="9efde-1770">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="9efde-1770">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1771">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1771">Role</span></span>

* <span data-ttu-id="9efde-1772">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="9efde-1772">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="9efde-1773">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="9efde-1773">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="9efde-1774">Search</span><span class="sxs-lookup"><span data-stu-id="9efde-1774">Search</span></span>

* <span data-ttu-id="9efde-1775">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="9efde-1775">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="9efde-1776">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9efde-1776">Service Bus</span></span>

* <span data-ttu-id="9efde-1777">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="9efde-1777">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="9efde-1778">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="9efde-1778">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="9efde-1779">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="9efde-1779">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="9efde-1780">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="9efde-1780">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1781">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1781">Storage</span></span>

* <span data-ttu-id="9efde-1782">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="9efde-1782">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="9efde-1783">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="9efde-1783">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1784">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1784">VM</span></span>

* <span data-ttu-id="9efde-1785">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="9efde-1785">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="9efde-1786">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="9efde-1786">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="9efde-1787">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="9efde-1787">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="9efde-1788">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="9efde-1788">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="9efde-1789">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1789">July 18, 2018</span></span>

<span data-ttu-id="9efde-1790">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="9efde-1790">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1791">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1791">Core</span></span>

* <span data-ttu-id="9efde-1792">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="9efde-1792">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="9efde-1793">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="9efde-1793">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="9efde-1794">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-1794">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1795">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1795">ACR</span></span>

* <span data-ttu-id="9efde-1796">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="9efde-1796">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="9efde-1797">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="9efde-1797">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="9efde-1798">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="9efde-1798">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="9efde-1799">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="9efde-1799">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1800">ACS</span></span>

* <span data-ttu-id="9efde-1801">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="9efde-1801">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1802">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1802">AppService</span></span>

* <span data-ttu-id="9efde-1803">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="9efde-1803">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-1804">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-1804">Batch</span></span>

* <span data-ttu-id="9efde-1805">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="9efde-1805">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="9efde-1806">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="9efde-1806">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9efde-1807">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9efde-1807">Batch AI</span></span>

* <span data-ttu-id="9efde-1808">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="9efde-1808">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1809">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1809">Container</span></span>

* <span data-ttu-id="9efde-1810">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="9efde-1810">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="9efde-1811">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="9efde-1811">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1812">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1812">Network</span></span>

* <span data-ttu-id="9efde-1813">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1813">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="9efde-1814">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1814">Added `network nic wait`</span></span>
* <span data-ttu-id="9efde-1815">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="9efde-1815">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="9efde-1816">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="9efde-1816">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="9efde-1817">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1817">Resource</span></span>

* <span data-ttu-id="9efde-1818">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9efde-1818">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="9efde-1819">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="9efde-1819">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="9efde-1820">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1820">Added `deployment wait` command</span></span>
* <span data-ttu-id="9efde-1821">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="9efde-1821">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1822">SQL</span></span>

* <span data-ttu-id="9efde-1823">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1823">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="9efde-1824">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="9efde-1824">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="9efde-1825">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="9efde-1825">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1826">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1826">Storage</span></span>

* <span data-ttu-id="9efde-1827">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="9efde-1827">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1828">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1828">VM</span></span>

* <span data-ttu-id="9efde-1829">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="9efde-1829">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="9efde-1830">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="9efde-1830">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="9efde-1831">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1831">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9efde-1832">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1832">July 3, 2018</span></span>

<span data-ttu-id="9efde-1833">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="9efde-1833">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-1834">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-1834">AKS</span></span>

* <span data-ttu-id="9efde-1835">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="9efde-1835">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="9efde-1836">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1836">July 3, 2018</span></span>

<span data-ttu-id="9efde-1837">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="9efde-1837">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1838">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1838">Core</span></span>

* <span data-ttu-id="9efde-1839">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="9efde-1839">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1840">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1840">ACR</span></span>

* <span data-ttu-id="9efde-1841">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="9efde-1841">Added polling build status</span></span>
* <span data-ttu-id="9efde-1842">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="9efde-1842">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="9efde-1843">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="9efde-1843">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1844">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1844">ACS</span></span>

* <span data-ttu-id="9efde-1845">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="9efde-1845">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="9efde-1846">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="9efde-1846">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="9efde-1847">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1847">Updated options for `aks browse` command.</span></span> <span data-ttu-id="9efde-1848">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="9efde-1848">Added `--listen-port` support</span></span>
* <span data-ttu-id="9efde-1849">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1849">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="9efde-1850">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="9efde-1850">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="9efde-1851">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="9efde-1851">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1852">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1852">AppService</span></span>

* <span data-ttu-id="9efde-1853">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="9efde-1853">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="9efde-1854">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="9efde-1854">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-1855">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-1855">Backup</span></span>

* <span data-ttu-id="9efde-1856">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="9efde-1856">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="9efde-1857">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9efde-1857">BatchAI</span></span>

* <span data-ttu-id="9efde-1858">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="9efde-1858">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="9efde-1859">Nube</span><span class="sxs-lookup"><span data-stu-id="9efde-1859">Cloud</span></span>

* <span data-ttu-id="9efde-1860">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="9efde-1860">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="9efde-1861">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-1861">Container</span></span>

* <span data-ttu-id="9efde-1862">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="9efde-1862">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="9efde-1863">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="9efde-1863">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="9efde-1864">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="9efde-1864">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-1865">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-1865">Extension</span></span>

* <span data-ttu-id="9efde-1866">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="9efde-1866">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1867">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1867">Network</span></span>

* <span data-ttu-id="9efde-1868">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="9efde-1868">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-1869">Rdbms</span><span class="sxs-lookup"><span data-stu-id="9efde-1869">Rdbms</span></span>

* <span data-ttu-id="9efde-1870">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1870">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-1871">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-1871">Resource</span></span>

* <span data-ttu-id="9efde-1872">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="9efde-1872">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1873">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1873">VM</span></span>

* <span data-ttu-id="9efde-1874">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="9efde-1874">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="9efde-1875">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1875">June 25, 2018</span></span>

<span data-ttu-id="9efde-1876">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="9efde-1876">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="9efde-1877">CLI</span><span class="sxs-lookup"><span data-stu-id="9efde-1877">CLI</span></span>

* <span data-ttu-id="9efde-1878">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-1878">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="9efde-1879">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1879">June 19, 2018</span></span>

<span data-ttu-id="9efde-1880">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="9efde-1880">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1881">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1881">Core</span></span>

* <span data-ttu-id="9efde-1882">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-1882">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1883">ACR</span></span>

* <span data-ttu-id="9efde-1884">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="9efde-1884">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="9efde-1885">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="9efde-1885">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1886">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1886">ACS</span></span>

* <span data-ttu-id="9efde-1887">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1887">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="9efde-1888">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="9efde-1888">Added `--update` support</span></span>
* <span data-ttu-id="9efde-1889">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="9efde-1889">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="9efde-1890">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="9efde-1890">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="9efde-1891">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="9efde-1891">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="9efde-1892">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9efde-1892">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="9efde-1893">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9efde-1893">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="9efde-1894">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9efde-1894">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1895">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1895">AppService</span></span>

* <span data-ttu-id="9efde-1896">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="9efde-1896">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="9efde-1897">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="9efde-1897">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-1898">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-1898">Batch</span></span>

* <span data-ttu-id="9efde-1899">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="9efde-1899">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9efde-1900">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9efde-1900">Batch AI</span></span>

* <span data-ttu-id="9efde-1901">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="9efde-1901">Added support for workspaces.</span></span> <span data-ttu-id="9efde-1902">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="9efde-1902">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="9efde-1903">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1903">Added support for experiments.</span></span> <span data-ttu-id="9efde-1904">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="9efde-1904">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="9efde-1905">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="9efde-1905">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="9efde-1906">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1906">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="9efde-1907">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1907">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="9efde-1908">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1908">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="9efde-1909">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="9efde-1909">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="9efde-1910">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1910">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="9efde-1911">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1911">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="9efde-1912">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1912">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="9efde-1913">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1913">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="9efde-1914">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1914">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="9efde-1915">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="9efde-1915">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="9efde-1916">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="9efde-1916">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="9efde-1917">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1917">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="9efde-1918">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="9efde-1918">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="9efde-1919">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="9efde-1919">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="9efde-1920">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9efde-1920">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9efde-1921">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="9efde-1921">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="9efde-1922">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="9efde-1922">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="9efde-1923">Mapas</span><span class="sxs-lookup"><span data-stu-id="9efde-1923">Maps</span></span>

* <span data-ttu-id="9efde-1924">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1924">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1925">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1925">Network</span></span>

* <span data-ttu-id="9efde-1926">Se ha agregado compatibilidad para `https` a `network lb probe create` [6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="9efde-1926">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="9efde-1927">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9efde-1927">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="9efde-1928">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="9efde-1928">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="9efde-1929">Reservations</span><span class="sxs-lookup"><span data-stu-id="9efde-1929">Reservations</span></span>

* <span data-ttu-id="9efde-1930">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1930">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="9efde-1931">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1931">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="9efde-1932">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1932">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="9efde-1933">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1933">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="9efde-1934">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1934">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="9efde-1935">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1935">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="9efde-1936">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-1936">Role</span></span>

* <span data-ttu-id="9efde-1937">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="9efde-1937">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-1938">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1938">SQL</span></span>

* <span data-ttu-id="9efde-1939">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="9efde-1939">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-1940">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1940">Storage</span></span>

* <span data-ttu-id="9efde-1941">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="9efde-1941">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1942">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1942">VM</span></span>

* <span data-ttu-id="9efde-1943">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1943">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="9efde-1944">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="9efde-1944">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="9efde-1945">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="9efde-1945">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9efde-1946">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1946">June 13, 2018</span></span>

<span data-ttu-id="9efde-1947">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="9efde-1947">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1948">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1948">Core</span></span>

* <span data-ttu-id="9efde-1949">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="9efde-1949">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="9efde-1950">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1950">June 13, 2018</span></span>

<span data-ttu-id="9efde-1951">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="9efde-1951">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-1952">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-1952">AKS</span></span>

* <span data-ttu-id="9efde-1953">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1953">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="9efde-1954">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="9efde-1954">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="9efde-1955">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1955">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="9efde-1956">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1956">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="9efde-1957">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1957">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-1958">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-1958">AppService</span></span>

* <span data-ttu-id="9efde-1959">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="9efde-1959">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9efde-1960">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1960">June 5, 2018</span></span>

<span data-ttu-id="9efde-1961">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="9efde-1961">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-1962">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-1962">Interactive</span></span>

* <span data-ttu-id="9efde-1963">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="9efde-1963">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="9efde-1964">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1964">June 5, 2018</span></span>

<span data-ttu-id="9efde-1965">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="9efde-1965">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1966">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1966">Core</span></span>

* <span data-ttu-id="9efde-1967">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="9efde-1967">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="9efde-1968">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="9efde-1968">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-1969">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-1969">ACR</span></span>

* <span data-ttu-id="9efde-1970">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="9efde-1970">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="9efde-1971">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1971">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="9efde-1972">AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-1972">AKS</span></span>

* <span data-ttu-id="9efde-1973">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="9efde-1973">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-1974">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-1974">Batch</span></span>

* <span data-ttu-id="9efde-1975">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="9efde-1975">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-1976">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-1976">IOT</span></span>

* <span data-ttu-id="9efde-1977">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="9efde-1977">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="9efde-1978">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-1978">Network</span></span>

* <span data-ttu-id="9efde-1979">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="9efde-1979">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="9efde-1980">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-1980">Policy Insights</span></span>

* <span data-ttu-id="9efde-1981">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-1981">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="9efde-1982">ARM</span><span class="sxs-lookup"><span data-stu-id="9efde-1982">ARM</span></span>

* <span data-ttu-id="9efde-1983">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="9efde-1983">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-1984">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-1984">SQL</span></span>

* <span data-ttu-id="9efde-1985">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="9efde-1985">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="9efde-1986">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="9efde-1986">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="9efde-1987">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-1987">Storage</span></span>

* <span data-ttu-id="9efde-1988">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="9efde-1988">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-1989">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-1989">VM</span></span>

* <span data-ttu-id="9efde-1990">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="9efde-1990">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="9efde-1991">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1991">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="9efde-1992">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="9efde-1992">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="9efde-1993">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-1993">May 22, 2018</span></span>

<span data-ttu-id="9efde-1994">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="9efde-1994">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="9efde-1995">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-1995">Core</span></span>

* <span data-ttu-id="9efde-1996">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="9efde-1996">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-1997">ACS</span></span>

* <span data-ttu-id="9efde-1998">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="9efde-1998">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="9efde-1999">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="9efde-1999">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-2000">AppService</span></span>

* <span data-ttu-id="9efde-2001">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="9efde-2001">Improved generic update commands</span></span>
* <span data-ttu-id="9efde-2002">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="9efde-2002">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2003">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2003">Container</span></span>

* <span data-ttu-id="9efde-2004">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="9efde-2004">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="9efde-2005">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-2005">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2006">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2006">Extension</span></span>

* <span data-ttu-id="9efde-2007">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="9efde-2007">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2008">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2008">Interactive</span></span>

* <span data-ttu-id="9efde-2009">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="9efde-2009">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="9efde-2010">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="9efde-2010">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-2011">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9efde-2011">KeyVault</span></span>

* <span data-ttu-id="9efde-2012">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="9efde-2012">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2013">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2013">Network</span></span>

* <span data-ttu-id="9efde-2014">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="9efde-2014">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="9efde-2015">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="9efde-2015">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2016">SQL</span></span>

* <span data-ttu-id="9efde-2017">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="9efde-2017">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="9efde-2018">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="9efde-2018">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="9efde-2019">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="9efde-2019">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="9efde-2020">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="9efde-2020">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="9efde-2021">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="9efde-2021">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="9efde-2022">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2022">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="9efde-2023">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="9efde-2023">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="9efde-2024">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2024">`edition`.</span></span> <span data-ttu-id="9efde-2025">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="9efde-2025">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="9efde-2026">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2026">`elasticPoolName`.</span></span> <span data-ttu-id="9efde-2027">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="9efde-2027">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="9efde-2028">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="9efde-2028">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="9efde-2029">`edition`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2029">`edition`.</span></span> <span data-ttu-id="9efde-2030">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="9efde-2030">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="9efde-2031">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2031">`dtu`.</span></span> <span data-ttu-id="9efde-2032">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="9efde-2032">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="9efde-2033">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2033">`databaseDtuMin`.</span></span> <span data-ttu-id="9efde-2034">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="9efde-2034">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="9efde-2035">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2035">`databaseDtuMax`.</span></span> <span data-ttu-id="9efde-2036">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="9efde-2036">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="9efde-2037">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2037">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="9efde-2038">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2038">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2039">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2039">Storage</span></span>

* <span data-ttu-id="9efde-2040">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="9efde-2040">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="9efde-2041">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="9efde-2041">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2042">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2042">VM</span></span>

* <span data-ttu-id="9efde-2043">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2043">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="9efde-2044">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="9efde-2044">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="9efde-2045">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="9efde-2045">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="9efde-2046">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="9efde-2046">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="9efde-2047">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2047">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="9efde-2048">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2048">May 7, 2018</span></span>

<span data-ttu-id="9efde-2049">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="9efde-2049">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2050">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2050">Core</span></span>

* <span data-ttu-id="9efde-2051">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="9efde-2051">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="9efde-2052">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="9efde-2052">Added limited support for positional arguments</span></span>
* <span data-ttu-id="9efde-2053">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2053">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="9efde-2054">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="9efde-2054">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="9efde-2055">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2055">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="9efde-2056">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="9efde-2056">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="9efde-2057">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2057">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="9efde-2058">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="9efde-2058">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="9efde-2059">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2059">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-2060">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-2060">ACR</span></span>

* <span data-ttu-id="9efde-2061">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="9efde-2061">Added ACR Build commands</span></span>
* <span data-ttu-id="9efde-2062">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="9efde-2062">Improved resource not found error messages</span></span>
* <span data-ttu-id="9efde-2063">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="9efde-2063">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="9efde-2064">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="9efde-2064">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="9efde-2065">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="9efde-2065">Improved repository commands error messages</span></span>
* <span data-ttu-id="9efde-2066">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="9efde-2066">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2067">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2067">ACS</span></span>

* <span data-ttu-id="9efde-2068">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-2068">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="9efde-2069">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="9efde-2069">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="9efde-2070">AMS</span><span class="sxs-lookup"><span data-stu-id="9efde-2070">AMS</span></span>

* <span data-ttu-id="9efde-2071">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="9efde-2071">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2072">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2072">Appservice</span></span>

* <span data-ttu-id="9efde-2073">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="9efde-2073">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="9efde-2074">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2074">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="9efde-2075">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="9efde-2075">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="9efde-2076">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-2076">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="9efde-2077">Batch AI</span><span class="sxs-lookup"><span data-stu-id="9efde-2077">Batch AI</span></span>

* <span data-ttu-id="9efde-2078">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="9efde-2078">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9efde-2079">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9efde-2079">Cognitive Services</span></span>

* <span data-ttu-id="9efde-2080">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="9efde-2080">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="9efde-2081">Consumo</span><span class="sxs-lookup"><span data-stu-id="9efde-2081">Consumption</span></span>

* <span data-ttu-id="9efde-2082">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="9efde-2082">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2083">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2083">Container</span></span>

* <span data-ttu-id="9efde-2084">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="9efde-2084">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="9efde-2085">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9efde-2085">Cosmos DB</span></span>

* <span data-ttu-id="9efde-2086">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="9efde-2086">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="9efde-2087">DMS</span><span class="sxs-lookup"><span data-stu-id="9efde-2087">DMS</span></span>

* <span data-ttu-id="9efde-2088">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2088">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2089">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2089">Extension</span></span>

* <span data-ttu-id="9efde-2090">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="9efde-2090">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2091">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2091">Interactive</span></span>

* <span data-ttu-id="9efde-2092">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="9efde-2092">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="9efde-2093">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="9efde-2093">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="9efde-2094">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="9efde-2094">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="9efde-2095">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2095">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="9efde-2096">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-2096">Lab</span></span>

* <span data-ttu-id="9efde-2097">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="9efde-2097">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2098">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2098">Network</span></span>

* <span data-ttu-id="9efde-2099">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="9efde-2099">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="9efde-2100">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2100">Profile</span></span>

* <span data-ttu-id="9efde-2101">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2101">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="9efde-2102">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="9efde-2102">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="9efde-2103">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="9efde-2103">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="9efde-2104">Redis</span><span class="sxs-lookup"><span data-stu-id="9efde-2104">Redis</span></span>

* <span data-ttu-id="9efde-2105">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="9efde-2105">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="9efde-2106">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2106">Deprecated `redis list-all`.</span></span> <span data-ttu-id="9efde-2107">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="9efde-2107">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="9efde-2108">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="9efde-2108">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="9efde-2109">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2109">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="9efde-2110">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-2110">Role</span></span>

* <span data-ttu-id="9efde-2111">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="9efde-2111">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2112">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2112">Storage</span></span>

* <span data-ttu-id="9efde-2113">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="9efde-2113">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="9efde-2114">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="9efde-2114">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="9efde-2115">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="9efde-2115">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="9efde-2116">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="9efde-2116">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="9efde-2117">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="9efde-2117">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2118">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2118">VM</span></span>

* <span data-ttu-id="9efde-2119">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="9efde-2119">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="9efde-2120">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="9efde-2120">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="9efde-2121">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="9efde-2121">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="9efde-2122">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="9efde-2122">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="9efde-2123">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="9efde-2123">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="9efde-2124">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="9efde-2124">Added write accelerator support</span></span>
* <span data-ttu-id="9efde-2125">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2125">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="9efde-2126">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="9efde-2126">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="9efde-2127">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="9efde-2127">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="9efde-2128">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2128">April 10, 2018</span></span>

<span data-ttu-id="9efde-2129">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="9efde-2129">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-2130">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-2130">ACR</span></span>

* <span data-ttu-id="9efde-2131">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="9efde-2131">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2132">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2132">ACS</span></span>

* <span data-ttu-id="9efde-2133">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="9efde-2133">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2134">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2134">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="9efde-2136">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="9efde-2136">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="9efde-2137">BatchAI</span><span class="sxs-lookup"><span data-stu-id="9efde-2137">BatchAI</span></span>

* <span data-ttu-id="9efde-2138">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="9efde-2138">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="9efde-2139">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="9efde-2139">Job level mounting</span></span>
  - <span data-ttu-id="9efde-2140">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="9efde-2140">Environment variables with secret values</span></span>
  - <span data-ttu-id="9efde-2141">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="9efde-2141">Performance counters settings</span></span>
  - <span data-ttu-id="9efde-2142">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="9efde-2142">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="9efde-2143">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="9efde-2143">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="9efde-2144">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="9efde-2144">Usage and limits reporting</span></span>
  - <span data-ttu-id="9efde-2145">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="9efde-2145">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="9efde-2146">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="9efde-2146">Support for custom images</span></span>
  - <span data-ttu-id="9efde-2147">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="9efde-2147">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="9efde-2148">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="9efde-2148">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="9efde-2149">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="9efde-2149">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="9efde-2150">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="9efde-2150">National clouds are supported</span></span>
* <span data-ttu-id="9efde-2151">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="9efde-2151">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="9efde-2152">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="9efde-2152">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="9efde-2153">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="9efde-2153">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="9efde-2154">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="9efde-2154">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="9efde-2155">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="9efde-2155">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="9efde-2156">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="9efde-2156">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="9efde-2157">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2157">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="9efde-2158">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="9efde-2158">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="9efde-2159">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="9efde-2159">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="9efde-2160">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2160">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="9efde-2161">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2161">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="9efde-2162">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="9efde-2162">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="9efde-2163">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2163">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="9efde-2164">Facturación</span><span class="sxs-lookup"><span data-stu-id="9efde-2164">Billing</span></span>

* <span data-ttu-id="9efde-2165">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="9efde-2165">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="9efde-2166">Consumo</span><span class="sxs-lookup"><span data-stu-id="9efde-2166">Consumption</span></span>

* <span data-ttu-id="9efde-2167">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2167">Added `marketplace` commands</span></span>
* <span data-ttu-id="9efde-2168">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9efde-2168">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="9efde-2169">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="9efde-2169">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="9efde-2170">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="9efde-2170">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="9efde-2171">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="9efde-2171">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="9efde-2172">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="9efde-2172">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2173">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2173">Container</span></span>

* <span data-ttu-id="9efde-2174">Se han agregado los parámetros de montaje de volúmenes del repositorio de git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` y `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2174">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="9efde-2175">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="9efde-2175">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2176">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2176">Extension</span></span>

* <span data-ttu-id="9efde-2177">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="9efde-2177">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2178">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2178">Interactive</span></span>

* <span data-ttu-id="9efde-2179">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="9efde-2179">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="9efde-2180">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2180">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="9efde-2181">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="9efde-2181">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2182">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2182">Network</span></span>

* <span data-ttu-id="9efde-2183">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2183">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="9efde-2184">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2184">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="9efde-2185">4910</span><span class="sxs-lookup"><span data-stu-id="9efde-2185">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="9efde-2186">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="9efde-2186">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="9efde-2187">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="9efde-2187">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="9efde-2188">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2188">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="9efde-2189">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2189">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="9efde-2190">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="9efde-2190">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2191">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2191">Profile</span></span>

* <span data-ttu-id="9efde-2192">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="9efde-2192">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="9efde-2193">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="9efde-2193">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-2194">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-2194">RDBMS</span></span>

* <span data-ttu-id="9efde-2195">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2195">Added `georestore` command</span></span>
* <span data-ttu-id="9efde-2196">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2196">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2197">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2197">Resource</span></span>

* <span data-ttu-id="9efde-2198">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2198">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="9efde-2199">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2199">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2200">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2200">SQL</span></span>

* <span data-ttu-id="9efde-2201">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="9efde-2201">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2202">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2202">Storage</span></span>

* <span data-ttu-id="9efde-2203">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="9efde-2203">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2204">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2204">VM</span></span>

* <span data-ttu-id="9efde-2205">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2205">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="9efde-2206">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="9efde-2206">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="9efde-2208">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2208">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="9efde-2209">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="9efde-2209">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="9efde-2210">5718</span><span class="sxs-lookup"><span data-stu-id="9efde-2210">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="9efde-2211">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="9efde-2211">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="9efde-2212">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2212">March 27, 2018</span></span>

<span data-ttu-id="9efde-2213">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="9efde-2213">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2214">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2214">Core</span></span>

* <span data-ttu-id="9efde-2215">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="9efde-2215">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2216">ACS</span></span>

* <span data-ttu-id="9efde-2217">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9efde-2217">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2218">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2218">Appservice</span></span>

* <span data-ttu-id="9efde-2219">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2219">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="9efde-2220">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2220">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-2221">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-2221">Backup</span></span>

* <span data-ttu-id="9efde-2222">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2222">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="9efde-2223">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2223">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="9efde-2224">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-2224">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="9efde-2225">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="9efde-2225">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2226">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2226">Container</span></span>

* <span data-ttu-id="9efde-2227">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2227">Added `container exec` command.</span></span> <span data-ttu-id="9efde-2228">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="9efde-2228">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="9efde-2229">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-2229">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2230">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2230">Extension</span></span>

* <span data-ttu-id="9efde-2231">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-2231">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="9efde-2232">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="9efde-2232">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="9efde-2233">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9efde-2233">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2234">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2234">Interactive</span></span>

* <span data-ttu-id="9efde-2235">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2235">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="9efde-2236">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="9efde-2236">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="9efde-2237">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2237">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="9efde-2238">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="9efde-2238">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="9efde-2239">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-2239">Lab</span></span>

* <span data-ttu-id="9efde-2240">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="9efde-2240">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2241">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2241">Monitor</span></span>

* <span data-ttu-id="9efde-2242">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="9efde-2242">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="9efde-2243">Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="9efde-2243">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="9efde-2244">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="9efde-2244">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2245">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2245">Network</span></span>

* <span data-ttu-id="9efde-2246">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="9efde-2246">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2247">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2247">Profile</span></span>

* <span data-ttu-id="9efde-2248">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="9efde-2248">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-2249">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-2249">RDBMS</span></span>

* <span data-ttu-id="9efde-2250">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="9efde-2250">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2251">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2251">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="9efde-2253">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-2253">Role</span></span>

* <span data-ttu-id="9efde-2254">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2254">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="9efde-2255">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="9efde-2255">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="9efde-2256">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2256">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="9efde-2257">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2257">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="9efde-2258">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="9efde-2258">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2259">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2259">Storage</span></span>

* <span data-ttu-id="9efde-2260">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="9efde-2260">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="9efde-2261">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="9efde-2261">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2262">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2262">VM</span></span>

* <span data-ttu-id="9efde-2263">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="9efde-2263">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="9efde-2264">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2264">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="9efde-2265">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="9efde-2265">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="9efde-2266">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="9efde-2266">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="9efde-2267">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2267">March 13, 2018</span></span>

<span data-ttu-id="9efde-2268">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="9efde-2268">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-2269">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-2269">ACR</span></span>

* <span data-ttu-id="9efde-2270">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2270">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="9efde-2271">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-2271">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="9efde-2272">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="9efde-2272">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2273">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2273">ACS</span></span>

* <span data-ttu-id="9efde-2274">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="9efde-2274">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="9efde-2275">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="9efde-2275">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="9efde-2276">Advisor</span><span class="sxs-lookup"><span data-stu-id="9efde-2276">Advisor</span></span>

* <span data-ttu-id="9efde-2277">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="9efde-2277">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="9efde-2278">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2278">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="9efde-2279">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="9efde-2279">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="9efde-2280">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="9efde-2280">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="9efde-2281">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2281">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2282">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2282">Appservice</span></span>

* <span data-ttu-id="9efde-2283">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-2283">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="9efde-2284">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2284">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="9efde-2285">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="9efde-2285">Eventhubs</span></span>

* <span data-ttu-id="9efde-2286">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-2286">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2287">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2287">Extension</span></span>

* <span data-ttu-id="9efde-2288">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="9efde-2288">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2289">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2289">Interactive</span></span>

* <span data-ttu-id="9efde-2290">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="9efde-2290">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="9efde-2291">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="9efde-2291">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="9efde-2292">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="9efde-2292">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="9efde-2293">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="9efde-2293">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2294">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2294">Monitor</span></span>

* <span data-ttu-id="9efde-2295">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-2295">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="9efde-2296">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2296">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="9efde-2297">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2297">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="9efde-2298">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2298">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2299">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2299">Network</span></span>

* <span data-ttu-id="9efde-2300">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2300">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="9efde-2301">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-2301">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="9efde-2302">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2302">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="9efde-2303">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2303">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2304">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2304">Profile</span></span>

* <span data-ttu-id="9efde-2305">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-2305">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="9efde-2306">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2306">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-2307">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-2307">RDBMS</span></span>

* <span data-ttu-id="9efde-2308">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="9efde-2308">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="9efde-2309">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="9efde-2309">Service Bus</span></span>

* <span data-ttu-id="9efde-2310">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-2310">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2311">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2311">Storage</span></span>

* <span data-ttu-id="9efde-2312">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="9efde-2312">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="9efde-2313">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="9efde-2313">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2314">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2314">VM</span></span>

* <span data-ttu-id="9efde-2315">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="9efde-2315">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="9efde-2316">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-2316">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="9efde-2317">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-2317">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="9efde-2318">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="9efde-2318">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="9efde-2319">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2319">February 27, 2018</span></span>

<span data-ttu-id="9efde-2320">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="9efde-2320">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2321">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2321">Core</span></span>

* <span data-ttu-id="9efde-2322">Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="9efde-2322">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="9efde-2323">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="9efde-2323">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="9efde-2324">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="9efde-2324">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2325">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2325">ACS</span></span>

* <span data-ttu-id="9efde-2326">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9efde-2326">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="9efde-2327">Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="9efde-2327">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="9efde-2328">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="9efde-2328">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="9efde-2329">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="9efde-2329">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2330">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2330">Appservice</span></span>

* <span data-ttu-id="9efde-2331">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="9efde-2331">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="9efde-2332">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="9efde-2332">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="9efde-2333">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9efde-2333">Cognitive Services</span></span>

* <span data-ttu-id="9efde-2334">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9efde-2334">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="9efde-2335">Consumo</span><span class="sxs-lookup"><span data-stu-id="9efde-2335">Consumption</span></span>

* <span data-ttu-id="9efde-2336">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="9efde-2336">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="9efde-2337">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="9efde-2337">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2338">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2338">Container</span></span>

* <span data-ttu-id="9efde-2339">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="9efde-2339">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2340">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2340">Network</span></span>

* <span data-ttu-id="9efde-2341">Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="9efde-2341">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2342">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2342">Resource</span></span>

* <span data-ttu-id="9efde-2343">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="9efde-2343">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="9efde-2344">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-2344">Role</span></span>

* <span data-ttu-id="9efde-2345">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="9efde-2345">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2346">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2346">SQL</span></span>

* <span data-ttu-id="9efde-2347">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="9efde-2347">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2348">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2348">Storage</span></span>

* <span data-ttu-id="9efde-2349">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2349">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2350">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2350">VM</span></span>

* <span data-ttu-id="9efde-2351">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="9efde-2351">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="9efde-2352">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2352">February 13, 2018</span></span>

<span data-ttu-id="9efde-2353">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="9efde-2353">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2354">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2354">Core</span></span>

* <span data-ttu-id="9efde-2355">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="9efde-2355">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2356">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2356">ACS</span></span>

* <span data-ttu-id="9efde-2357">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2357">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="9efde-2358">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2358">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="9efde-2359">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9efde-2359">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="9efde-2360">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-2360">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="9efde-2361">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="9efde-2361">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="9efde-2362">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="9efde-2362">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="9efde-2363">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9efde-2363">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="9efde-2364">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="9efde-2364">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2365">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2365">Appservice</span></span>

* <span data-ttu-id="9efde-2366">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="9efde-2366">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="9efde-2367">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="9efde-2367">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-2368">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-2368">CDN</span></span>

* <span data-ttu-id="9efde-2369">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2369">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2370">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2370">Container</span></span>

* <span data-ttu-id="9efde-2371">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="9efde-2371">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="9efde-2372">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-2372">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-2373">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-2373">CosmosDB</span></span>

* <span data-ttu-id="9efde-2374">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="9efde-2374">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2375">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2375">Extension</span></span>

* <span data-ttu-id="9efde-2376">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2376">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="9efde-2377">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2377">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="9efde-2378">Comentarios</span><span class="sxs-lookup"><span data-stu-id="9efde-2378">Feedback</span></span>

* <span data-ttu-id="9efde-2379">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="9efde-2379">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2380">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2380">Interactive</span></span>

* <span data-ttu-id="9efde-2381">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="9efde-2381">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="9efde-2382">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="9efde-2382">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-2383">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-2383">IoT</span></span>

* <span data-ttu-id="9efde-2384">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2384">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9efde-2385">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2385">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="9efde-2386">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2386">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="9efde-2387">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="9efde-2387">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2388">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2388">Monitor</span></span>

* <span data-ttu-id="9efde-2389">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2389">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2390">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2390">Network</span></span>

* <span data-ttu-id="9efde-2391">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-2391">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="9efde-2392">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2392">Profile</span></span>

* <span data-ttu-id="9efde-2393">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="9efde-2393">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2394">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2394">Resource</span></span>

* <span data-ttu-id="9efde-2395">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="9efde-2395">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="9efde-2396">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-2396">Role</span></span>

* <span data-ttu-id="9efde-2397">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2397">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2398">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2398">SQL</span></span>

* <span data-ttu-id="9efde-2399">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2399">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="9efde-2400">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2400">Added `sql db rename`</span></span>
* <span data-ttu-id="9efde-2401">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="9efde-2401">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2402">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2402">Storage</span></span>

* <span data-ttu-id="9efde-2403">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="9efde-2403">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2404">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2404">VM</span></span>

* <span data-ttu-id="9efde-2405">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="9efde-2405">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="9efde-2406">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="9efde-2406">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="9efde-2407">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="9efde-2407">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="9efde-2408">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2408">January 31, 2018</span></span>

<span data-ttu-id="9efde-2409">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="9efde-2409">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2410">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2410">Core</span></span>

* <span data-ttu-id="9efde-2411">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="9efde-2411">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="9efde-2412">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="9efde-2412">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="9efde-2413">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="9efde-2413">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="9efde-2414">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="9efde-2414">Use `--verbose` to see</span></span>
* <span data-ttu-id="9efde-2415">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="9efde-2415">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2416">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2416">ACS</span></span>

* <span data-ttu-id="9efde-2417">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="9efde-2417">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="9efde-2418">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="9efde-2418">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2419">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2419">Appservice</span></span>

* <span data-ttu-id="9efde-2420">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="9efde-2420">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="9efde-2421">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="9efde-2421">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-2422">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-2422">CDN</span></span>

* <span data-ttu-id="9efde-2423">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2423">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-2424">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-2424">CosmosDB</span></span>

* <span data-ttu-id="9efde-2425">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="9efde-2425">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2426">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2426">Interactive</span></span>

* <span data-ttu-id="9efde-2427">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="9efde-2427">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2428">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2428">Network</span></span>

* <span data-ttu-id="9efde-2429">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2429">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="9efde-2430">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="9efde-2430">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="9efde-2431">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2431">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="9efde-2432">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2432">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="9efde-2433">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="9efde-2433">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="9efde-2434">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="9efde-2434">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="9efde-2435">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="9efde-2435">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="9efde-2436">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="9efde-2436">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="9efde-2437">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="9efde-2437">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="9efde-2438">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="9efde-2438">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2439">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2439">Profile</span></span>

* <span data-ttu-id="9efde-2440">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="9efde-2440">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2441">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2441">Resource</span></span>

* <span data-ttu-id="9efde-2442">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="9efde-2442">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2443">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2443">Storage</span></span>

* <span data-ttu-id="9efde-2444">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="9efde-2444">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="9efde-2445">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="9efde-2445">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="9efde-2446">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="9efde-2446">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="9efde-2447">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2447">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="9efde-2448">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="9efde-2448">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2449">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2449">VM</span></span>

* <span data-ttu-id="9efde-2450">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="9efde-2450">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="9efde-2451">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="9efde-2451">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="9efde-2452">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="9efde-2452">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="9efde-2453">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2453">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="9efde-2454">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="9efde-2454">January 17, 2018</span></span>

<span data-ttu-id="9efde-2455">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="9efde-2455">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-2456">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-2456">ACR</span></span>

* <span data-ttu-id="9efde-2457">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="9efde-2457">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="9efde-2458">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="9efde-2458">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2459">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2459">ACS</span></span>

* <span data-ttu-id="9efde-2460">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="9efde-2460">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="9efde-2461">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="9efde-2461">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2462">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2462">Appservice</span></span>

* <span data-ttu-id="9efde-2463">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="9efde-2463">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="9efde-2464">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="9efde-2464">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="9efde-2465">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="9efde-2465">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-2466">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-2466">Backup</span></span>

* <span data-ttu-id="9efde-2467">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="9efde-2467">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="9efde-2468">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="9efde-2468">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="9efde-2469">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="9efde-2469">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="9efde-2470">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="9efde-2470">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="9efde-2471">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="9efde-2471">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-2472">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-2472">Batch</span></span>

* <span data-ttu-id="9efde-2473">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="9efde-2473">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="9efde-2474">Nube</span><span class="sxs-lookup"><span data-stu-id="9efde-2474">Cloud</span></span>

* <span data-ttu-id="9efde-2475">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="9efde-2475">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="9efde-2476">Consumo</span><span class="sxs-lookup"><span data-stu-id="9efde-2476">Consumption</span></span>

* <span data-ttu-id="9efde-2477">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="9efde-2477">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="9efde-2478">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9efde-2478">Event Grid</span></span>

* <span data-ttu-id="9efde-2479">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9efde-2479">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9efde-2480">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="9efde-2480">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="9efde-2481">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2481">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="9efde-2482">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="9efde-2482">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="9efde-2483">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2483">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="9efde-2484">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2484">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="9efde-2485">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="9efde-2485">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="9efde-2486">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="9efde-2486">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2487">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2487">Interactive</span></span>

* <span data-ttu-id="9efde-2488">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="9efde-2488">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="9efde-2489">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="9efde-2489">Fixed errors on startup</span></span>
* <span data-ttu-id="9efde-2490">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="9efde-2490">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-2491">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-2491">IoT</span></span>

* <span data-ttu-id="9efde-2492">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9efde-2492">Added support for device provisioning service</span></span>
* <span data-ttu-id="9efde-2493">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2493">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="9efde-2494">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-2494">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2495">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2495">Monitor</span></span>

* <span data-ttu-id="9efde-2496">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="9efde-2496">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="9efde-2497">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2497">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="9efde-2498">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="9efde-2498">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2499">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2499">Network</span></span>

* <span data-ttu-id="9efde-2500">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2500">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="9efde-2501">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2501">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2502">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2502">Profile</span></span>

* <span data-ttu-id="9efde-2503">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="9efde-2503">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="9efde-2504">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-2504">Role</span></span>

* <span data-ttu-id="9efde-2505">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="9efde-2505">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9efde-2506">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9efde-2506">Service Fabric</span></span>

* <span data-ttu-id="9efde-2507">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="9efde-2507">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="9efde-2508">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="9efde-2508">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2509">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2509">VM</span></span>

* <span data-ttu-id="9efde-2510">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="9efde-2510">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="9efde-2511">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="9efde-2511">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="9efde-2512">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="9efde-2512">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="9efde-2513">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="9efde-2513">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="9efde-2514">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="9efde-2514">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="9efde-2515">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2515">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="9efde-2516">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2516">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="9efde-2517">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="9efde-2517">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="9efde-2518">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2518">December 19, 2017</span></span>

<span data-ttu-id="9efde-2519">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="9efde-2519">Version 2.0.23</span></span>

* <span data-ttu-id="9efde-2520">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="9efde-2520">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2521">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2521">Container</span></span>

* <span data-ttu-id="9efde-2522">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2522">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2523">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2523">Network</span></span>

* <span data-ttu-id="9efde-2524">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2524">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="9efde-2525">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2525">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2526">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2526">Storage</span></span>

* <span data-ttu-id="9efde-2527">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="9efde-2527">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2528">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2528">VM</span></span>

* <span data-ttu-id="9efde-2529">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="9efde-2529">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="9efde-2530">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2530">December 5, 2017</span></span>

<span data-ttu-id="9efde-2531">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="9efde-2531">Version 2.0.22</span></span>

* <span data-ttu-id="9efde-2532">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2532">Removed `az component` commands.</span></span> <span data-ttu-id="9efde-2533">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="9efde-2533">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2534">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2534">Core</span></span>
* <span data-ttu-id="9efde-2535">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="9efde-2535">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="9efde-2536">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="9efde-2536">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2537">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2537">ACS</span></span>

* <span data-ttu-id="9efde-2538">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="9efde-2538">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="9efde-2539">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2539">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="9efde-2540">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="9efde-2540">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="9efde-2541">Advisor</span><span class="sxs-lookup"><span data-stu-id="9efde-2541">Advisor</span></span>

* <span data-ttu-id="9efde-2542">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-2542">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2543">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2543">Appservice</span></span>

* <span data-ttu-id="9efde-2544">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="9efde-2544">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="9efde-2545">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="9efde-2545">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="9efde-2546">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="9efde-2546">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="9efde-2547">Consumo</span><span class="sxs-lookup"><span data-stu-id="9efde-2547">Consumption</span></span>

* <span data-ttu-id="9efde-2548">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="9efde-2548">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2549">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2549">Container</span></span>

* <span data-ttu-id="9efde-2550">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="9efde-2550">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2551">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2551">Monitor</span></span>

* <span data-ttu-id="9efde-2552">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="9efde-2552">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2553">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2553">Resource</span></span>

* <span data-ttu-id="9efde-2554">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="9efde-2554">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="9efde-2555">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-2555">Role</span></span>

* <span data-ttu-id="9efde-2556">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="9efde-2556">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="9efde-2557">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="9efde-2557">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="9efde-2558">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="9efde-2558">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2559">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2559">SQL</span></span>

* <span data-ttu-id="9efde-2560">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="9efde-2560">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="9efde-2561">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2561">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2562">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2562">VM</span></span>

* <span data-ttu-id="9efde-2563">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="9efde-2563">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="9efde-2564">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2564">November 14, 2017</span></span>

<span data-ttu-id="9efde-2565">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="9efde-2565">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-2566">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-2566">ACR</span></span>

* <span data-ttu-id="9efde-2567">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="9efde-2567">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="9efde-2568">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2568">ACS</span></span>

* <span data-ttu-id="9efde-2569">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="9efde-2569">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="9efde-2570">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2570">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="9efde-2571">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="9efde-2571">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="9efde-2572">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="9efde-2572">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="9efde-2573">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="9efde-2573">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2574">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2574">Appservice</span></span>

* <span data-ttu-id="9efde-2575">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="9efde-2575">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="9efde-2576">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9efde-2576">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="9efde-2577">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="9efde-2577">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="9efde-2578">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="9efde-2578">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="9efde-2579">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="9efde-2579">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="9efde-2580">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="9efde-2580">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-2581">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-2581">Batch</span></span>

* <span data-ttu-id="9efde-2582">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="9efde-2582">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="9efde-2583">Batchai</span><span class="sxs-lookup"><span data-stu-id="9efde-2583">Batchai</span></span>

* <span data-ttu-id="9efde-2584">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2584">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="9efde-2585">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2585">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="9efde-2586">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="9efde-2586">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="9efde-2587">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2587">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="9efde-2588">Nube</span><span class="sxs-lookup"><span data-stu-id="9efde-2588">Cloud</span></span>

* <span data-ttu-id="9efde-2589">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="9efde-2589">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2590">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2590">Container</span></span>

* <span data-ttu-id="9efde-2591">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="9efde-2591">Added support to open multiple ports</span></span>
* <span data-ttu-id="9efde-2592">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="9efde-2592">Added container group restart policy</span></span>
* <span data-ttu-id="9efde-2593">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="9efde-2593">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="9efde-2594">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="9efde-2594">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9efde-2595">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9efde-2595">Data Lake Analytics</span></span>

* <span data-ttu-id="9efde-2596">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="9efde-2596">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9efde-2597">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9efde-2597">Data Lake Store</span></span>

* <span data-ttu-id="9efde-2598">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="9efde-2598">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2599">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2599">Extension</span></span>

* <span data-ttu-id="9efde-2600">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="9efde-2600">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="9efde-2601">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="9efde-2601">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-2602">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-2602">IoT</span></span>

* <span data-ttu-id="9efde-2603">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="9efde-2603">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2604">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2604">Monitor</span></span>

* <span data-ttu-id="9efde-2605">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2605">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2606">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2606">Network</span></span>

* <span data-ttu-id="9efde-2607">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="9efde-2607">Added support for CAA DNS records</span></span>
* <span data-ttu-id="9efde-2608">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2608">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="9efde-2609">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2609">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="9efde-2610">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="9efde-2610">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="9efde-2611">Reservations</span><span class="sxs-lookup"><span data-stu-id="9efde-2611">Reservations</span></span>

* <span data-ttu-id="9efde-2612">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-2612">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2613">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2613">Resource</span></span>

* <span data-ttu-id="9efde-2614">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-2614">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2615">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2615">SQL</span></span>

* <span data-ttu-id="9efde-2616">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2616">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2617">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2617">Storage</span></span>

* <span data-ttu-id="9efde-2618">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="9efde-2618">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="9efde-2619">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="9efde-2619">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="9efde-2620">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="9efde-2620">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="9efde-2621">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="9efde-2621">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="9efde-2622">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2622">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="9efde-2623">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="9efde-2623">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="9efde-2624">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="9efde-2624">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2625">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2625">VM</span></span>

* <span data-ttu-id="9efde-2626">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="9efde-2626">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="9efde-2627">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="9efde-2627">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="9efde-2628">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="9efde-2628">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="9efde-2629">Cambio de nombre de `vm format-secret` a `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="9efde-2629">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="9efde-2630">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9efde-2630">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="9efde-2631">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2631">October 24, 2017</span></span>

<span data-ttu-id="9efde-2632">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="9efde-2632">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2633">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2633">Core</span></span>

* <span data-ttu-id="9efde-2634">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="9efde-2634">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-2635">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-2635">ACR</span></span>

* <span data-ttu-id="9efde-2636">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="9efde-2636">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="9efde-2637">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="9efde-2637">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="9efde-2638">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="9efde-2638">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2639">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2639">ACS</span></span>

* <span data-ttu-id="9efde-2640">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="9efde-2640">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="9efde-2641">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9efde-2641">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2642">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2642">Appservice</span></span>

* <span data-ttu-id="9efde-2643">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="9efde-2643">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="9efde-2644">Componente</span><span class="sxs-lookup"><span data-stu-id="9efde-2644">Component</span></span>

* <span data-ttu-id="9efde-2645">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="9efde-2645">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2646">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2646">Monitor</span></span>

* <span data-ttu-id="9efde-2647">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2647">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2648">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2648">Resource</span></span>

* <span data-ttu-id="9efde-2649">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="9efde-2649">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="9efde-2650">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="9efde-2650">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2651">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2651">VM</span></span>

* <span data-ttu-id="9efde-2652">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2652">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="9efde-2653">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2653">October 9, 2017</span></span>

<span data-ttu-id="9efde-2654">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="9efde-2654">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2655">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2655">Core</span></span>

* <span data-ttu-id="9efde-2656">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="9efde-2656">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2657">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2657">Appservice</span></span>

* <span data-ttu-id="9efde-2658">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2658">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-2659">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-2659">Batch</span></span>

* <span data-ttu-id="9efde-2660">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="9efde-2660">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="9efde-2661">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="9efde-2661">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="9efde-2662">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-2662">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="9efde-2663">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="9efde-2663">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="9efde-2664">Batchai</span><span class="sxs-lookup"><span data-stu-id="9efde-2664">Batchai</span></span>

* <span data-ttu-id="9efde-2665">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-2665">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-2666">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9efde-2666">Keyvault</span></span>

* <span data-ttu-id="9efde-2667">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9efde-2667">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="9efde-2668">(#4448)</span><span class="sxs-lookup"><span data-stu-id="9efde-2668">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="9efde-2669">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2669">Network</span></span>

* <span data-ttu-id="9efde-2670">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="9efde-2670">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="9efde-2671">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="9efde-2671">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2672">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2672">Resource</span></span>

* <span data-ttu-id="9efde-2673">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-2673">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="9efde-2674">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="9efde-2674">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="9efde-2675">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="9efde-2675">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="9efde-2676">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="9efde-2676">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2677">Sql</span><span class="sxs-lookup"><span data-stu-id="9efde-2677">Sql</span></span>

* <span data-ttu-id="9efde-2678">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="9efde-2678">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="9efde-2679">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="9efde-2679">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="9efde-2680">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="9efde-2680">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2681">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2681">Storage</span></span>

* <span data-ttu-id="9efde-2682">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="9efde-2682">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2683">Vm</span><span class="sxs-lookup"><span data-stu-id="9efde-2683">Vm</span></span>

* <span data-ttu-id="9efde-2684">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="9efde-2684">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="9efde-2685">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2685">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="9efde-2686">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="9efde-2686">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="9efde-2687">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2687">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="9efde-2688">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2688">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="9efde-2689">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2689">September 22, 2017</span></span>

<span data-ttu-id="9efde-2690">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="9efde-2690">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2691">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2691">Resource</span></span>

* <span data-ttu-id="9efde-2692">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="9efde-2692">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="9efde-2693">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="9efde-2693">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="9efde-2694">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2694">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="9efde-2695">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="9efde-2695">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2696">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2696">Network</span></span>

* <span data-ttu-id="9efde-2697">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="9efde-2697">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="9efde-2698">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="9efde-2698">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="9efde-2699">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="9efde-2699">Added `asg` application security group commands</span></span>
* <span data-ttu-id="9efde-2700">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2700">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="9efde-2701">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2701">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9efde-2702">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2702">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="9efde-2703">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2703">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2704">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2704">Storage</span></span>

* <span data-ttu-id="9efde-2705">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="9efde-2705">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="9efde-2706">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="9efde-2706">Eventgrid</span></span>

* <span data-ttu-id="9efde-2707">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="9efde-2707">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2708">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2708">SQL</span></span>

* <span data-ttu-id="9efde-2709">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="9efde-2709">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="9efde-2710">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="9efde-2710">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="9efde-2711">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2711">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-2712">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9efde-2712">Keyvault</span></span>

* <span data-ttu-id="9efde-2713">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="9efde-2713">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2714">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2714">VM</span></span>

* <span data-ttu-id="9efde-2715">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2715">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="9efde-2716">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="9efde-2716">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="9efde-2717">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2717">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="9efde-2718">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="9efde-2718">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="9efde-2719">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="9efde-2719">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="9efde-2720">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="9efde-2720">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2721">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2721">ACS</span></span>

* <span data-ttu-id="9efde-2722">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2722">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2723">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2723">Appservice</span></span>

* <span data-ttu-id="9efde-2724">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2724">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="9efde-2725">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="9efde-2725">Backup</span></span>

* <span data-ttu-id="9efde-2726">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-2726">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="9efde-2727">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2727">September 11, 2017</span></span>

<span data-ttu-id="9efde-2728">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="9efde-2728">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="9efde-2729">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2729">Core</span></span>

* <span data-ttu-id="9efde-2730">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="9efde-2730">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="9efde-2731">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="9efde-2731">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2732">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2732">Acs</span></span>

* <span data-ttu-id="9efde-2733">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2733">Added `acs list-locations` command</span></span>
* <span data-ttu-id="9efde-2734">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="9efde-2734">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2735">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2735">Appservice</span></span>

* <span data-ttu-id="9efde-2736">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="9efde-2736">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-2737">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-2737">CDN</span></span>

* <span data-ttu-id="9efde-2738">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2738">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="9efde-2739">Extensión</span><span class="sxs-lookup"><span data-stu-id="9efde-2739">Extension</span></span>

* <span data-ttu-id="9efde-2740">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-2740">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-2741">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9efde-2741">Keyvault</span></span>

* <span data-ttu-id="9efde-2742">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="9efde-2742">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2743">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2743">Network</span></span>

* <span data-ttu-id="9efde-2744">Cambio de nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9efde-2744">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9efde-2745">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2745">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="9efde-2746">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2746">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="9efde-2747">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2747">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9efde-2748">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2748">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-2749">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-2749">Resource</span></span>

* <span data-ttu-id="9efde-2750">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2750">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="9efde-2751">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2751">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="9efde-2752">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="9efde-2752">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="9efde-2753">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="9efde-2753">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-2754">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-2754">SQL</span></span>

* <span data-ttu-id="9efde-2755">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2755">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2756">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2756">VM</span></span>

* <span data-ttu-id="9efde-2757">Solucionado: no asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2757">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="9efde-2758">Solucionado: usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="9efde-2758">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="9efde-2759">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2759">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="9efde-2760">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="9efde-2760">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="9efde-2761">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2761">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="9efde-2762">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2762">August 31, 2017</span></span>

<span data-ttu-id="9efde-2763">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="9efde-2763">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-2764">Keyvault</span><span class="sxs-lookup"><span data-stu-id="9efde-2764">Keyvault</span></span>

* <span data-ttu-id="9efde-2765">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2765">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="9efde-2766">Sf</span><span class="sxs-lookup"><span data-stu-id="9efde-2766">Sf</span></span>

* <span data-ttu-id="9efde-2767">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="9efde-2767">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2768">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2768">Storage</span></span>

* <span data-ttu-id="9efde-2769">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="9efde-2769">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="9efde-2770">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="9efde-2770">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="9efde-2771">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2771">August 28, 2017</span></span>

<span data-ttu-id="9efde-2772">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="9efde-2772">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="9efde-2773">CLI</span><span class="sxs-lookup"><span data-stu-id="9efde-2773">CLI</span></span>

* <span data-ttu-id="9efde-2774">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="9efde-2774">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2775">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2775">ACS</span></span>

* <span data-ttu-id="9efde-2776">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-2776">Corrected preview regions</span></span>
* <span data-ttu-id="9efde-2777">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="9efde-2777">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="9efde-2778">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="9efde-2778">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2779">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2779">Appservice</span></span>

* <span data-ttu-id="9efde-2780">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2780">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="9efde-2781">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2781">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="9efde-2782">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2782">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="9efde-2783">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="9efde-2783">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="9efde-2784">Solucionado: la configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="9efde-2784">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-2785">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-2785">IoT</span></span>

* <span data-ttu-id="9efde-2786">Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="9efde-2786">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2787">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2787">Network</span></span>

* <span data-ttu-id="9efde-2788">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="9efde-2788">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="9efde-2789">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="9efde-2789">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="9efde-2790">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2790">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="9efde-2791">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2791">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="9efde-2792">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2792">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2793">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2793">Profile</span></span>

* <span data-ttu-id="9efde-2794">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="9efde-2794">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9efde-2795">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9efde-2795">Service Fabric</span></span>

* <span data-ttu-id="9efde-2796">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-2796">Preview release</span></span>
* <span data-ttu-id="9efde-2797">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="9efde-2797">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="9efde-2798">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="9efde-2798">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="9efde-2799">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2799">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2800">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2800">Storage</span></span>

* <span data-ttu-id="9efde-2801">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="9efde-2801">Enabled setting blob tier</span></span>
* <span data-ttu-id="9efde-2802">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="9efde-2802">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="9efde-2803">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2803">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="9efde-2804">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="9efde-2804">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="9efde-2805">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="9efde-2805">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="9efde-2806">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="9efde-2806">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2807">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2807">VM</span></span>

* <span data-ttu-id="9efde-2808">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2808">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="9efde-2809">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2809">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="9efde-2810">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2810">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="9efde-2811">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="9efde-2811">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="9efde-2812">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="9efde-2812">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="9efde-2813">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2813">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="9efde-2814">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2814">August 15, 2017</span></span>

<span data-ttu-id="9efde-2815">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="9efde-2815">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2816">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2816">ACS</span></span>

* <span data-ttu-id="9efde-2817">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="9efde-2817">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2818">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2818">Appservice</span></span>

* <span data-ttu-id="9efde-2819">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="9efde-2819">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="9efde-2820">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9efde-2820">Event Grid</span></span>

* <span data-ttu-id="9efde-2821">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="9efde-2821">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="9efde-2822">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2822">August 11, 2017</span></span>

<span data-ttu-id="9efde-2823">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="9efde-2823">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2824">ACS</span></span>

* <span data-ttu-id="9efde-2825">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-2825">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-2826">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-2826">Batch</span></span>

* <span data-ttu-id="9efde-2827">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="9efde-2827">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="9efde-2828">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="9efde-2828">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="9efde-2829">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="9efde-2829">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="9efde-2830">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="9efde-2830">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="9efde-2831">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="9efde-2831">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="9efde-2832">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="9efde-2832">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="9efde-2833">Componente</span><span class="sxs-lookup"><span data-stu-id="9efde-2833">Component</span></span>

* <span data-ttu-id="9efde-2834">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="9efde-2834">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="9efde-2835">Contenedor</span><span class="sxs-lookup"><span data-stu-id="9efde-2835">Container</span></span>

* <span data-ttu-id="9efde-2836">`create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="9efde-2836">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="9efde-2837">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9efde-2837">Data Lake Store</span></span>

* <span data-ttu-id="9efde-2838">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="9efde-2838">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="9efde-2839">Event Grid</span><span class="sxs-lookup"><span data-stu-id="9efde-2839">Event Grid</span></span>

* <span data-ttu-id="9efde-2840">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="9efde-2840">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2841">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2841">Network</span></span>

* <span data-ttu-id="9efde-2842">`lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="9efde-2842">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="9efde-2843">`application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2843">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="9efde-2844">`application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="9efde-2844">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="9efde-2845">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2845">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2846">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2846">Profile</span></span>

* <span data-ttu-id="9efde-2847">`account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="9efde-2847">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-2848">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-2848">Storage</span></span>

* <span data-ttu-id="9efde-2849">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="9efde-2849">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-2850">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-2850">VM</span></span>

* <span data-ttu-id="9efde-2851">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="9efde-2851">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="9efde-2852">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2852">Exposed `list-skus` command</span></span>
* <span data-ttu-id="9efde-2853">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="9efde-2853">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="9efde-2854">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="9efde-2854">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="9efde-2855">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="9efde-2855">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="9efde-2856">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-2856">July 28, 2017</span></span>

<span data-ttu-id="9efde-2857">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="9efde-2857">Version 2.0.12</span></span>

* <span data-ttu-id="9efde-2858">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="9efde-2858">Added container commands</span></span>
* <span data-ttu-id="9efde-2859">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="9efde-2859">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="9efde-2860">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-2860">Core</span></span>

* <span data-ttu-id="9efde-2861">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="9efde-2861">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="9efde-2862">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="9efde-2862">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="9efde-2863">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="9efde-2863">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="9efde-2864">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="9efde-2864">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="9efde-2865">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="9efde-2865">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="9efde-2866">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="9efde-2866">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="9efde-2867">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="9efde-2867">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9efde-2868">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="9efde-2868">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="9efde-2869">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="9efde-2869">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="9efde-2870">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="9efde-2870">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="9efde-2871">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="9efde-2871">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="9efde-2872">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="9efde-2872">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="9efde-2873">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2873">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="9efde-2874">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2874">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="9efde-2875">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="9efde-2875">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="9efde-2876">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="9efde-2876">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="9efde-2877">ACR</span><span class="sxs-lookup"><span data-stu-id="9efde-2877">ACR</span></span>

* <span data-ttu-id="9efde-2878">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="9efde-2878">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="9efde-2879">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="9efde-2879">Support SKU update for managed registries</span></span>
* <span data-ttu-id="9efde-2880">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2880">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="9efde-2881">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="9efde-2881">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="9efde-2882">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="9efde-2882">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="9efde-2883">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="9efde-2883">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-2884">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-2884">ACS</span></span>

* <span data-ttu-id="9efde-2885">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="9efde-2885">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-2886">Appservice</span><span class="sxs-lookup"><span data-stu-id="9efde-2886">Appservice</span></span>

* <span data-ttu-id="9efde-2887">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="9efde-2887">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="9efde-2888">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="9efde-2888">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="9efde-2889">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2889">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="9efde-2890">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="9efde-2890">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="9efde-2891">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="9efde-2891">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="9efde-2892">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="9efde-2892">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="9efde-2893">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="9efde-2893">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="9efde-2894">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="9efde-2894">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="9efde-2895">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="9efde-2895">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="9efde-2896">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="9efde-2896">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="9efde-2897">Batch</span><span class="sxs-lookup"><span data-stu-id="9efde-2897">Batch</span></span>

* <span data-ttu-id="9efde-2898">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="9efde-2898">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="9efde-2899">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2899">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="9efde-2900">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2900">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="9efde-2901">CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-2901">CDN</span></span>

* <span data-ttu-id="9efde-2902">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="9efde-2902">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="9efde-2903">Nube</span><span class="sxs-lookup"><span data-stu-id="9efde-2903">Cloud</span></span>

* <span data-ttu-id="9efde-2904">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="9efde-2904">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="9efde-2905">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="9efde-2905">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="9efde-2906">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="9efde-2906">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="9efde-2907">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="9efde-2907">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="9efde-2908">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2908">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-2909">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-2909">CosmosDB</span></span>

* <span data-ttu-id="9efde-2910">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="9efde-2910">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="9efde-2911">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="9efde-2911">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9efde-2912">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9efde-2912">Data Lake Analytics</span></span>

* <span data-ttu-id="9efde-2913">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2913">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="9efde-2914">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2914">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="9efde-2915">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2915">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9efde-2916">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9efde-2916">Data Lake Store</span></span>

* <span data-ttu-id="9efde-2917">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2917">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="9efde-2918">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="9efde-2918">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="9efde-2919">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2919">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="9efde-2920">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="9efde-2920">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="9efde-2921">Interactive</span><span class="sxs-lookup"><span data-stu-id="9efde-2921">Interactive</span></span>

* <span data-ttu-id="9efde-2922">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="9efde-2922">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="9efde-2923">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2923">Increased test coverage</span></span>
* <span data-ttu-id="9efde-2924">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="9efde-2924">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="9efde-2925">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="9efde-2925">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="9efde-2926">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="9efde-2926">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="9efde-2927">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="9efde-2927">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="9efde-2928">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="9efde-2928">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="9efde-2929">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2929">Added `--progress` flag</span></span>
* <span data-ttu-id="9efde-2930">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="9efde-2930">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="9efde-2931">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="9efde-2931">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="9efde-2932">IoT</span><span class="sxs-lookup"><span data-stu-id="9efde-2932">IoT</span></span>

* <span data-ttu-id="9efde-2933">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="9efde-2933">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="9efde-2934">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="9efde-2934">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="9efde-2935">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="9efde-2935">Key vault</span></span>

* <span data-ttu-id="9efde-2936">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="9efde-2936">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="9efde-2937">Subcomandos de `keyvault``purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9efde-2937">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="9efde-2938">Subcomandos de `keyvault secret``backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9efde-2938">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9efde-2939">Subcomandos de `keyvault certificate``purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9efde-2939">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="9efde-2940">Subcomandos de `keyvault key``purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="9efde-2940">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="9efde-2941">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="9efde-2941">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="9efde-2942">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="9efde-2942">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="9efde-2943">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="9efde-2943">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="9efde-2944">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-2944">Lab</span></span>

* <span data-ttu-id="9efde-2945">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2945">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="9efde-2946">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2946">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-2947">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-2947">Monitor</span></span>

* <span data-ttu-id="9efde-2948">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="9efde-2948">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="9efde-2949">Cambio de nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="9efde-2949">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="9efde-2950">Cambio de nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="9efde-2950">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="9efde-2951">Cambio de nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="9efde-2951">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="9efde-2952">Cambio de nombre de `monitor alert-rules` a `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="9efde-2952">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="9efde-2953">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="9efde-2953">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="9efde-2954">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="9efde-2954">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="9efde-2955">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2955">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="9efde-2956">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="9efde-2956">`location` no longer required</span></span>
  * <span data-ttu-id="9efde-2957">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="9efde-2957">Add name and ID support for target</span></span>
  * <span data-ttu-id="9efde-2958">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2958">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="9efde-2959">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="9efde-2959">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="9efde-2960">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="9efde-2960">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="9efde-2961">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="9efde-2961">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="9efde-2962">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2962">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="9efde-2963">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="9efde-2963">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="9efde-2964">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-2964">Network</span></span>

* <span data-ttu-id="9efde-2965">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2965">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="9efde-2966">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2966">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="9efde-2967">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="9efde-2967">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="9efde-2968">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="9efde-2968">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="9efde-2969">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2969">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="9efde-2970">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2970">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="9efde-2971">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="9efde-2971">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="9efde-2972">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="9efde-2972">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="9efde-2973">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="9efde-2973">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="9efde-2974">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="9efde-2974">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="9efde-2975">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="9efde-2975">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="9efde-2976">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2976">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="9efde-2977">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="9efde-2977">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="9efde-2978">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2978">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="9efde-2979">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2979">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="9efde-2980">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2980">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="9efde-2981">Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.</span><span class="sxs-lookup"><span data-stu-id="9efde-2981">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="9efde-2982">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2982">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="9efde-2983">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2983">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="9efde-2984">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2984">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="9efde-2985">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2985">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="9efde-2986">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2986">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="9efde-2987">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="9efde-2987">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="9efde-2988">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="9efde-2988">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="9efde-2989">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="9efde-2989">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="9efde-2990">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="9efde-2990">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="9efde-2991">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="9efde-2991">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-2992">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-2992">Profile</span></span>

* <span data-ttu-id="9efde-2993">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="9efde-2993">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="9efde-2994">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="9efde-2994">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="9efde-2995">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="9efde-2995">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="9efde-2996">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="9efde-2996">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="9efde-2997">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="9efde-2997">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="9efde-2998">RDBMS</span><span class="sxs-lookup"><span data-stu-id="9efde-2998">RDBMS</span></span>

* <span data-ttu-id="9efde-2999">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="9efde-2999">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="9efde-3000">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="9efde-3000">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="9efde-3001">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="9efde-3001">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="9efde-3002">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="9efde-3002">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-3003">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-3003">Resource</span></span>

* <span data-ttu-id="9efde-3004">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3004">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="9efde-3005">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3005">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="9efde-3006">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3006">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="9efde-3007">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3007">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="9efde-3008">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="9efde-3008">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="9efde-3009">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3009">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="9efde-3010">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="9efde-3010">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="9efde-3011">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3011">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="9efde-3012">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-3012">Role</span></span>

* <span data-ttu-id="9efde-3013">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="9efde-3013">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="9efde-3014">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="9efde-3014">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="9efde-3015">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3015">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="9efde-3016">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3016">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="9efde-3017">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3017">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="9efde-3018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9efde-3018">Service Fabric</span></span>
* <span data-ttu-id="9efde-3019">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="9efde-3019">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="9efde-3020">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="9efde-3020">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="9efde-3021">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="9efde-3021">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-3022">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-3022">SQL</span></span>

* <span data-ttu-id="9efde-3023">Se eliminó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="9efde-3023">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="9efde-3024">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3024">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="9efde-3025">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="9efde-3025">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-3026">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-3026">Storage</span></span>

* <span data-ttu-id="9efde-3027">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="9efde-3027">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="9efde-3028">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="9efde-3028">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="9efde-3029">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="9efde-3029">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="9efde-3030">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="9efde-3030">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="9efde-3031">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="9efde-3031">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="9efde-3032">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="9efde-3032">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-3033">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-3033">VM</span></span>

* <span data-ttu-id="9efde-3034">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="9efde-3034">Support configuring nsg</span></span>
* <span data-ttu-id="9efde-3035">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="9efde-3035">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="9efde-3036">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="9efde-3036">Support managed service identities</span></span>
* <span data-ttu-id="9efde-3037">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="9efde-3037">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="9efde-3038">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="9efde-3038">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="9efde-3039">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-3039">May 10, 2017</span></span>

<span data-ttu-id="9efde-3040">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="9efde-3040">Version 2.0.6</span></span>

* <span data-ttu-id="9efde-3041">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="9efde-3041">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="9efde-3042">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="9efde-3042">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="9efde-3043">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9efde-3043">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="9efde-3044">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="9efde-3044">Include Cognitive Services module</span></span>
* <span data-ttu-id="9efde-3045">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="9efde-3045">Include Service Fabric module</span></span>
* <span data-ttu-id="9efde-3046">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="9efde-3046">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="9efde-3047">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="9efde-3047">Add support for CDN commands</span></span>
* <span data-ttu-id="9efde-3048">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="9efde-3048">Remove Container module</span></span>
* <span data-ttu-id="9efde-3049">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="9efde-3049">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="9efde-3050">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="9efde-3050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="9efde-3051">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-3051">Core</span></span>

* <span data-ttu-id="9efde-3052">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="9efde-3052">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="9efde-3053">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="9efde-3053">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="9efde-3054">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="9efde-3054">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="9efde-3055">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="9efde-3055">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="9efde-3056">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="9efde-3056">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="9efde-3057">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="9efde-3057">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="9efde-3058">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="9efde-3058">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="9efde-3059">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="9efde-3059">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="9efde-3060">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="9efde-3060">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="9efde-3061">core: rendimiento mejorado.</span><span class="sxs-lookup"><span data-stu-id="9efde-3061">core: Improved performance</span></span>
* <span data-ttu-id="9efde-3062">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="9efde-3062">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="9efde-3063">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="9efde-3063">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-3064">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-3064">ACS</span></span>

* <span data-ttu-id="9efde-3065">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="9efde-3065">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="9efde-3066">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="9efde-3066">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="9efde-3067">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="9efde-3067">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="9efde-3068">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="9efde-3068">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-3069">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-3069">AppService</span></span>

* <span data-ttu-id="9efde-3070">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="9efde-3070">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="9efde-3071">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="9efde-3071">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="9efde-3072">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="9efde-3072">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="9efde-3073">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="9efde-3073">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="9efde-3074">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="9efde-3074">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="9efde-3075">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="9efde-3075">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="9efde-3076">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="9efde-3076">support slot swap with preview</span></span>
* <span data-ttu-id="9efde-3077">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="9efde-3077">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="9efde-3078">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="9efde-3078">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="9efde-3079">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-3079">CosmosDB</span></span>

* <span data-ttu-id="9efde-3080">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="9efde-3080">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="9efde-3081">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="9efde-3081">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="9efde-3082">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="9efde-3082">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="9efde-3083">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="9efde-3083">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="9efde-3084">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9efde-3084">Data Lake Analytics</span></span>

* <span data-ttu-id="9efde-3085">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="9efde-3085">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="9efde-3086">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="9efde-3086">Add support for new catalog item type: package.</span></span> <span data-ttu-id="9efde-3087">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="9efde-3087">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="9efde-3088">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="9efde-3088">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="9efde-3089">Tabla</span><span class="sxs-lookup"><span data-stu-id="9efde-3089">Table</span></span>
  * <span data-ttu-id="9efde-3090">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="9efde-3090">Table valued function</span></span>
  * <span data-ttu-id="9efde-3091">Ver</span><span class="sxs-lookup"><span data-stu-id="9efde-3091">View</span></span>
  * <span data-ttu-id="9efde-3092">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="9efde-3092">Table Statistics.</span></span> <span data-ttu-id="9efde-3093">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="9efde-3093">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="9efde-3094">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9efde-3094">Data Lake Store</span></span>

* <span data-ttu-id="9efde-3095">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="9efde-3095">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="9efde-3096">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="9efde-3096">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="9efde-3097">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="9efde-3097">missed help for access show.</span></span> <span data-ttu-id="9efde-3098">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="9efde-3098">adding it.</span></span> <span data-ttu-id="9efde-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="9efde-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="9efde-3100">Buscar</span><span class="sxs-lookup"><span data-stu-id="9efde-3100">Find</span></span>

* <span data-ttu-id="9efde-3101">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="9efde-3101">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="9efde-3102">KeyVault</span><span class="sxs-lookup"><span data-stu-id="9efde-3102">KeyVault</span></span>

* <span data-ttu-id="9efde-3103">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="9efde-3103">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="9efde-3104">BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="9efde-3104">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="9efde-3105">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="9efde-3105">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="9efde-3106">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="9efde-3106">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="9efde-3107">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="9efde-3107">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="9efde-3108">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-3108">Lab</span></span>

* <span data-ttu-id="9efde-3109">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-3109">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="9efde-3110">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-3110">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="9efde-3111">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-3111">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="9efde-3112">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-3112">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="9efde-3113">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="9efde-3113">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="9efde-3114">Supervisión</span><span class="sxs-lookup"><span data-stu-id="9efde-3114">Monitor</span></span>

* <span data-ttu-id="9efde-3115">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="9efde-3115">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="9efde-3116">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="9efde-3116">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="9efde-3117">Red</span><span class="sxs-lookup"><span data-stu-id="9efde-3117">Network</span></span>

* <span data-ttu-id="9efde-3118">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="9efde-3118">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="9efde-3119">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="9efde-3119">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="9efde-3120">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9efde-3120">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="9efde-3121">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="9efde-3121">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="9efde-3122">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="9efde-3122">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="9efde-3123">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9efde-3123">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="9efde-3124">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="9efde-3124">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="9efde-3125">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="9efde-3125">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="9efde-3126">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="9efde-3126">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="9efde-3127">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="9efde-3127">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="9efde-3128">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="9efde-3128">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="9efde-3129">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="9efde-3129">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="9efde-3130">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="9efde-3130">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="9efde-3131">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="9efde-3131">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="9efde-3132">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="9efde-3132">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="9efde-3133">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="9efde-3133">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="9efde-3134">Perfil</span><span class="sxs-lookup"><span data-stu-id="9efde-3134">Profile</span></span>

* <span data-ttu-id="9efde-3135">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="9efde-3135">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="9efde-3136">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="9efde-3136">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="9efde-3137">Redis</span><span class="sxs-lookup"><span data-stu-id="9efde-3137">Redis</span></span>

* <span data-ttu-id="9efde-3138">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="9efde-3138">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="9efde-3139">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="9efde-3139">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="9efde-3140">Resource</span><span class="sxs-lookup"><span data-stu-id="9efde-3140">Resource</span></span>

* <span data-ttu-id="9efde-3141">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="9efde-3141">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="9efde-3142">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="9efde-3142">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="9efde-3143">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="9efde-3143">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="9efde-3144">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="9efde-3144">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="9efde-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="9efde-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="9efde-3146">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="9efde-3146">Add docs for az lock update.</span></span> <span data-ttu-id="9efde-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="9efde-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="9efde-3148">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="9efde-3148">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="9efde-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="9efde-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="9efde-3150">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="9efde-3150">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="9efde-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="9efde-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="9efde-3152">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="9efde-3152">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="9efde-3153">Role</span><span class="sxs-lookup"><span data-stu-id="9efde-3153">Role</span></span>

* <span data-ttu-id="9efde-3154">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="9efde-3154">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="9efde-3155">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="9efde-3155">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="9efde-3156">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="9efde-3156">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="9efde-3157">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="9efde-3157">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="9efde-3158">SQL</span><span class="sxs-lookup"><span data-stu-id="9efde-3158">SQL</span></span>

* <span data-ttu-id="9efde-3159">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="9efde-3159">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="9efde-3160">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="9efde-3160">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="9efde-3161">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-3161">Storage</span></span>

* <span data-ttu-id="9efde-3162">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="9efde-3162">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="9efde-3163">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="9efde-3163">Add support for incremental blob copy</span></span>
* <span data-ttu-id="9efde-3164">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="9efde-3164">Add support for large block blob upload</span></span>
* <span data-ttu-id="9efde-3165">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="9efde-3165">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-3166">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-3166">VM</span></span>

* <span data-ttu-id="9efde-3167">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="9efde-3167">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="9efde-3168">nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="9efde-3168">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="9efde-3169">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="9efde-3169">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="9efde-3170">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="9efde-3170">az vm/vmss disk</span></span>
  3. <span data-ttu-id="9efde-3171">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="9efde-3171">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="9efde-3172">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="9efde-3172">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="9efde-3173">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="9efde-3173">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="9efde-3174">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-3174">April 3, 2017</span></span>

<span data-ttu-id="9efde-3175">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="9efde-3175">Version 2.0.2</span></span>

<span data-ttu-id="9efde-3176">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="9efde-3176">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="9efde-3177">Core</span><span class="sxs-lookup"><span data-stu-id="9efde-3177">Core</span></span>

* <span data-ttu-id="9efde-3178">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="9efde-3178">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="9efde-3179">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="9efde-3179">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="9efde-3180">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="9efde-3180">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="9efde-3181">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9efde-3181">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9efde-3182">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="9efde-3182">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="9efde-3183">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="9efde-3183">Add prompting for missing template parameters.</span></span> <span data-ttu-id="9efde-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="9efde-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="9efde-3185">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="9efde-3185">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="9efde-3186">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="9efde-3186">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="9efde-3187">ACS</span><span class="sxs-lookup"><span data-stu-id="9efde-3187">ACS</span></span>

* <span data-ttu-id="9efde-3188">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="9efde-3188">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="9efde-3189">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="9efde-3189">Add support for ssh key password prompting.</span></span> <span data-ttu-id="9efde-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="9efde-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="9efde-3191">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="9efde-3191">Add support for windows clusters.</span></span> <span data-ttu-id="9efde-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="9efde-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="9efde-3193">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="9efde-3193">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="9efde-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="9efde-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="9efde-3195">AppService</span><span class="sxs-lookup"><span data-stu-id="9efde-3195">AppService</span></span>

* <span data-ttu-id="9efde-3196">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="9efde-3196">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="9efde-3197">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="9efde-3197">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="9efde-3198">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="9efde-3198">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="9efde-3199">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="9efde-3199">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="9efde-3200">DataLake</span><span class="sxs-lookup"><span data-stu-id="9efde-3200">DataLake</span></span>

* <span data-ttu-id="9efde-3201">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="9efde-3201">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="9efde-3202">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="9efde-3202">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="9efde-3203">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="9efde-3203">DocuemntDB</span></span>

* <span data-ttu-id="9efde-3204">DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="9efde-3204">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="9efde-3205">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="9efde-3205">VM</span></span>

* <span data-ttu-id="9efde-3206">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="9efde-3206">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="9efde-3207">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="9efde-3207">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="9efde-3208">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="9efde-3208">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="9efde-3209">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="9efde-3209">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="9efde-3210">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="9efde-3210">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="9efde-3211">Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span><span class="sxs-lookup"><span data-stu-id="9efde-3211">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="9efde-3212">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="9efde-3212">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="9efde-3213">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="9efde-3213">February 27, 2017</span></span>

<span data-ttu-id="9efde-3214">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="9efde-3214">Version 2.0.0</span></span>

<span data-ttu-id="9efde-3215">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="9efde-3215">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="9efde-3216">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="9efde-3216">Container Service (acs)</span></span>
- <span data-ttu-id="9efde-3217">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="9efde-3217">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="9efde-3218">Redes</span><span class="sxs-lookup"><span data-stu-id="9efde-3218">Networking</span></span>
- <span data-ttu-id="9efde-3219">Storage</span><span class="sxs-lookup"><span data-stu-id="9efde-3219">Storage</span></span>

<span data-ttu-id="9efde-3220">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="9efde-3220">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="9efde-3221">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="9efde-3221">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="9efde-3222">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="9efde-3222">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="9efde-3223">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="9efde-3223">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="9efde-3224">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="9efde-3224">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="9efde-3225">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="9efde-3225">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="9efde-3226">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="9efde-3226">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="9efde-3227">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="9efde-3227">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="9efde-3228">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="9efde-3228">Provide feedback from the command line with the `az feedback` command</span></span>

