---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 10/09/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 0aec9dce0eda007c71df3693b39c7ec8cc9856cd
ms.sourcegitcommit: 0fc354c24454f5c9c5ff4b7296ad7b18ffdf31b1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/10/2018
ms.locfileid: "48904793"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="d2dde-103">Notas de la versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="d2dde-103">Azure CLI release notes</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="d2dde-104">9 de octubre de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-104">October 9, 2018</span></span>

<span data-ttu-id="d2dde-105">Versión 2.0.47</span><span class="sxs-lookup"><span data-stu-id="d2dde-105">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-106">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-106">Core</span></span>
* <span data-ttu-id="d2dde-107">Ha mejorado el control de errores para los errores de "Solicitud incorrecta"</span><span class="sxs-lookup"><span data-stu-id="d2dde-107">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-108">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-108">ACR</span></span>
* <span data-ttu-id="d2dde-109">Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm</span><span class="sxs-lookup"><span data-stu-id="d2dde-109">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-110">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-110">ACS</span></span>
* <span data-ttu-id="d2dde-111">Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1</span><span class="sxs-lookup"><span data-stu-id="d2dde-111">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="d2dde-112">Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko</span><span class="sxs-lookup"><span data-stu-id="d2dde-112">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="d2dde-113">Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante</span><span class="sxs-lookup"><span data-stu-id="d2dde-113">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="d2dde-114">Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas</span><span class="sxs-lookup"><span data-stu-id="d2dde-114">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-115">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-115">Container</span></span>
* <span data-ttu-id="d2dde-116">Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico</span><span class="sxs-lookup"><span data-stu-id="d2dde-116">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="d2dde-117">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows</span><span class="sxs-lookup"><span data-stu-id="d2dde-117">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="d2dde-118">Centro de eventos</span><span class="sxs-lookup"><span data-stu-id="d2dde-118">Event Hub</span></span>
* <span data-ttu-id="d2dde-119">Se ha corregido el comando `eventhub update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-119">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="d2dde-120">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="d2dde-120">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="d2dde-121">Extensiones</span><span class="sxs-lookup"><span data-stu-id="d2dde-121">Extensions</span></span>
* <span data-ttu-id="d2dde-122">Se ha corregido un problema al intentar agregar una extensión que ya está instalada</span><span class="sxs-lookup"><span data-stu-id="d2dde-122">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="d2dde-123">HDInsight</span><span class="sxs-lookup"><span data-stu-id="d2dde-123">HDInsight</span></span>
* <span data-ttu-id="d2dde-124">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d2dde-124">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-125">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-125">IoT</span></span>
* <span data-ttu-id="d2dde-126">Se ha agregado un comando de instalación de extensiones al banner de primera ejecución</span><span class="sxs-lookup"><span data-stu-id="d2dde-126">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-127">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d2dde-127">KeyVault</span></span>
* <span data-ttu-id="d2dde-128">Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente</span><span class="sxs-lookup"><span data-stu-id="d2dde-128">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-129">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-129">Network</span></span>
* <span data-ttu-id="d2dde-130">Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada.</span><span class="sxs-lookup"><span data-stu-id="d2dde-130">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="d2dde-131">Consulte el número 6052</span><span class="sxs-lookup"><span data-stu-id="d2dde-131">See #6052</span></span>
* <span data-ttu-id="d2dde-132">`--remote-vnet-id` en desuso para `network vnet peering create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-132">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="d2dde-133">Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador</span><span class="sxs-lookup"><span data-stu-id="d2dde-133">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="d2dde-134">Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d2dde-134">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="d2dde-135">Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`</span><span class="sxs-lookup"><span data-stu-id="d2dde-135">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="d2dde-136">Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`</span><span class="sxs-lookup"><span data-stu-id="d2dde-136">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="d2dde-137">Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-137">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-138">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-138">Role</span></span>
* <span data-ttu-id="d2dde-139">Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`</span><span class="sxs-lookup"><span data-stu-id="d2dde-139">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="d2dde-140">Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`</span><span class="sxs-lookup"><span data-stu-id="d2dde-140">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="d2dde-141">Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos</span><span class="sxs-lookup"><span data-stu-id="d2dde-141">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="d2dde-142">Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"</span><span class="sxs-lookup"><span data-stu-id="d2dde-142">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="d2dde-143">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="d2dde-143">Service Bus</span></span>
* <span data-ttu-id="d2dde-144">[CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía</span><span class="sxs-lookup"><span data-stu-id="d2dde-144">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-145">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-145">VM</span></span>
* <span data-ttu-id="d2dde-146">Se ha corregido el campo `accessSas` vacío en `disk grant-access`</span><span class="sxs-lookup"><span data-stu-id="d2dde-146">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="d2dde-147">Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso</span><span class="sxs-lookup"><span data-stu-id="d2dde-147">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="d2dde-148">Se ha corregido los comandos de actualización de `sig`</span><span class="sxs-lookup"><span data-stu-id="d2dde-148">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="d2dde-149">Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`</span><span class="sxs-lookup"><span data-stu-id="d2dde-149">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="d2dde-150">Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="d2dde-150">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="d2dde-151">Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible</span><span class="sxs-lookup"><span data-stu-id="d2dde-151">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="d2dde-152">21 de septiembre de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-152">September 21, 2018</span></span>

<span data-ttu-id="d2dde-153">Versión 2.0.46</span><span class="sxs-lookup"><span data-stu-id="d2dde-153">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-154">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-154">ACR</span></span>
* <span data-ttu-id="d2dde-155">Se han agregado comandos de tareas de ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-155">Added ACR Task commands</span></span>
* <span data-ttu-id="d2dde-156">Se ha agregado un comando de ejecución rápida</span><span class="sxs-lookup"><span data-stu-id="d2dde-156">Added quick run command</span></span>
* <span data-ttu-id="d2dde-157">Grupo de comandos `build-task` en desuso</span><span class="sxs-lookup"><span data-stu-id="d2dde-157">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="d2dde-158">Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-158">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="d2dde-159">Se ha agregado compatibilidad para la creación idempotente de un Registro administrado</span><span class="sxs-lookup"><span data-stu-id="d2dde-159">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="d2dde-160">Se ha agregado una marca sin formato para mostrar los registros de compilación</span><span class="sxs-lookup"><span data-stu-id="d2dde-160">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-161">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-161">ACS</span></span>
* <span data-ttu-id="d2dde-162">Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS</span><span class="sxs-lookup"><span data-stu-id="d2dde-162">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="d2dde-163">Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment</span><span class="sxs-lookup"><span data-stu-id="d2dde-163">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-164">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-164">AppService</span></span>

* <span data-ttu-id="d2dde-165">Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)</span><span class="sxs-lookup"><span data-stu-id="d2dde-165">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="d2dde-166">az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show</span><span class="sxs-lookup"><span data-stu-id="d2dde-166">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="d2dde-167">Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="d2dde-167">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="d2dde-168">Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas</span><span class="sxs-lookup"><span data-stu-id="d2dde-168">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-169">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-169">Batch</span></span>
* <span data-ttu-id="d2dde-170">Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter</span><span class="sxs-lookup"><span data-stu-id="d2dde-170">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="d2dde-171">Se ha actualizado la documentación de los formatos de `--json-file` aceptados</span><span class="sxs-lookup"><span data-stu-id="d2dde-171">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="d2dde-172">Se ha agregado `--max-tasks-per-node-option` a `batch pool create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-172">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="d2dde-173">Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción</span><span class="sxs-lookup"><span data-stu-id="d2dde-173">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d2dde-174">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d2dde-174">Batch AI</span></span> 
* <span data-ttu-id="d2dde-175">Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-175">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d2dde-176">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d2dde-176">Cognitive Services</span></span>
* <span data-ttu-id="d2dde-177">Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`</span><span class="sxs-lookup"><span data-stu-id="d2dde-177">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="d2dde-178">Se ha agregado el comando `cognitiveservices account list-usage`</span><span class="sxs-lookup"><span data-stu-id="d2dde-178">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="d2dde-179">Se ha agregado el comando `cognitiveservices account list-kinds`</span><span class="sxs-lookup"><span data-stu-id="d2dde-179">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="d2dde-180">Se ha agregado el comando `cognitiveservices account list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-180">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="d2dde-181">`cognitiveservices list` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-181">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="d2dde-182">Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`</span><span class="sxs-lookup"><span data-stu-id="d2dde-182">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-183">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-183">Container</span></span>
* <span data-ttu-id="d2dde-184">Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución</span><span class="sxs-lookup"><span data-stu-id="d2dde-184">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="d2dde-185">Se ha agregado `--network-profile` para pasar un perfil de red</span><span class="sxs-lookup"><span data-stu-id="d2dde-185">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="d2dde-186">Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-186">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="d2dde-187">Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d2dde-187">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="d2dde-188">DataLake</span><span class="sxs-lookup"><span data-stu-id="d2dde-188">Datalake</span></span>
* <span data-ttu-id="d2dde-189">Se han agregado comandos para las reglas de red virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-189">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="d2dde-190">Shell interactivo</span><span class="sxs-lookup"><span data-stu-id="d2dde-190">Interactive Shell</span></span>
* <span data-ttu-id="d2dde-191">Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente</span><span class="sxs-lookup"><span data-stu-id="d2dde-191">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="d2dde-192">Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso</span><span class="sxs-lookup"><span data-stu-id="d2dde-192">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-193">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-193">IoT</span></span>
* <span data-ttu-id="d2dde-194">Se ha agregado compatibilidad para el enrutamiento de centros de IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-194">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="d2dde-195">Key Vault</span><span class="sxs-lookup"><span data-stu-id="d2dde-195">Key Vault</span></span>
* <span data-ttu-id="d2dde-196">Se ha corregido la importación de claves de Key Vault para las claves RSA</span><span class="sxs-lookup"><span data-stu-id="d2dde-196">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-197">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-197">Network</span></span>
* <span data-ttu-id="d2dde-198">Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas</span><span class="sxs-lookup"><span data-stu-id="d2dde-198">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="d2dde-199">Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio</span><span class="sxs-lookup"><span data-stu-id="d2dde-199">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="d2dde-200">Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer</span><span class="sxs-lookup"><span data-stu-id="d2dde-200">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="d2dde-201">Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos</span><span class="sxs-lookup"><span data-stu-id="d2dde-201">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="d2dde-202">Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-202">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="d2dde-203">Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-203">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="d2dde-204">Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos</span><span class="sxs-lookup"><span data-stu-id="d2dde-204">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="d2dde-205">Se agrega el comando `network watcher run-configuration-diagnostic`</span><span class="sxs-lookup"><span data-stu-id="d2dde-205">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="d2dde-206">Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`</span><span class="sxs-lookup"><span data-stu-id="d2dde-206">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="d2dde-207">`network express-route create/update`: se ha agregado la marca `--allow-global-reach`</span><span class="sxs-lookup"><span data-stu-id="d2dde-207">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="d2dde-208">`network vnet subnet create/update`: se ha agregado compatibilidad para `--delegation`</span><span class="sxs-lookup"><span data-stu-id="d2dde-208">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="d2dde-209">Se agregó el comando `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-209">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="d2dde-210">`network traffic-manager profile create/update`: se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` a Monitor Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`</span><span class="sxs-lookup"><span data-stu-id="d2dde-210">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="d2dde-211">`network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.</span><span class="sxs-lookup"><span data-stu-id="d2dde-211">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="d2dde-212">`dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`</span><span class="sxs-lookup"><span data-stu-id="d2dde-212">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="d2dde-213">Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta</span><span class="sxs-lookup"><span data-stu-id="d2dde-213">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="d2dde-214">Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red</span><span class="sxs-lookup"><span data-stu-id="d2dde-214">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="d2dde-215">Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="d2dde-215">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="d2dde-216">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d2dde-216">RDBMS</span></span>
* <span data-ttu-id="d2dde-217">Se ha agregado compatibilidad para el servicio MariaDB</span><span class="sxs-lookup"><span data-stu-id="d2dde-217">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="d2dde-218">Reserva</span><span class="sxs-lookup"><span data-stu-id="d2dde-218">Reservation</span></span>
* <span data-ttu-id="d2dde-219">Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados</span><span class="sxs-lookup"><span data-stu-id="d2dde-219">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="d2dde-220">Se ha agregado la propiedad de nombre en el modelo de revisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-220">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="d2dde-221">Administración de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="d2dde-221">Manage App</span></span>
* <span data-ttu-id="d2dde-222">Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado</span><span class="sxs-lookup"><span data-stu-id="d2dde-222">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="d2dde-223">Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos</span><span class="sxs-lookup"><span data-stu-id="d2dde-223">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-224">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-224">Role</span></span>
* <span data-ttu-id="d2dde-225">Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios</span><span class="sxs-lookup"><span data-stu-id="d2dde-225">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="d2dde-226">SignalR</span><span class="sxs-lookup"><span data-stu-id="d2dde-226">SignalR</span></span>
* <span data-ttu-id="d2dde-227">Primera versión</span><span class="sxs-lookup"><span data-stu-id="d2dde-227">First release</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-228">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-228">Storage</span></span>
* <span data-ttu-id="d2dde-229">Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas</span><span class="sxs-lookup"><span data-stu-id="d2dde-229">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="d2dde-230">Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable</span><span class="sxs-lookup"><span data-stu-id="d2dde-230">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-231">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-231">VM</span></span>
* <span data-ttu-id="d2dde-232">Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)</span><span class="sxs-lookup"><span data-stu-id="d2dde-232">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="d2dde-233">Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`</span><span class="sxs-lookup"><span data-stu-id="d2dde-233">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="d2dde-234">28 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-234">August 28, 2018</span></span>

<span data-ttu-id="d2dde-235">Versión 2.0.45</span><span class="sxs-lookup"><span data-stu-id="d2dde-235">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-236">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-236">Core</span></span>

* <span data-ttu-id="d2dde-237">Se ha corregido un problema al cargar el archivo de configuración vacío</span><span class="sxs-lookup"><span data-stu-id="d2dde-237">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="d2dde-238">Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d2dde-238">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-239">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-239">ACR</span></span>

* <span data-ttu-id="d2dde-240">Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM</span><span class="sxs-lookup"><span data-stu-id="d2dde-240">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="d2dde-241">Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`</span><span class="sxs-lookup"><span data-stu-id="d2dde-241">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-242">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-242">ACS</span></span>

* <span data-ttu-id="d2dde-243">Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`</span><span class="sxs-lookup"><span data-stu-id="d2dde-243">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="d2dde-244">Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster</span><span class="sxs-lookup"><span data-stu-id="d2dde-244">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-245">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-245">AppService</span></span>

* <span data-ttu-id="d2dde-246">Se ha agregado compatibilidad con CORS en functionapp y webapp</span><span class="sxs-lookup"><span data-stu-id="d2dde-246">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="d2dde-247">Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-247">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="d2dde-248">Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-248">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="d2dde-249">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="d2dde-249">Backup</span></span>

* <span data-ttu-id="d2dde-250">Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-250">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="d2dde-251">Servicio de bots</span><span class="sxs-lookup"><span data-stu-id="d2dde-251">Bot Service</span></span>

* <span data-ttu-id="d2dde-252">Versión inicial de la CLI del servicio de bots</span><span class="sxs-lookup"><span data-stu-id="d2dde-252">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d2dde-253">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d2dde-253">Cognitive Services</span></span>

* <span data-ttu-id="d2dde-254">Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios</span><span class="sxs-lookup"><span data-stu-id="d2dde-254">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-255">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-255">IoT</span></span>

* <span data-ttu-id="d2dde-256">Se ha corregido un problema con los centros vinculados asociados</span><span class="sxs-lookup"><span data-stu-id="d2dde-256">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-257">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-257">Monitor</span></span>

* <span data-ttu-id="d2dde-258">Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real</span><span class="sxs-lookup"><span data-stu-id="d2dde-258">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="d2dde-259">Comandos `monitor alert` en desuso</span><span class="sxs-lookup"><span data-stu-id="d2dde-259">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-260">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-260">Network</span></span>

* <span data-ttu-id="d2dde-261">Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-261">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-262">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-262">Resource</span></span>

* <span data-ttu-id="d2dde-263">Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-263">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-264">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-264">Storage</span></span>

* <span data-ttu-id="d2dde-265">Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-265">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-266">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-266">VM</span></span>

* <span data-ttu-id="d2dde-267">Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-267">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="d2dde-268">`--storage-caching` en desuso para `vm create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-268">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="d2dde-269">14 de agosto de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-269">Auguest 14, 2018</span></span>

<span data-ttu-id="d2dde-270">Versión 2.0.44</span><span class="sxs-lookup"><span data-stu-id="d2dde-270">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-271">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-271">Core</span></span>

* <span data-ttu-id="d2dde-272">Se ha corregido una presentación numérica en la salida `table`</span><span class="sxs-lookup"><span data-stu-id="d2dde-272">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="d2dde-273">Se ha agregado el formato de salida de YAML</span><span class="sxs-lookup"><span data-stu-id="d2dde-273">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="d2dde-274">Telemetría</span><span class="sxs-lookup"><span data-stu-id="d2dde-274">Telemetry</span></span>

* <span data-ttu-id="d2dde-275">Se han mejorado los informes de telemetría</span><span class="sxs-lookup"><span data-stu-id="d2dde-275">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-276">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-276">ACR</span></span>

* <span data-ttu-id="d2dde-277">Se agregaron los comandos `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-277">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="d2dde-278">Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente</span><span class="sxs-lookup"><span data-stu-id="d2dde-278">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-279">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-279">ACS</span></span>

* <span data-ttu-id="d2dde-280">Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows</span><span class="sxs-lookup"><span data-stu-id="d2dde-280">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="d2dde-281">Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI</span><span class="sxs-lookup"><span data-stu-id="d2dde-281">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="d2dde-282">Se ha cambiado a la asignación de roles a la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="d2dde-282">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="d2dde-283">Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona</span><span class="sxs-lookup"><span data-stu-id="d2dde-283">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="d2dde-284">Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe</span><span class="sxs-lookup"><span data-stu-id="d2dde-284">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="d2dde-285">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-285">AppService</span></span>

* <span data-ttu-id="d2dde-286">Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="d2dde-286">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="d2dde-287">Se ha corregido un bloqueo en la implementación de zip</span><span class="sxs-lookup"><span data-stu-id="d2dde-287">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="d2dde-288">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d2dde-288">BatchAI</span></span>

* <span data-ttu-id="d2dde-289">Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".</span><span class="sxs-lookup"><span data-stu-id="d2dde-289">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="d2dde-290">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-290">Container</span></span>

* <span data-ttu-id="d2dde-291">Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-291">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="d2dde-292">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-292">IoT</span></span>

* <span data-ttu-id="d2dde-293">[CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot</span><span class="sxs-lookup"><span data-stu-id="d2dde-293">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="d2dde-294">Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`</span><span class="sxs-lookup"><span data-stu-id="d2dde-294">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="d2dde-295">Iot Central</span><span class="sxs-lookup"><span data-stu-id="d2dde-295">Iot Central</span></span>

* <span data-ttu-id="d2dde-296">Versión inicial del módulo de IoT Central</span><span class="sxs-lookup"><span data-stu-id="d2dde-296">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-297">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d2dde-297">KeyVault</span></span>


* <span data-ttu-id="d2dde-298">Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas</span><span class="sxs-lookup"><span data-stu-id="d2dde-298">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="d2dde-299">Se han agregado comandos para las reglas de red</span><span class="sxs-lookup"><span data-stu-id="d2dde-299">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="d2dde-300">Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto</span><span class="sxs-lookup"><span data-stu-id="d2dde-300">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="d2dde-301">Se ha agregado compatibilidad para la versión de varias api de administración de KV</span><span class="sxs-lookup"><span data-stu-id="d2dde-301">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="d2dde-302">Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV</span><span class="sxs-lookup"><span data-stu-id="d2dde-302">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="d2dde-303">Retransmisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-303">Relay</span></span>

* <span data-ttu-id="d2dde-304">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d2dde-304">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-305">Sql</span><span class="sxs-lookup"><span data-stu-id="d2dde-305">Sql</span></span>

* <span data-ttu-id="d2dde-306">Se agregaron los comandos `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-306">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-307">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-307">Storage</span></span>

* <span data-ttu-id="d2dde-308">[CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región</span><span class="sxs-lookup"><span data-stu-id="d2dde-308">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="d2dde-309">Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`</span><span class="sxs-lookup"><span data-stu-id="d2dde-309">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="d2dde-310">Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado</span><span class="sxs-lookup"><span data-stu-id="d2dde-310">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="d2dde-311">Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos</span><span class="sxs-lookup"><span data-stu-id="d2dde-311">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="d2dde-312">Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-312">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-313">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-313">VM</span></span>

* <span data-ttu-id="d2dde-314">Se han agregado filtros comunes a `vm list-skus` para facilitar su uso</span><span class="sxs-lookup"><span data-stu-id="d2dde-314">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="d2dde-315">31 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-315">July 31, 2018</span></span>

<span data-ttu-id="d2dde-316">Versión 2.0.43</span><span class="sxs-lookup"><span data-stu-id="d2dde-316">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-317">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-317">ACR</span></span>

* <span data-ttu-id="d2dde-318">Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-318">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="d2dde-319">Se agregó el comando `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-319">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-320">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-320">ACS</span></span>

* <span data-ttu-id="d2dde-321">Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].</span><span class="sxs-lookup"><span data-stu-id="d2dde-321">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-322">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-322">Batch</span></span>

* <span data-ttu-id="d2dde-323">Se ha corregido el error al mostrar el token de AAD en cloudshell.</span><span class="sxs-lookup"><span data-stu-id="d2dde-323">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-324">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-324">Container</span></span>

* <span data-ttu-id="d2dde-325">Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="d2dde-325">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-326">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-326">Network</span></span>

* <span data-ttu-id="d2dde-327">Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d2dde-327">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="d2dde-328">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-328">Resource</span></span>

* <span data-ttu-id="d2dde-329">Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.</span><span class="sxs-lookup"><span data-stu-id="d2dde-329">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="d2dde-330">Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.</span><span class="sxs-lookup"><span data-stu-id="d2dde-330">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-331">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-331">Role</span></span>

* <span data-ttu-id="d2dde-332">Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.</span><span class="sxs-lookup"><span data-stu-id="d2dde-332">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="d2dde-333">Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.</span><span class="sxs-lookup"><span data-stu-id="d2dde-333">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="d2dde-334">Search</span><span class="sxs-lookup"><span data-stu-id="d2dde-334">Search</span></span>

* <span data-ttu-id="d2dde-335">Se han agregado comandos al servicio Azure Search.</span><span class="sxs-lookup"><span data-stu-id="d2dde-335">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="d2dde-336">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="d2dde-336">Service Bus</span></span>

* <span data-ttu-id="d2dde-337">S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.</span><span class="sxs-lookup"><span data-stu-id="d2dde-337">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="d2dde-338">Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.</span><span class="sxs-lookup"><span data-stu-id="d2dde-338">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="d2dde-339">`--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`</span><span class="sxs-lookup"><span data-stu-id="d2dde-339">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="d2dde-340">`--dead-letter-on-filter-exceptions` en `subscriptions`</span><span class="sxs-lookup"><span data-stu-id="d2dde-340">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-341">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-341">Storage</span></span>

* <span data-ttu-id="d2dde-342">Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.</span><span class="sxs-lookup"><span data-stu-id="d2dde-342">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="d2dde-343">Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-343">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-344">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-344">VM</span></span>

* <span data-ttu-id="d2dde-345">Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.</span><span class="sxs-lookup"><span data-stu-id="d2dde-345">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="d2dde-346">Se ha agregado compatibilidad con `StandardSSD_LRS`</span><span class="sxs-lookup"><span data-stu-id="d2dde-346">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="d2dde-347">Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="d2dde-347">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="d2dde-348">[CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.</span><span class="sxs-lookup"><span data-stu-id="d2dde-348">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="d2dde-349">18 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-349">July 18, 2018</span></span>

<span data-ttu-id="d2dde-350">Versión 2.0.42</span><span class="sxs-lookup"><span data-stu-id="d2dde-350">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-351">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-351">Core</span></span>

* <span data-ttu-id="d2dde-352">Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL</span><span class="sxs-lookup"><span data-stu-id="d2dde-352">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="d2dde-353">Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="d2dde-353">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="d2dde-354">[CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-354">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-355">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-355">ACR</span></span>

* <span data-ttu-id="d2dde-356">[CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"</span><span class="sxs-lookup"><span data-stu-id="d2dde-356">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="d2dde-357">Se han agregado los comandos `show` y `update` en el grupo `acr repository`</span><span class="sxs-lookup"><span data-stu-id="d2dde-357">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="d2dde-358">Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada</span><span class="sxs-lookup"><span data-stu-id="d2dde-358">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="d2dde-359">Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen</span><span class="sxs-lookup"><span data-stu-id="d2dde-359">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-360">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-360">ACS</span></span>

* <span data-ttu-id="d2dde-361">Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5</span><span class="sxs-lookup"><span data-stu-id="d2dde-361">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-362">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-362">AppService</span></span>

* <span data-ttu-id="d2dde-363">Se ha agregado compatibilidad con las SKU de PremiumV2</span><span class="sxs-lookup"><span data-stu-id="d2dde-363">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-364">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-364">Batch</span></span>

* <span data-ttu-id="d2dde-365">Se ha corregido el error del uso del credencial de token en el modo de shell en la nube</span><span class="sxs-lookup"><span data-stu-id="d2dde-365">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="d2dde-366">Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas</span><span class="sxs-lookup"><span data-stu-id="d2dde-366">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d2dde-367">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d2dde-367">Batch AI</span></span>

* <span data-ttu-id="d2dde-368">Se ha corregido el comando `az batchai job exec`</span><span class="sxs-lookup"><span data-stu-id="d2dde-368">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-369">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-369">Container</span></span>

* <span data-ttu-id="d2dde-370">Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub</span><span class="sxs-lookup"><span data-stu-id="d2dde-370">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="d2dde-371">Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml</span><span class="sxs-lookup"><span data-stu-id="d2dde-371">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-372">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-372">Network</span></span>

* <span data-ttu-id="d2dde-373">Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-373">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="d2dde-374">Se agregó `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-374">Added `network nic wait`</span></span>
* <span data-ttu-id="d2dde-375">El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso</span><span class="sxs-lookup"><span data-stu-id="d2dde-375">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="d2dde-376">Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-376">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="d2dde-377">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-377">Resource</span></span>

* <span data-ttu-id="d2dde-378">Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d2dde-378">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="d2dde-379">Se ha agregado compatibilidad de `--no-wait` con `deployment delete`</span><span class="sxs-lookup"><span data-stu-id="d2dde-379">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="d2dde-380">Se agregó el comando `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-380">Added `deployment wait` command</span></span>
* <span data-ttu-id="d2dde-381">Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile</span><span class="sxs-lookup"><span data-stu-id="d2dde-381">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-382">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-382">SQL</span></span>

* <span data-ttu-id="d2dde-383">Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-383">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="d2dde-384">Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`</span><span class="sxs-lookup"><span data-stu-id="d2dde-384">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="d2dde-385">Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`</span><span class="sxs-lookup"><span data-stu-id="d2dde-385">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-386">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-386">Storage</span></span>

* <span data-ttu-id="d2dde-387">Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas</span><span class="sxs-lookup"><span data-stu-id="d2dde-387">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-388">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-388">VM</span></span>

* <span data-ttu-id="d2dde-389">[CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado</span><span class="sxs-lookup"><span data-stu-id="d2dde-389">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="d2dde-390">Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-390">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="d2dde-391">Se agregó `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-391">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d2dde-392">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-392">July 3, 2018</span></span>

<span data-ttu-id="d2dde-393">Versión 2.0.41</span><span class="sxs-lookup"><span data-stu-id="d2dde-393">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="d2dde-394">AKS</span><span class="sxs-lookup"><span data-stu-id="d2dde-394">AKS</span></span>

* <span data-ttu-id="d2dde-395">Se ha cambiado la supervisión para utilizar el identificador de suscripción</span><span class="sxs-lookup"><span data-stu-id="d2dde-395">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="d2dde-396">3 de julio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-396">July 3, 2018</span></span>

<span data-ttu-id="d2dde-397">Versión 2.0.40</span><span class="sxs-lookup"><span data-stu-id="d2dde-397">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-398">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-398">Core</span></span>

* <span data-ttu-id="d2dde-399">Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="d2dde-399">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-400">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-400">ACR</span></span>

* <span data-ttu-id="d2dde-401">Se ha agregado el estado de compilación de sondeo</span><span class="sxs-lookup"><span data-stu-id="d2dde-401">Added polling build status</span></span>
* <span data-ttu-id="d2dde-402">Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="d2dde-402">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="d2dde-403">Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`</span><span class="sxs-lookup"><span data-stu-id="d2dde-403">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-404">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-404">ACS</span></span>

* <span data-ttu-id="d2dde-405">[CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="d2dde-405">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="d2dde-406">Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="d2dde-406">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="d2dde-407">Se han actualizado las opciones del comando `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-407">Updated options for `aks browse` command.</span></span> <span data-ttu-id="d2dde-408">Se ha agregado compatibilidad con `--listen-port`</span><span class="sxs-lookup"><span data-stu-id="d2dde-408">Added `--listen-port` support</span></span>
* <span data-ttu-id="d2dde-409">Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-409">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="d2dde-410">Use virtual-kubelet-for-aks-latest.tgz</span><span class="sxs-lookup"><span data-stu-id="d2dde-410">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="d2dde-411">Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente</span><span class="sxs-lookup"><span data-stu-id="d2dde-411">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-412">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-412">AppService</span></span>

* <span data-ttu-id="d2dde-413">Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`</span><span class="sxs-lookup"><span data-stu-id="d2dde-413">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="d2dde-414">Se ha quitado la etiqueta `preview` para la característica de identidad</span><span class="sxs-lookup"><span data-stu-id="d2dde-414">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="d2dde-415">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="d2dde-415">Backup</span></span>

* <span data-ttu-id="d2dde-416">Se ha actualizado la definición del módulo</span><span class="sxs-lookup"><span data-stu-id="d2dde-416">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="d2dde-417">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d2dde-417">BatchAI</span></span>

* <span data-ttu-id="d2dde-418">Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-418">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="d2dde-419">Nube</span><span class="sxs-lookup"><span data-stu-id="d2dde-419">Cloud</span></span>

* <span data-ttu-id="d2dde-420">Se ha agregado el sufijo de servidor `acr login` a la configuración de nube</span><span class="sxs-lookup"><span data-stu-id="d2dde-420">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-421">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-421">Container</span></span>

* <span data-ttu-id="d2dde-422">Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución</span><span class="sxs-lookup"><span data-stu-id="d2dde-422">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="d2dde-423">Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`</span><span class="sxs-lookup"><span data-stu-id="d2dde-423">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="d2dde-424">Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar</span><span class="sxs-lookup"><span data-stu-id="d2dde-424">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-425">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-425">Extension</span></span>

* <span data-ttu-id="d2dde-426">Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI</span><span class="sxs-lookup"><span data-stu-id="d2dde-426">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-427">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-427">Network</span></span>

* <span data-ttu-id="d2dde-428">Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))</span><span class="sxs-lookup"><span data-stu-id="d2dde-428">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="d2dde-429">Rdbms</span><span class="sxs-lookup"><span data-stu-id="d2dde-429">Rdbms</span></span>

* <span data-ttu-id="d2dde-430">Se agregaron los comandos `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-430">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-431">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-431">Resource</span></span>

* <span data-ttu-id="d2dde-432">Se ha agregado un nuevo grupo de operaciones `deployment`</span><span class="sxs-lookup"><span data-stu-id="d2dde-432">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-433">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-433">VM</span></span>

* <span data-ttu-id="d2dde-434">Se ha agregado compatibilidad para quitar la identidad asignada por el sistema</span><span class="sxs-lookup"><span data-stu-id="d2dde-434">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="d2dde-435">25 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-435">June 25, 2018</span></span>

<span data-ttu-id="d2dde-436">Versión 2.0.39</span><span class="sxs-lookup"><span data-stu-id="d2dde-436">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="d2dde-437">CLI</span><span class="sxs-lookup"><span data-stu-id="d2dde-437">CLI</span></span>

* <span data-ttu-id="d2dde-438">Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-438">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="d2dde-439">19 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-439">June 19, 2018</span></span>

<span data-ttu-id="d2dde-440">Versión 2.0.38</span><span class="sxs-lookup"><span data-stu-id="d2dde-440">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-441">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-441">Core</span></span>

* <span data-ttu-id="d2dde-442">Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-442">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-443">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-443">ACR</span></span>

* <span data-ttu-id="d2dde-444">Se ha agregado `azure-storage-blob` como dependencia</span><span class="sxs-lookup"><span data-stu-id="d2dde-444">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="d2dde-445">Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos</span><span class="sxs-lookup"><span data-stu-id="d2dde-445">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-446">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-446">ACS</span></span>

* <span data-ttu-id="d2dde-447">Se actualizaron las opciones del comando `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-447">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="d2dde-448">Se ha agregado compatibilidad con `--update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-448">Added `--update` support</span></span>
* <span data-ttu-id="d2dde-449">Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`</span><span class="sxs-lookup"><span data-stu-id="d2dde-449">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="d2dde-450">Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados</span><span class="sxs-lookup"><span data-stu-id="d2dde-450">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="d2dde-451">Se ha corregido el error del comando `acs browse`</span><span class="sxs-lookup"><span data-stu-id="d2dde-451">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="d2dde-452">Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="d2dde-452">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="d2dde-453">Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d2dde-453">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="d2dde-454">Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d2dde-454">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-455">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-455">AppService</span></span>

* <span data-ttu-id="d2dde-456">Se ha agregado compatibilidad con las versiones más recientes de urllib</span><span class="sxs-lookup"><span data-stu-id="d2dde-456">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="d2dde-457">Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos</span><span class="sxs-lookup"><span data-stu-id="d2dde-457">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-458">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-458">Batch</span></span>

* <span data-ttu-id="d2dde-459">Se ha eliminado la dependencia de `azure-batch-extensions`</span><span class="sxs-lookup"><span data-stu-id="d2dde-459">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d2dde-460">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d2dde-460">Batch AI</span></span>

* <span data-ttu-id="d2dde-461">Se ha agregado compatibilidad para áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="d2dde-461">Added support for workspaces.</span></span> <span data-ttu-id="d2dde-462">Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.</span><span class="sxs-lookup"><span data-stu-id="d2dde-462">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="d2dde-463">Se ha agregado compatibilidad para experimentos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-463">Added support for experiments.</span></span> <span data-ttu-id="d2dde-464">Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados</span><span class="sxs-lookup"><span data-stu-id="d2dde-464">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="d2dde-465">Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker</span><span class="sxs-lookup"><span data-stu-id="d2dde-465">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="d2dde-466">Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-466">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="d2dde-467">Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-467">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="d2dde-468">Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-468">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="d2dde-469">[CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.</span><span class="sxs-lookup"><span data-stu-id="d2dde-469">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="d2dde-470">[CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-470">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="d2dde-471">[CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-471">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="d2dde-472">Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-472">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="d2dde-473">[CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-473">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="d2dde-474">Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-474">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="d2dde-475">[CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-475">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="d2dde-476">Ahora, la ubicación ahora es un atributo de un área de trabajo.</span><span class="sxs-lookup"><span data-stu-id="d2dde-476">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="d2dde-477">[CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-477">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="d2dde-478">[CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:</span><span class="sxs-lookup"><span data-stu-id="d2dde-478">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="d2dde-479">Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]</span><span class="sxs-lookup"><span data-stu-id="d2dde-479">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="d2dde-480">Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d2dde-480">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="d2dde-481">Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]</span><span class="sxs-lookup"><span data-stu-id="d2dde-481">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="d2dde-482">Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]</span><span class="sxs-lookup"><span data-stu-id="d2dde-482">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="d2dde-483">Mapas</span><span class="sxs-lookup"><span data-stu-id="d2dde-483">Maps</span></span>

* <span data-ttu-id="d2dde-484">[CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-484">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-485">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-485">Network</span></span>

* <span data-ttu-id="d2dde-486">Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)</span><span class="sxs-lookup"><span data-stu-id="d2dde-486">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="d2dde-487">Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-487">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="d2dde-488">n.º 6502</span><span class="sxs-lookup"><span data-stu-id="d2dde-488">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="d2dde-489">Reservations</span><span class="sxs-lookup"><span data-stu-id="d2dde-489">Reservations</span></span>

* <span data-ttu-id="d2dde-490">[CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-490">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="d2dde-491">Se ha agregado el parámetro `Location` a `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-491">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="d2dde-492">[CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-492">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="d2dde-493">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-493">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="d2dde-494">[CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-494">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="d2dde-495">Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-495">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-496">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-496">Role</span></span>

* <span data-ttu-id="d2dde-497">Se ha mejorado el control de errores</span><span class="sxs-lookup"><span data-stu-id="d2dde-497">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-498">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-498">SQL</span></span>

* <span data-ttu-id="d2dde-499">Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción</span><span class="sxs-lookup"><span data-stu-id="d2dde-499">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-500">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-500">Storage</span></span>

* <span data-ttu-id="d2dde-501">Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible</span><span class="sxs-lookup"><span data-stu-id="d2dde-501">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-502">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-502">VM</span></span>

* <span data-ttu-id="d2dde-503">Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-503">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="d2dde-504">Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`</span><span class="sxs-lookup"><span data-stu-id="d2dde-504">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="d2dde-505">Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado</span><span class="sxs-lookup"><span data-stu-id="d2dde-505">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d2dde-506">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-506">June 13, 2018</span></span>

<span data-ttu-id="d2dde-507">Versión 2.0.37</span><span class="sxs-lookup"><span data-stu-id="d2dde-507">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-508">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-508">Core</span></span>

* <span data-ttu-id="d2dde-509">Se ha mejorado la telemetría interactiva</span><span class="sxs-lookup"><span data-stu-id="d2dde-509">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="d2dde-510">13 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-510">June 13, 2018</span></span>

<span data-ttu-id="d2dde-511">Versión 2.0.36</span><span class="sxs-lookup"><span data-stu-id="d2dde-511">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="d2dde-512">AKS</span><span class="sxs-lookup"><span data-stu-id="d2dde-512">AKS</span></span>

* <span data-ttu-id="d2dde-513">Se han agregado opciones de red avanzadas a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-513">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="d2dde-514">Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP</span><span class="sxs-lookup"><span data-stu-id="d2dde-514">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="d2dde-515">Se agregó el argumento `--no-ssh-key` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-515">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="d2dde-516">Se agregó el argumento `--enable-rbac` a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-516">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="d2dde-517">[VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-517">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-518">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-518">AppService</span></span>

* <span data-ttu-id="d2dde-519">Se corrigió un problema con las versiones de urllib incompatibles</span><span class="sxs-lookup"><span data-stu-id="d2dde-519">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d2dde-520">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-520">June 5, 2018</span></span>

<span data-ttu-id="d2dde-521">Versión 2.0.35</span><span class="sxs-lookup"><span data-stu-id="d2dde-521">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-522">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-522">Interactive</span></span>

* <span data-ttu-id="d2dde-523">Se agregaron límites a las dependencias de modo interactivo</span><span class="sxs-lookup"><span data-stu-id="d2dde-523">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="d2dde-524">5 de junio de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-524">June 5, 2018</span></span>

<span data-ttu-id="d2dde-525">Versión 2.0.34</span><span class="sxs-lookup"><span data-stu-id="d2dde-525">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-526">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-526">Core</span></span>

* <span data-ttu-id="d2dde-527">Se ha agregado compatibilidad para referencias a recursos entre inquilinos</span><span class="sxs-lookup"><span data-stu-id="d2dde-527">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="d2dde-528">Se ha mejorado la confiabilidad de la carga de datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="d2dde-528">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-529">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-529">ACR</span></span>

* <span data-ttu-id="d2dde-530">Se ha agregado compatibilidad para VSTS como ubicación de origen remoto</span><span class="sxs-lookup"><span data-stu-id="d2dde-530">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="d2dde-531">Se agregó el comando `acr import`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-531">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="d2dde-532">AKS</span><span class="sxs-lookup"><span data-stu-id="d2dde-532">AKS</span></span>

* <span data-ttu-id="d2dde-533">Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos</span><span class="sxs-lookup"><span data-stu-id="d2dde-533">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-534">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-534">Batch</span></span>

* <span data-ttu-id="d2dde-535">Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="d2dde-535">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-536">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-536">IOT</span></span>

* <span data-ttu-id="d2dde-537">Se ha agregado compatibilidad para crear centros de IoT de nivel básico</span><span class="sxs-lookup"><span data-stu-id="d2dde-537">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-538">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-538">Network</span></span>

* <span data-ttu-id="d2dde-539">Se ha mejorado `network vnet peering`</span><span class="sxs-lookup"><span data-stu-id="d2dde-539">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="d2dde-540">Información de directiva</span><span class="sxs-lookup"><span data-stu-id="d2dde-540">Policy Insights</span></span>

* <span data-ttu-id="d2dde-541">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="d2dde-541">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="d2dde-542">ARM</span><span class="sxs-lookup"><span data-stu-id="d2dde-542">ARM</span></span>

* <span data-ttu-id="d2dde-543">Se han agregado comandos `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-543">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-544">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-544">SQL</span></span>

* <span data-ttu-id="d2dde-545">Se han agregado nuevos comandos de instancia administrada:</span><span class="sxs-lookup"><span data-stu-id="d2dde-545">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="d2dde-546">Se han agregado nuevos comandos de base de datos administrada:</span><span class="sxs-lookup"><span data-stu-id="d2dde-546">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="d2dde-547">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-547">Storage</span></span>

* <span data-ttu-id="d2dde-548">Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo</span><span class="sxs-lookup"><span data-stu-id="d2dde-548">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-549">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-549">VM</span></span>

* <span data-ttu-id="d2dde-550">Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar</span><span class="sxs-lookup"><span data-stu-id="d2dde-550">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="d2dde-551">Se agregó la opción `--accelerated-networking` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-551">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="d2dde-552">Se ha agregado `--tags` a `identity create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-552">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="d2dde-553">22 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-553">May 22, 2018</span></span>

<span data-ttu-id="d2dde-554">Versión 2.0.33</span><span class="sxs-lookup"><span data-stu-id="d2dde-554">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-555">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-555">Core</span></span>

* <span data-ttu-id="d2dde-556">Se ha agregado compatibilidad para expandir `@` en nombres de archivo</span><span class="sxs-lookup"><span data-stu-id="d2dde-556">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-557">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-557">ACS</span></span>

* <span data-ttu-id="d2dde-558">Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`</span><span class="sxs-lookup"><span data-stu-id="d2dde-558">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="d2dde-559">Se ha corregido el error tipográfico en el mensaje de ayuda</span><span class="sxs-lookup"><span data-stu-id="d2dde-559">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-560">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-560">AppService</span></span>

* <span data-ttu-id="d2dde-561">Se han mejorado los comandos de actualización genéricos</span><span class="sxs-lookup"><span data-stu-id="d2dde-561">Improved generic update commands</span></span>
* <span data-ttu-id="d2dde-562">Se ha añadido compatibilidad con async para `webapp deployment source config-zip`</span><span class="sxs-lookup"><span data-stu-id="d2dde-562">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-563">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-563">Container</span></span>

* <span data-ttu-id="d2dde-564">Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml</span><span class="sxs-lookup"><span data-stu-id="d2dde-564">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="d2dde-565">Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d2dde-565">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-566">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-566">Extension</span></span>

* <span data-ttu-id="d2dde-567">Se ha mejorado la eliminación de extensiones</span><span class="sxs-lookup"><span data-stu-id="d2dde-567">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-568">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-568">Interactive</span></span>

* <span data-ttu-id="d2dde-569">Se ha cambiado el registro para silenciar el analizador en las finalizaciones</span><span class="sxs-lookup"><span data-stu-id="d2dde-569">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="d2dde-570">Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda</span><span class="sxs-lookup"><span data-stu-id="d2dde-570">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-571">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d2dde-571">KeyVault</span></span>

* <span data-ttu-id="d2dde-572">Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad</span><span class="sxs-lookup"><span data-stu-id="d2dde-572">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-573">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-573">Network</span></span>

* <span data-ttu-id="d2dde-574">Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="d2dde-574">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="d2dde-575">Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="d2dde-575">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-576">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-576">SQL</span></span>

* <span data-ttu-id="d2dde-577">[CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:</span><span class="sxs-lookup"><span data-stu-id="d2dde-577">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="d2dde-578">Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`</span><span class="sxs-lookup"><span data-stu-id="d2dde-578">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="d2dde-579">Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`</span><span class="sxs-lookup"><span data-stu-id="d2dde-579">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="d2dde-580">Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="d2dde-580">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="d2dde-581">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="d2dde-581">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="d2dde-582">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-582">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="d2dde-583">Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`</span><span class="sxs-lookup"><span data-stu-id="d2dde-583">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="d2dde-584">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-584">`edition`.</span></span> <span data-ttu-id="d2dde-585">Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`</span><span class="sxs-lookup"><span data-stu-id="d2dde-585">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="d2dde-586">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-586">`elasticPoolName`.</span></span> <span data-ttu-id="d2dde-587">Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`</span><span class="sxs-lookup"><span data-stu-id="d2dde-587">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="d2dde-588">[CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:</span><span class="sxs-lookup"><span data-stu-id="d2dde-588">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="d2dde-589">`edition`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-589">`edition`.</span></span> <span data-ttu-id="d2dde-590">Para actualizar, use el parámetro `--edition`</span><span class="sxs-lookup"><span data-stu-id="d2dde-590">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="d2dde-591">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-591">`dtu`.</span></span> <span data-ttu-id="d2dde-592">Para actualizar, use el parámetro `--capacity`</span><span class="sxs-lookup"><span data-stu-id="d2dde-592">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="d2dde-593">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-593">`databaseDtuMin`.</span></span> <span data-ttu-id="d2dde-594">Para actualizar, use el parámetro `--db-min-capacity`</span><span class="sxs-lookup"><span data-stu-id="d2dde-594">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="d2dde-595">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-595">`databaseDtuMax`.</span></span> <span data-ttu-id="d2dde-596">Para actualizar, use el parámetro `--db-max-capacity`</span><span class="sxs-lookup"><span data-stu-id="d2dde-596">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="d2dde-597">Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-597">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="d2dde-598">Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-598">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-599">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-599">Storage</span></span>

* <span data-ttu-id="d2dde-600">Se ha agregado la función de autocompletar al argumento `--account-name`</span><span class="sxs-lookup"><span data-stu-id="d2dde-600">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="d2dde-601">Se ha corregido un problema con `storage entity query`</span><span class="sxs-lookup"><span data-stu-id="d2dde-601">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-602">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-602">VM</span></span>

* <span data-ttu-id="d2dde-603">[CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-603">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="d2dde-604">Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`</span><span class="sxs-lookup"><span data-stu-id="d2dde-604">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="d2dde-605">Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`</span><span class="sxs-lookup"><span data-stu-id="d2dde-605">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="d2dde-606">Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque</span><span class="sxs-lookup"><span data-stu-id="d2dde-606">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="d2dde-607">Se ha agregado `--license-type` a `[vm|vmss] update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-607">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="d2dde-608">7 de mayo de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-608">May 7, 2018</span></span>

<span data-ttu-id="d2dde-609">Versión 2.0.32</span><span class="sxs-lookup"><span data-stu-id="d2dde-609">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-610">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-610">Core</span></span>

* <span data-ttu-id="d2dde-611">Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado</span><span class="sxs-lookup"><span data-stu-id="d2dde-611">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="d2dde-612">Se ha agregado compatibilidad limitada con argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="d2dde-612">Added limited support for positional arguments</span></span>
* <span data-ttu-id="d2dde-613">Se ha corregido el problema en el que `--query` no se podía usar con `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-613">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="d2dde-614">N.º 5591</span><span class="sxs-lookup"><span data-stu-id="d2dde-614">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="d2dde-615">Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-615">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="d2dde-616">Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta</span><span class="sxs-lookup"><span data-stu-id="d2dde-616">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="d2dde-617">Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-617">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="d2dde-618">Se han mejorado los errores cuando los usuarios escriben `az ''`</span><span class="sxs-lookup"><span data-stu-id="d2dde-618">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="d2dde-619">Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-619">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-620">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-620">ACR</span></span>

* <span data-ttu-id="d2dde-621">Se han agregado comandos ACR Build</span><span class="sxs-lookup"><span data-stu-id="d2dde-621">Added ACR Build commands</span></span>
* <span data-ttu-id="d2dde-622">Se han mejorado los mensajes de error para un recurso no encontrado</span><span class="sxs-lookup"><span data-stu-id="d2dde-622">Improved resource not found error messages</span></span>
* <span data-ttu-id="d2dde-623">Se ha mejorado el rendimiento en la creación de recursos y el control de errores</span><span class="sxs-lookup"><span data-stu-id="d2dde-623">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="d2dde-624">Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL</span><span class="sxs-lookup"><span data-stu-id="d2dde-624">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="d2dde-625">Se han mejorado los mensajes de error de los comandos del repositorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-625">Improved repository commands error messages</span></span>
* <span data-ttu-id="d2dde-626">Se han actualizado las columnas de tabla y la ordenación</span><span class="sxs-lookup"><span data-stu-id="d2dde-626">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-627">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-627">ACS</span></span>

* <span data-ttu-id="d2dde-628">Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d2dde-628">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="d2dde-629">Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`</span><span class="sxs-lookup"><span data-stu-id="d2dde-629">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="d2dde-630">AMS</span><span class="sxs-lookup"><span data-stu-id="d2dde-630">AMS</span></span>

* <span data-ttu-id="d2dde-631">Versión inicial: administración de recursos de Azure Media Services</span><span class="sxs-lookup"><span data-stu-id="d2dde-631">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-632">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-632">Appservice</span></span>

* <span data-ttu-id="d2dde-633">Se ha corregido un error en `webapp delete` cuando se indica `--slot`</span><span class="sxs-lookup"><span data-stu-id="d2dde-633">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="d2dde-634">Se ha eliminado `--runtime-version` en `webapp auth update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-634">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="d2dde-635">Se ha agregado compatibilidad con min\_tls\_version y https2.0</span><span class="sxs-lookup"><span data-stu-id="d2dde-635">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="d2dde-636">Se ha agregado compatibilidad con multicontenedores</span><span class="sxs-lookup"><span data-stu-id="d2dde-636">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="d2dde-637">Batch AI</span><span class="sxs-lookup"><span data-stu-id="d2dde-637">Batch AI</span></span>

* <span data-ttu-id="d2dde-638">Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster</span><span class="sxs-lookup"><span data-stu-id="d2dde-638">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d2dde-639">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d2dde-639">Cognitive Services</span></span>

* <span data-ttu-id="d2dde-640">Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)</span><span class="sxs-lookup"><span data-stu-id="d2dde-640">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="d2dde-641">Consumo</span><span class="sxs-lookup"><span data-stu-id="d2dde-641">Consumption</span></span>

* <span data-ttu-id="d2dde-642">Se han agregado nuevos comandos a la API de presupuestos</span><span class="sxs-lookup"><span data-stu-id="d2dde-642">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-643">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-643">Container</span></span>

* <span data-ttu-id="d2dde-644">Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen</span><span class="sxs-lookup"><span data-stu-id="d2dde-644">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="d2dde-645">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d2dde-645">Cosmos DB</span></span>

* <span data-ttu-id="d2dde-646">Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="d2dde-646">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="d2dde-647">DMS</span><span class="sxs-lookup"><span data-stu-id="d2dde-647">DMS</span></span>

* <span data-ttu-id="d2dde-648">Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-648">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-649">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-649">Extension</span></span>

* <span data-ttu-id="d2dde-650">Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse</span><span class="sxs-lookup"><span data-stu-id="d2dde-650">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-651">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-651">Interactive</span></span>

* <span data-ttu-id="d2dde-652">Se permiten autocompletadores interactivos para los argumentos posicionales</span><span class="sxs-lookup"><span data-stu-id="d2dde-652">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="d2dde-653">Se presenta una salida de uso sencillo cuando los usuarios escriben '\'</span><span class="sxs-lookup"><span data-stu-id="d2dde-653">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="d2dde-654">Se ha corregido la finalización de parámetros sin ayuda</span><span class="sxs-lookup"><span data-stu-id="d2dde-654">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="d2dde-655">Se han corregido las descripciones de los grupos de comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-655">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="d2dde-656">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-656">Lab</span></span>

* <span data-ttu-id="d2dde-657">Se han corregido las regresiones en la conversión de Knack</span><span class="sxs-lookup"><span data-stu-id="d2dde-657">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-658">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-658">Network</span></span>

* <span data-ttu-id="d2dde-659">[CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="d2dde-659">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="d2dde-660">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-660">Profile</span></span>

* <span data-ttu-id="d2dde-661">Se ha corregido la detección de origen en `disk create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-661">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="d2dde-662">[CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse</span><span class="sxs-lookup"><span data-stu-id="d2dde-662">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="d2dde-663">Se ha corregido el error de escritura en el resumen breve de `account get-access-token`</span><span class="sxs-lookup"><span data-stu-id="d2dde-663">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="d2dde-664">Redis</span><span class="sxs-lookup"><span data-stu-id="d2dde-664">Redis</span></span>

* <span data-ttu-id="d2dde-665">Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`</span><span class="sxs-lookup"><span data-stu-id="d2dde-665">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="d2dde-666">Entra en desuso `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-666">Deprecated `redis list-all`.</span></span> <span data-ttu-id="d2dde-667">Esta funcionalidad se ha situado en `redis list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-667">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="d2dde-668">Entra en desuso `redis import-method` en favor de `redis import`</span><span class="sxs-lookup"><span data-stu-id="d2dde-668">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="d2dde-669">Se ha agregado compatibilidad con `--ids` en varios comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-669">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-670">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-670">Role</span></span>

* <span data-ttu-id="d2dde-671">[CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso</span><span class="sxs-lookup"><span data-stu-id="d2dde-671">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-672">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-672">Storage</span></span>

* <span data-ttu-id="d2dde-673">Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta</span><span class="sxs-lookup"><span data-stu-id="d2dde-673">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="d2dde-674">Se expone --socket-timeout en la carga y descarga de blobs</span><span class="sxs-lookup"><span data-stu-id="d2dde-674">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="d2dde-675">Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas</span><span class="sxs-lookup"><span data-stu-id="d2dde-675">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="d2dde-676">Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"</span><span class="sxs-lookup"><span data-stu-id="d2dde-676">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="d2dde-677">Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores</span><span class="sxs-lookup"><span data-stu-id="d2dde-677">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-678">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-678">VM</span></span>

* <span data-ttu-id="d2dde-679">Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados</span><span class="sxs-lookup"><span data-stu-id="d2dde-679">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="d2dde-680">Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="d2dde-680">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="d2dde-681">[CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI</span><span class="sxs-lookup"><span data-stu-id="d2dde-681">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="d2dde-682">Se ha agregado compatibilidad con la directiva de expulsión para `vmss`</span><span class="sxs-lookup"><span data-stu-id="d2dde-682">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="d2dde-683">[CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:</span><span class="sxs-lookup"><span data-stu-id="d2dde-683">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="d2dde-684">Se ha agregado compatibilidad con el acelerador de escritura</span><span class="sxs-lookup"><span data-stu-id="d2dde-684">Added write accelerator support</span></span>
* <span data-ttu-id="d2dde-685">Se agregó `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-685">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="d2dde-686">Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable</span><span class="sxs-lookup"><span data-stu-id="d2dde-686">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="d2dde-687">Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio</span><span class="sxs-lookup"><span data-stu-id="d2dde-687">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="d2dde-688">10 de abril de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-688">April 10, 2018</span></span>

<span data-ttu-id="d2dde-689">Versión 2.0.31</span><span class="sxs-lookup"><span data-stu-id="d2dde-689">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-690">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-690">ACR</span></span>

* <span data-ttu-id="d2dde-691">Control de errores mejorado de la conmutación por recuperación con wincred</span><span class="sxs-lookup"><span data-stu-id="d2dde-691">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-692">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-692">ACS</span></span>

* <span data-ttu-id="d2dde-693">Se cambió AKS, se crearon SPN para que sean válidas durante 5 años</span><span class="sxs-lookup"><span data-stu-id="d2dde-693">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-694">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-694">Appservice</span></span>

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="d2dde-696">Se ha corregido la excepción no detectada de planes de webapp no existentes</span><span class="sxs-lookup"><span data-stu-id="d2dde-696">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="d2dde-697">BatchAI</span><span class="sxs-lookup"><span data-stu-id="d2dde-697">BatchAI</span></span>

* <span data-ttu-id="d2dde-698">Se ha agregado compatibilidad con la API 2018-03-01</span><span class="sxs-lookup"><span data-stu-id="d2dde-698">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="d2dde-699">Montaje en el nivel de trabajo</span><span class="sxs-lookup"><span data-stu-id="d2dde-699">Job level mounting</span></span>
 - <span data-ttu-id="d2dde-700">Variables de entorno con valores de secreto</span><span class="sxs-lookup"><span data-stu-id="d2dde-700">Environment variables with secret values</span></span>
 - <span data-ttu-id="d2dde-701">Configuración de contadores de rendimiento</span><span class="sxs-lookup"><span data-stu-id="d2dde-701">Performance counters settings</span></span>
 - <span data-ttu-id="d2dde-702">Creación de informes de segmentos de ruta de acceso específicas del trabajo</span><span class="sxs-lookup"><span data-stu-id="d2dde-702">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="d2dde-703">Compatibilidad con subcarpetas en API de lista de archivos</span><span class="sxs-lookup"><span data-stu-id="d2dde-703">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="d2dde-704">Uso y los límites de informes</span><span class="sxs-lookup"><span data-stu-id="d2dde-704">Usage and limits reporting</span></span>
 - <span data-ttu-id="d2dde-705">Permitir especificar el tipo de almacenamiento en caché de los servidores NFS</span><span class="sxs-lookup"><span data-stu-id="d2dde-705">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="d2dde-706">Compatibilidad con imágenes personalizadas</span><span class="sxs-lookup"><span data-stu-id="d2dde-706">Support for custom images</span></span>
 - <span data-ttu-id="d2dde-707">Se ha agregado compatibilidad con el kit de herramientas de pyTorch</span><span class="sxs-lookup"><span data-stu-id="d2dde-707">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="d2dde-708">Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo</span><span class="sxs-lookup"><span data-stu-id="d2dde-708">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="d2dde-709">Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones</span><span class="sxs-lookup"><span data-stu-id="d2dde-709">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="d2dde-710">Se admiten las nubes nacionales</span><span class="sxs-lookup"><span data-stu-id="d2dde-710">National clouds are supported</span></span>
* <span data-ttu-id="d2dde-711">Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración</span><span class="sxs-lookup"><span data-stu-id="d2dde-711">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="d2dde-712">Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada</span><span class="sxs-lookup"><span data-stu-id="d2dde-712">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="d2dde-713">Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI</span><span class="sxs-lookup"><span data-stu-id="d2dde-713">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="d2dde-714">Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración.</span><span class="sxs-lookup"><span data-stu-id="d2dde-714">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="d2dde-715">Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)</span><span class="sxs-lookup"><span data-stu-id="d2dde-715">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="d2dde-716">Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)</span><span class="sxs-lookup"><span data-stu-id="d2dde-716">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="d2dde-717">Se mejoró la salida `table` de las operaciones `show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-717">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="d2dde-718">Se agregó la opción `--use-auto-storage` para la creación de clústeres.</span><span class="sxs-lookup"><span data-stu-id="d2dde-718">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="d2dde-719">Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres</span><span class="sxs-lookup"><span data-stu-id="d2dde-719">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="d2dde-720">Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-720">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="d2dde-721">Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-721">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="d2dde-722">[CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`</span><span class="sxs-lookup"><span data-stu-id="d2dde-722">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="d2dde-723">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-723">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="d2dde-724">Facturación</span><span class="sxs-lookup"><span data-stu-id="d2dde-724">Billing</span></span>

* <span data-ttu-id="d2dde-725">Se han agregado comandos de inscripción de cuenta</span><span class="sxs-lookup"><span data-stu-id="d2dde-725">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="d2dde-726">Consumo</span><span class="sxs-lookup"><span data-stu-id="d2dde-726">Consumption</span></span>

* <span data-ttu-id="d2dde-727">Se agregaron los comandos `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-727">Added `marketplace` commands</span></span>
* <span data-ttu-id="d2dde-728">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d2dde-728">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="d2dde-729">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`</span><span class="sxs-lookup"><span data-stu-id="d2dde-729">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="d2dde-730">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`</span><span class="sxs-lookup"><span data-stu-id="d2dde-730">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="d2dde-731">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`</span><span class="sxs-lookup"><span data-stu-id="d2dde-731">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="d2dde-732">[CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`</span><span class="sxs-lookup"><span data-stu-id="d2dde-732">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-733">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-733">Container</span></span>

* <span data-ttu-id="d2dde-734">Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`</span><span class="sxs-lookup"><span data-stu-id="d2dde-734">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="d2dde-735">Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name</span><span class="sxs-lookup"><span data-stu-id="d2dde-735">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-736">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-736">Extension</span></span>

* <span data-ttu-id="d2dde-737">Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración</span><span class="sxs-lookup"><span data-stu-id="d2dde-737">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-738">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-738">Interactive</span></span>

* <span data-ttu-id="d2dde-739">Se ha cambiado para detener la finalización de los comandos no reconocidos</span><span class="sxs-lookup"><span data-stu-id="d2dde-739">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="d2dde-740">Se han agregado enlaces de evento antes y después de crear el subárbol de comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-740">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="d2dde-741">Se ha agregado finalización para los parámetros `--ids`</span><span class="sxs-lookup"><span data-stu-id="d2dde-741">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-742">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-742">Network</span></span>

* <span data-ttu-id="d2dde-743">Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-743">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="d2dde-744">Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-744">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="d2dde-745">4910</span><span class="sxs-lookup"><span data-stu-id="d2dde-745">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="d2dde-746">Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="d2dde-746">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="d2dde-747">Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection</span><span class="sxs-lookup"><span data-stu-id="d2dde-747">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="d2dde-748">Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-748">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="d2dde-749">Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-749">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="d2dde-750">Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`</span><span class="sxs-lookup"><span data-stu-id="d2dde-750">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-751">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-751">Profile</span></span>

* <span data-ttu-id="d2dde-752">Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-752">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="d2dde-753">[CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`</span><span class="sxs-lookup"><span data-stu-id="d2dde-753">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="d2dde-754">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d2dde-754">RDBMS</span></span>

* <span data-ttu-id="d2dde-755">Se agregó el comando `georestore`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-755">Added `georestore` command</span></span>
* <span data-ttu-id="d2dde-756">Se ha elimina la restricción de tamaño de almacenamiento del comando `create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-756">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-757">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-757">Resource</span></span>

* <span data-ttu-id="d2dde-758">Se agregó compatibilidad para `--metadata` a `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-758">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="d2dde-759">Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-759">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-760">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-760">SQL</span></span>

* <span data-ttu-id="d2dde-761">Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`</span><span class="sxs-lookup"><span data-stu-id="d2dde-761">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-762">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-762">Storage</span></span>

* <span data-ttu-id="d2dde-763">Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto</span><span class="sxs-lookup"><span data-stu-id="d2dde-763">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-764">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-764">VM</span></span>

* <span data-ttu-id="d2dde-765">Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-765">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="d2dde-766">Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados</span><span class="sxs-lookup"><span data-stu-id="d2dde-766">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="d2dde-768">Se ha agregado compatibilidad para la SKU de IP pública a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-768">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="d2dde-769">Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén.</span><span class="sxs-lookup"><span data-stu-id="d2dde-769">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="d2dde-770">5718</span><span class="sxs-lookup"><span data-stu-id="d2dde-770">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="d2dde-771">Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas</span><span class="sxs-lookup"><span data-stu-id="d2dde-771">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="d2dde-772">27 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-772">March 27, 2018</span></span>

<span data-ttu-id="d2dde-773">Versión 2.0.30</span><span class="sxs-lookup"><span data-stu-id="d2dde-773">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-774">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-774">Core</span></span>

* <span data-ttu-id="d2dde-775">Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda</span><span class="sxs-lookup"><span data-stu-id="d2dde-775">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-776">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-776">ACS</span></span>

* <span data-ttu-id="d2dde-777">Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d2dde-777">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-778">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-778">Appservice</span></span>

* <span data-ttu-id="d2dde-779">Se ha agregado compatibilidad solo para HTTPS a `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-779">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="d2dde-780">Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-780">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d2dde-781">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="d2dde-781">Backup</span></span>

* <span data-ttu-id="d2dde-782">Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-782">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="d2dde-783">Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-783">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="d2dde-784">Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="d2dde-784">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="d2dde-785">Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`</span><span class="sxs-lookup"><span data-stu-id="d2dde-785">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-786">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-786">Container</span></span>

* <span data-ttu-id="d2dde-787">Se ha agregado el comando `container exec`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-787">Added `container exec` command.</span></span> <span data-ttu-id="d2dde-788">Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución</span><span class="sxs-lookup"><span data-stu-id="d2dde-788">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="d2dde-789">Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d2dde-789">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-790">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-790">Extension</span></span>

* <span data-ttu-id="d2dde-791">Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d2dde-791">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="d2dde-792">Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`</span><span class="sxs-lookup"><span data-stu-id="d2dde-792">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="d2dde-793">[CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="d2dde-793">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-794">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-794">Interactive</span></span>

* <span data-ttu-id="d2dde-795">Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-795">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="d2dde-796">Se ha corregido el error al usar el parámetro `--style`</span><span class="sxs-lookup"><span data-stu-id="d2dde-796">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="d2dde-797">Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-797">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="d2dde-798">Compatibilidad mejorada para completer</span><span class="sxs-lookup"><span data-stu-id="d2dde-798">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="d2dde-799">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-799">Lab</span></span>

* <span data-ttu-id="d2dde-800">Se han corregido los errores del comando `create environment`</span><span class="sxs-lookup"><span data-stu-id="d2dde-800">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-801">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-801">Monitor</span></span>

* <span data-ttu-id="d2dde-802">Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d2dde-802">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="d2dde-803">Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar</span><span class="sxs-lookup"><span data-stu-id="d2dde-803">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="d2dde-804">Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)</span><span class="sxs-lookup"><span data-stu-id="d2dde-804">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-805">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-805">Network</span></span>

* <span data-ttu-id="d2dde-806">Se ha agregado compatibilidad para zonas DNS privadas</span><span class="sxs-lookup"><span data-stu-id="d2dde-806">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-807">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-807">Profile</span></span>

* <span data-ttu-id="d2dde-808">Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`</span><span class="sxs-lookup"><span data-stu-id="d2dde-808">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d2dde-809">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d2dde-809">RDBMS</span></span>

* <span data-ttu-id="d2dde-810">Se ha agregado el modelo de negocio GA API versión 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="d2dde-810">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-811">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-811">Resource</span></span>

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="d2dde-813">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-813">Role</span></span>

* <span data-ttu-id="d2dde-814">Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-814">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="d2dde-815">Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto</span><span class="sxs-lookup"><span data-stu-id="d2dde-815">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="d2dde-816">Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-816">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="d2dde-817">[CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-817">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="d2dde-818">Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`</span><span class="sxs-lookup"><span data-stu-id="d2dde-818">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-819">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-819">Storage</span></span>

* <span data-ttu-id="d2dde-820">Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB</span><span class="sxs-lookup"><span data-stu-id="d2dde-820">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="d2dde-821">Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición</span><span class="sxs-lookup"><span data-stu-id="d2dde-821">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-822">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-822">VM</span></span>

* <span data-ttu-id="d2dde-823">Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias</span><span class="sxs-lookup"><span data-stu-id="d2dde-823">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="d2dde-824">Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-824">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="d2dde-825">Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado</span><span class="sxs-lookup"><span data-stu-id="d2dde-825">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="d2dde-826">[CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida</span><span class="sxs-lookup"><span data-stu-id="d2dde-826">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="d2dde-827">13 de marzo de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-827">March 13, 2018</span></span>

<span data-ttu-id="d2dde-828">Versión 2.0.29</span><span class="sxs-lookup"><span data-stu-id="d2dde-828">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-829">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-829">ACR</span></span>

* <span data-ttu-id="d2dde-830">Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-830">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="d2dde-831">Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-831">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="d2dde-832">Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-832">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-833">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-833">ACS</span></span>

* <span data-ttu-id="d2dde-834">Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.</span><span class="sxs-lookup"><span data-stu-id="d2dde-834">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="d2dde-835">Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.</span><span class="sxs-lookup"><span data-stu-id="d2dde-835">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="d2dde-836">Advisor</span><span class="sxs-lookup"><span data-stu-id="d2dde-836">Advisor</span></span>

* <span data-ttu-id="d2dde-837">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-837">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="d2dde-838">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-838">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="d2dde-839">[CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`</span><span class="sxs-lookup"><span data-stu-id="d2dde-839">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="d2dde-840">Se ha agregado el parámetro `--refresh` a `advisor recommendation list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-840">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="d2dde-841">Se agregó el comando `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-841">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-842">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-842">Appservice</span></span>

* <span data-ttu-id="d2dde-843">`[webapp|functionapp] assign-identity` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-843">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="d2dde-844">Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-844">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="d2dde-845">Event Hubs</span><span class="sxs-lookup"><span data-stu-id="d2dde-845">Eventhubs</span></span>

* <span data-ttu-id="d2dde-846">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d2dde-846">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-847">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-847">Extension</span></span>

* <span data-ttu-id="d2dde-848">Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.</span><span class="sxs-lookup"><span data-stu-id="d2dde-848">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-849">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-849">Interactive</span></span>

* <span data-ttu-id="d2dde-850">Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.</span><span class="sxs-lookup"><span data-stu-id="d2dde-850">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="d2dde-851">Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.</span><span class="sxs-lookup"><span data-stu-id="d2dde-851">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="d2dde-852">Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.</span><span class="sxs-lookup"><span data-stu-id="d2dde-852">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="d2dde-853">Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.</span><span class="sxs-lookup"><span data-stu-id="d2dde-853">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-854">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-854">Monitor</span></span>

* <span data-ttu-id="d2dde-855">Los comandos `monitor autoscale-settings` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-855">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="d2dde-856">Se agregaron los comandos `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-856">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="d2dde-857">Se agregaron los comandos `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-857">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="d2dde-858">Se agregaron los comandos `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-858">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-859">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-859">Network</span></span>

* <span data-ttu-id="d2dde-860">[CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-860">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="d2dde-861">Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="d2dde-861">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="d2dde-862">Se han agregado comandos `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-862">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="d2dde-863">Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-863">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-864">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-864">Profile</span></span>

* <span data-ttu-id="d2dde-865">El parámetro `--msi` de `az login` está en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-865">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="d2dde-866">Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-866">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="d2dde-867">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d2dde-867">RDBMS</span></span>

* <span data-ttu-id="d2dde-868">[VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview</span><span class="sxs-lookup"><span data-stu-id="d2dde-868">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="d2dde-869">Azure Service Bus</span><span class="sxs-lookup"><span data-stu-id="d2dde-869">Service Bus</span></span>

* <span data-ttu-id="d2dde-870">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d2dde-870">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-871">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-871">Storage</span></span>

* <span data-ttu-id="d2dde-872">Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.</span><span class="sxs-lookup"><span data-stu-id="d2dde-872">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="d2dde-873">Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.</span><span class="sxs-lookup"><span data-stu-id="d2dde-873">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-874">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-874">VM</span></span>

* <span data-ttu-id="d2dde-875">Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.</span><span class="sxs-lookup"><span data-stu-id="d2dde-875">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="d2dde-876">`[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-876">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="d2dde-877">Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-877">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="d2dde-878">Se ha cambiado la prioridad predeterminada en `vmss create` a None.</span><span class="sxs-lookup"><span data-stu-id="d2dde-878">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="d2dde-879">27 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-879">February 27, 2018</span></span>

<span data-ttu-id="d2dde-880">Versión 2.0.28</span><span class="sxs-lookup"><span data-stu-id="d2dde-880">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-881">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-881">Core</span></span>

* <span data-ttu-id="d2dde-882">Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew</span><span class="sxs-lookup"><span data-stu-id="d2dde-882">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="d2dde-883">Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas</span><span class="sxs-lookup"><span data-stu-id="d2dde-883">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="d2dde-884">Se ha agregado el registro de HTTP a `--debug`</span><span class="sxs-lookup"><span data-stu-id="d2dde-884">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-885">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-885">ACS</span></span>

* <span data-ttu-id="d2dde-886">Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="d2dde-886">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="d2dde-887">Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI</span><span class="sxs-lookup"><span data-stu-id="d2dde-887">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="d2dde-888">Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`</span><span class="sxs-lookup"><span data-stu-id="d2dde-888">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="d2dde-889">Se ha eliminado el aviso de desuso de `aks get-versions`</span><span class="sxs-lookup"><span data-stu-id="d2dde-889">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-890">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-890">Appservice</span></span>

* <span data-ttu-id="d2dde-891">Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="d2dde-891">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="d2dde-892">Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida</span><span class="sxs-lookup"><span data-stu-id="d2dde-892">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="d2dde-893">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d2dde-893">Cognitive Services</span></span>

* <span data-ttu-id="d2dde-894">Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d2dde-894">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="d2dde-895">Consumo</span><span class="sxs-lookup"><span data-stu-id="d2dde-895">Consumption</span></span>

* <span data-ttu-id="d2dde-896">Se han agregado nuevos comandos a la API PriceSheet</span><span class="sxs-lookup"><span data-stu-id="d2dde-896">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="d2dde-897">Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva</span><span class="sxs-lookup"><span data-stu-id="d2dde-897">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-898">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-898">Container</span></span>

* <span data-ttu-id="d2dde-899">Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI</span><span class="sxs-lookup"><span data-stu-id="d2dde-899">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-900">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-900">Network</span></span>

* <span data-ttu-id="d2dde-901">Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`</span><span class="sxs-lookup"><span data-stu-id="d2dde-901">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-902">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-902">Resource</span></span>

* <span data-ttu-id="d2dde-903">Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error</span><span class="sxs-lookup"><span data-stu-id="d2dde-903">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-904">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-904">Role</span></span>

* <span data-ttu-id="d2dde-905">Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="d2dde-905">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-906">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-906">SQL</span></span>

* <span data-ttu-id="d2dde-907">Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización</span><span class="sxs-lookup"><span data-stu-id="d2dde-907">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-908">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-908">Storage</span></span>

* <span data-ttu-id="d2dde-909">Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-909">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-910">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-910">VM</span></span>

* <span data-ttu-id="d2dde-911">Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS</span><span class="sxs-lookup"><span data-stu-id="d2dde-911">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="d2dde-912">13 de febrero de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-912">February 13, 2018</span></span>

<span data-ttu-id="d2dde-913">Versión 2.0.27</span><span class="sxs-lookup"><span data-stu-id="d2dde-913">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-914">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-914">Core</span></span>

* <span data-ttu-id="d2dde-915">Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre</span><span class="sxs-lookup"><span data-stu-id="d2dde-915">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-916">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-916">ACS</span></span>

* <span data-ttu-id="d2dde-917">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-917">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="d2dde-918">Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-918">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="d2dde-919">Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d2dde-919">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="d2dde-920">Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS</span><span class="sxs-lookup"><span data-stu-id="d2dde-920">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="d2dde-921">Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"</span><span class="sxs-lookup"><span data-stu-id="d2dde-921">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="d2dde-922">Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`</span><span class="sxs-lookup"><span data-stu-id="d2dde-922">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="d2dde-923">Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d2dde-923">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="d2dde-924">Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`</span><span class="sxs-lookup"><span data-stu-id="d2dde-924">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-925">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-925">Appservice</span></span>

* <span data-ttu-id="d2dde-926">Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula</span><span class="sxs-lookup"><span data-stu-id="d2dde-926">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="d2dde-927">Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`</span><span class="sxs-lookup"><span data-stu-id="d2dde-927">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="d2dde-928">CDN</span><span class="sxs-lookup"><span data-stu-id="d2dde-928">CDN</span></span>

* <span data-ttu-id="d2dde-929">Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-929">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-930">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-930">Container</span></span>

* <span data-ttu-id="d2dde-931">Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros</span><span class="sxs-lookup"><span data-stu-id="d2dde-931">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="d2dde-932">Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d2dde-932">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d2dde-933">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d2dde-933">CosmosDB</span></span>

* <span data-ttu-id="d2dde-934">Se ha agregado compatibilidad para la configuración de funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d2dde-934">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-935">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-935">Extension</span></span>

* <span data-ttu-id="d2dde-936">Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-936">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="d2dde-937">Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-937">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="d2dde-938">Comentarios</span><span class="sxs-lookup"><span data-stu-id="d2dde-938">Feedback</span></span>

* <span data-ttu-id="d2dde-939">Se ha agregado información de la extensión a los datos de telemetría</span><span class="sxs-lookup"><span data-stu-id="d2dde-939">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-940">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-940">Interactive</span></span>

* <span data-ttu-id="d2dde-941">Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell</span><span class="sxs-lookup"><span data-stu-id="d2dde-941">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="d2dde-942">Se ha corregido la regresión con el completado de los parámetros que faltan</span><span class="sxs-lookup"><span data-stu-id="d2dde-942">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-943">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-943">IoT</span></span>

* <span data-ttu-id="d2dde-944">Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-944">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d2dde-945">Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-945">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="d2dde-946">Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-946">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="d2dde-947">Se ha cambiado `iot hub create` para permitir especificar el número de particiones</span><span class="sxs-lookup"><span data-stu-id="d2dde-947">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-948">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-948">Monitor</span></span>

* <span data-ttu-id="d2dde-949">Se ha corregido el comando `az monitor log-profiles create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-949">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-950">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-950">Network</span></span>

* <span data-ttu-id="d2dde-951">Se ha corregido la opción `--tags` en los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="d2dde-951">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="d2dde-952">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-952">Profile</span></span>

* <span data-ttu-id="d2dde-953">Se ha habilitado `az login` en el modo interactivo</span><span class="sxs-lookup"><span data-stu-id="d2dde-953">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-954">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-954">Resource</span></span>

* <span data-ttu-id="d2dde-955">Se ha agregado de nuevo `feature show`</span><span class="sxs-lookup"><span data-stu-id="d2dde-955">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-956">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-956">Role</span></span>

* <span data-ttu-id="d2dde-957">Se agregó el argumento `--available-to-other-tenants` a `ad app update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-957">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-958">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-958">SQL</span></span>

* <span data-ttu-id="d2dde-959">Se agregaron los comandos `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-959">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="d2dde-960">Se agregó `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-960">Added `sql db rename`</span></span>
* <span data-ttu-id="d2dde-961">Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql</span><span class="sxs-lookup"><span data-stu-id="d2dde-961">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-962">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-962">Storage</span></span>

* <span data-ttu-id="d2dde-963">Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal</span><span class="sxs-lookup"><span data-stu-id="d2dde-963">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-964">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-964">VM</span></span>

* <span data-ttu-id="d2dde-965">Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado</span><span class="sxs-lookup"><span data-stu-id="d2dde-965">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="d2dde-966">Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI</span><span class="sxs-lookup"><span data-stu-id="d2dde-966">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="d2dde-967">`vm boot-diagnostics get-boot-log` fija</span><span class="sxs-lookup"><span data-stu-id="d2dde-967">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="d2dde-968">31 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-968">January 31, 2018</span></span>

<span data-ttu-id="d2dde-969">Versión 2.0.26</span><span class="sxs-lookup"><span data-stu-id="d2dde-969">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-970">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-970">Core</span></span>

* <span data-ttu-id="d2dde-971">Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI</span><span class="sxs-lookup"><span data-stu-id="d2dde-971">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="d2dde-972">Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows</span><span class="sxs-lookup"><span data-stu-id="d2dde-972">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="d2dde-973">Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información.</span><span class="sxs-lookup"><span data-stu-id="d2dde-973">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="d2dde-974">Use `--verbose` para verlo</span><span class="sxs-lookup"><span data-stu-id="d2dde-974">Use `--verbose` to see</span></span>
* <span data-ttu-id="d2dde-975">Se ha agregado un indicador de progreso para los comandos de espera</span><span class="sxs-lookup"><span data-stu-id="d2dde-975">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-976">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-976">ACS</span></span>

* <span data-ttu-id="d2dde-977">Se ha aclarado el argumento `--disable-browser`</span><span class="sxs-lookup"><span data-stu-id="d2dde-977">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="d2dde-978">Se ha mejorado el completado con tabulación para los argumentos `--vm-size`</span><span class="sxs-lookup"><span data-stu-id="d2dde-978">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-979">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-979">Appservice</span></span>

* <span data-ttu-id="d2dde-980">`webapp log [tail|download]` fija</span><span class="sxs-lookup"><span data-stu-id="d2dde-980">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="d2dde-981">Se ha eliminado la comprobación `kind` en aplicaciones web y funciones</span><span class="sxs-lookup"><span data-stu-id="d2dde-981">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="d2dde-982">CDN</span><span class="sxs-lookup"><span data-stu-id="d2dde-982">CDN</span></span>

* <span data-ttu-id="d2dde-983">Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-983">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d2dde-984">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d2dde-984">CosmosDB</span></span>

* <span data-ttu-id="d2dde-985">Se ha corregido la descripción de parámetros en las directivas de conmutación por error</span><span class="sxs-lookup"><span data-stu-id="d2dde-985">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-986">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-986">Interactive</span></span>

* <span data-ttu-id="d2dde-987">Se ha corregido un problema por el que no aparecía el completado de las opciones del comando</span><span class="sxs-lookup"><span data-stu-id="d2dde-987">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-988">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-988">Network</span></span>

* <span data-ttu-id="d2dde-989">Se ha agregado protección para `--cert-password` en `application-gateway create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-989">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="d2dde-990">Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="d2dde-990">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="d2dde-991">Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-991">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="d2dde-992">Se ha corregido un problema de cliente no encontrado en `asg create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-992">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="d2dde-993">Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`</span><span class="sxs-lookup"><span data-stu-id="d2dde-993">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="d2dde-994">Se han corregido los problemas siguientes en `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="d2dde-994">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="d2dde-995">Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos</span><span class="sxs-lookup"><span data-stu-id="d2dde-995">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="d2dde-996">Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape</span><span class="sxs-lookup"><span data-stu-id="d2dde-996">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="d2dde-997">Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`</span><span class="sxs-lookup"><span data-stu-id="d2dde-997">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="d2dde-998">Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`</span><span class="sxs-lookup"><span data-stu-id="d2dde-998">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-999">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-999">Profile</span></span>

* <span data-ttu-id="d2dde-1000">Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad</span><span class="sxs-lookup"><span data-stu-id="d2dde-1000">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1001">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1001">Resource</span></span>

* <span data-ttu-id="d2dde-1002">Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas</span><span class="sxs-lookup"><span data-stu-id="d2dde-1002">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1003">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1003">Storage</span></span>

* <span data-ttu-id="d2dde-1004">Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2</span><span class="sxs-lookup"><span data-stu-id="d2dde-1004">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="d2dde-1005">Se ha agregado un informe de progreso a todos los comandos de carga y descarga</span><span class="sxs-lookup"><span data-stu-id="d2dde-1005">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="d2dde-1006">Se ha corregido un error en la opción "-n" en `storage account check-name`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1006">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="d2dde-1007">Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1007">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="d2dde-1008">Se han corregido errores en varios parámetros que debían analizarse como enteros</span><span class="sxs-lookup"><span data-stu-id="d2dde-1008">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1009">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1009">VM</span></span>

* <span data-ttu-id="d2dde-1010">Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales</span><span class="sxs-lookup"><span data-stu-id="d2dde-1010">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="d2dde-1011">Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1011">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="d2dde-1012">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="d2dde-1012">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="d2dde-1013">Se ha agregado protección para `--admin-password` en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1013">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="d2dde-1014">17 de enero de 2018</span><span class="sxs-lookup"><span data-stu-id="d2dde-1014">January 17, 2018</span></span>

<span data-ttu-id="d2dde-1015">Versión 2.0.25</span><span class="sxs-lookup"><span data-stu-id="d2dde-1015">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-1016">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-1016">ACR</span></span>

* <span data-ttu-id="d2dde-1017">Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows</span><span class="sxs-lookup"><span data-stu-id="d2dde-1017">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="d2dde-1018">Se han habilitado los registros del registro</span><span class="sxs-lookup"><span data-stu-id="d2dde-1018">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1019">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1019">ACS</span></span>

* <span data-ttu-id="d2dde-1020">Se ha corregido el comando `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1020">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="d2dde-1021">Se ha eliminado el requisito de rol SPN</span><span class="sxs-lookup"><span data-stu-id="d2dde-1021">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1022">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1022">Appservice</span></span>

* <span data-ttu-id="d2dde-1023">Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL</span><span class="sxs-lookup"><span data-stu-id="d2dde-1023">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="d2dde-1024">Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1024">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="d2dde-1025">Se ha corregido la compatibilidad con ranuras en `log tail`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1025">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="d2dde-1026">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="d2dde-1026">Backup</span></span>

* <span data-ttu-id="d2dde-1027">Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional</span><span class="sxs-lookup"><span data-stu-id="d2dde-1027">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="d2dde-1028">Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1028">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="d2dde-1029">Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas</span><span class="sxs-lookup"><span data-stu-id="d2dde-1029">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="d2dde-1030">Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido</span><span class="sxs-lookup"><span data-stu-id="d2dde-1030">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="d2dde-1031">Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada</span><span class="sxs-lookup"><span data-stu-id="d2dde-1031">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-1032">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-1032">Batch</span></span>

* <span data-ttu-id="d2dde-1033">Se ha cambiado `batch login` para devolver los detalles de la autenticación</span><span class="sxs-lookup"><span data-stu-id="d2dde-1033">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="d2dde-1034">Nube</span><span class="sxs-lookup"><span data-stu-id="d2dde-1034">Cloud</span></span>

* <span data-ttu-id="d2dde-1035">Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube</span><span class="sxs-lookup"><span data-stu-id="d2dde-1035">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="d2dde-1036">Consumo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1036">Consumption</span></span>

* <span data-ttu-id="d2dde-1037">Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1037">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="d2dde-1038">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d2dde-1038">Event Grid</span></span>

* <span data-ttu-id="d2dde-1039">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1039">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d2dde-1040">[CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1040">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="d2dde-1041">[CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1041">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="d2dde-1042">Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1042">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="d2dde-1043">Se ha agregado el comando `eventgrid topic update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1043">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="d2dde-1044">Se ha agregado el comando `eventgrid event-subscription update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1044">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="d2dde-1045">Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1045">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="d2dde-1046">Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema</span><span class="sxs-lookup"><span data-stu-id="d2dde-1046">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-1047">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-1047">Interactive</span></span>

* <span data-ttu-id="d2dde-1048">Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x</span><span class="sxs-lookup"><span data-stu-id="d2dde-1048">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="d2dde-1049">Se han corregido errores en el inicio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1049">Fixed errors on startup</span></span>
* <span data-ttu-id="d2dde-1050">Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1050">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-1051">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-1051">IoT</span></span>

* <span data-ttu-id="d2dde-1052">Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1052">Added support for device provisioning service</span></span>
* <span data-ttu-id="d2dde-1053">Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1053">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="d2dde-1054">Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-1054">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-1055">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1055">Monitor</span></span>

* <span data-ttu-id="d2dde-1056">Se ha agregado compatibilidad con la configuración de múltiples diagnósticos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1056">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="d2dde-1057">El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1057">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="d2dde-1058">Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1058">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1059">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1059">Network</span></span>

* <span data-ttu-id="d2dde-1060">Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1060">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="d2dde-1061">Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1061">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-1062">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-1062">Profile</span></span>

* <span data-ttu-id="d2dde-1063">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="d2dde-1063">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-1064">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-1064">Role</span></span>

* <span data-ttu-id="d2dde-1065">Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph</span><span class="sxs-lookup"><span data-stu-id="d2dde-1065">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d2dde-1066">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d2dde-1066">Service Fabric</span></span>

* <span data-ttu-id="d2dde-1067">Se han agregado errores detallados a la respuesta de la validación en la creación del clúster</span><span class="sxs-lookup"><span data-stu-id="d2dde-1067">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="d2dde-1068">Se ha corregido un problema de cliente no encontrado en varios comandos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1068">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1069">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1069">VM</span></span>

* <span data-ttu-id="d2dde-1070">[VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1070">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="d2dde-1071">[CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"</span><span class="sxs-lookup"><span data-stu-id="d2dde-1071">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="d2dde-1072">[CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI</span><span class="sxs-lookup"><span data-stu-id="d2dde-1072">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="d2dde-1073">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1073">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="d2dde-1074">Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones</span><span class="sxs-lookup"><span data-stu-id="d2dde-1074">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="d2dde-1075">Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1075">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="d2dde-1076">Se han corregido problemas de error en `[vm|vmss] create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1076">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="d2dde-1077">Se ha corregido el uso excesivo de recursos producido por `vm image list --all`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1077">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="d2dde-1078">19 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1078">December 19, 2017</span></span>

<span data-ttu-id="d2dde-1079">Versión 2.0.23</span><span class="sxs-lookup"><span data-stu-id="d2dde-1079">Version 2.0.23</span></span>

* <span data-ttu-id="d2dde-1080">Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario</span><span class="sxs-lookup"><span data-stu-id="d2dde-1080">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-1081">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-1081">Container</span></span>

* <span data-ttu-id="d2dde-1082">Se corrigió el orden incorrecto de los parámetros en los registros del contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-1082">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1083">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1083">Network</span></span>

* <span data-ttu-id="d2dde-1084">Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1084">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="d2dde-1085">Se agregó el argumento `--ip-tags` a `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1085">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1086">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1086">Storage</span></span>

* <span data-ttu-id="d2dde-1087">Se agregó compatibilidad con almacenamiento V2</span><span class="sxs-lookup"><span data-stu-id="d2dde-1087">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1088">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1088">VM</span></span>

* <span data-ttu-id="d2dde-1089">[Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales</span><span class="sxs-lookup"><span data-stu-id="d2dde-1089">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="d2dde-1090">5 de diciembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1090">December 5, 2017</span></span>

<span data-ttu-id="d2dde-1091">Versión 2.0.22</span><span class="sxs-lookup"><span data-stu-id="d2dde-1091">Version 2.0.22</span></span>

* <span data-ttu-id="d2dde-1092">Se quitaron los comandos `az component`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1092">Removed `az component` commands.</span></span> <span data-ttu-id="d2dde-1093">Use `az extension` en su lugar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1093">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-1094">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1094">Core</span></span>
* <span data-ttu-id="d2dde-1095">Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us</span><span class="sxs-lookup"><span data-stu-id="d2dde-1095">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="d2dde-1096">Se corrigió el problema por el que se podía enviar datos de telemetría continuamente</span><span class="sxs-lookup"><span data-stu-id="d2dde-1096">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1097">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1097">ACS</span></span>

* <span data-ttu-id="d2dde-1098">Se agregaron los comandos `aks install-connector` y `aks remove-connector`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1098">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="d2dde-1099">Se mejoraron los informes de errores de `acs create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1099">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="d2dde-1100">Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa</span><span class="sxs-lookup"><span data-stu-id="d2dde-1100">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="d2dde-1101">Advisor</span><span class="sxs-lookup"><span data-stu-id="d2dde-1101">Advisor</span></span>

* <span data-ttu-id="d2dde-1102">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1102">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1103">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1103">Appservice</span></span>

* <span data-ttu-id="d2dde-1104">Se corrigió la generación de nombres de certificado con `webapp config ssl upload`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1104">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="d2dde-1105">Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas</span><span class="sxs-lookup"><span data-stu-id="d2dde-1105">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="d2dde-1106">Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1106">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="d2dde-1107">Consumo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1107">Consumption</span></span>

* <span data-ttu-id="d2dde-1108">Se agregó compatibilidad con la versión de API 2017-11-30</span><span class="sxs-lookup"><span data-stu-id="d2dde-1108">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-1109">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-1109">Container</span></span>

* <span data-ttu-id="d2dde-1110">Se corrigió la regresión de puertos predeterminados</span><span class="sxs-lookup"><span data-stu-id="d2dde-1110">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-1111">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1111">Monitor</span></span>

* <span data-ttu-id="d2dde-1112">Se agregó compatibilidad multidimensional al comando metrics</span><span class="sxs-lookup"><span data-stu-id="d2dde-1112">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1113">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1113">Resource</span></span>

* <span data-ttu-id="d2dde-1114">Se agregó el argumento `--include-response-body` a `resource show`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1114">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-1115">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-1115">Role</span></span>

* <span data-ttu-id="d2dde-1116">Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1116">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="d2dde-1117">Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir</span><span class="sxs-lookup"><span data-stu-id="d2dde-1117">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="d2dde-1118">Se mejoraron los informes de errores de `ad sp create-for-rbac`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1118">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-1119">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-1119">SQL</span></span>

* <span data-ttu-id="d2dde-1120">Se agregaron los comandos `sql db list-usages` y `sql db show-usage`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1120">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="d2dde-1121">Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1121">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1122">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1122">VM</span></span>

* <span data-ttu-id="d2dde-1123">Se agregó información de zona a `az vm list-skus`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1123">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="d2dde-1124">14 de noviembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1124">November 14, 2017</span></span>

<span data-ttu-id="d2dde-1125">Versión 2.0.21</span><span class="sxs-lookup"><span data-stu-id="d2dde-1125">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-1126">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-1126">ACR</span></span>

* <span data-ttu-id="d2dde-1127">Se agregó compatibilidad para crear webhooks en regiones de replicación</span><span class="sxs-lookup"><span data-stu-id="d2dde-1127">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="d2dde-1128">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1128">ACS</span></span>

* <span data-ttu-id="d2dde-1129">Se cambió el texto de "agente" a "nodo" en AKS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1129">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="d2dde-1130">Opción `--orchestrator-release` en desuso para `acs create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1130">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="d2dde-1131">Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1131">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="d2dde-1132">Se corrigió `az aks browse` en Windows</span><span class="sxs-lookup"><span data-stu-id="d2dde-1132">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="d2dde-1133">Se corrigió `az aks get-credentials` en Windows</span><span class="sxs-lookup"><span data-stu-id="d2dde-1133">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1134">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1134">Appservice</span></span>

* <span data-ttu-id="d2dde-1135">Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función</span><span class="sxs-lookup"><span data-stu-id="d2dde-1135">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="d2dde-1136">Se agregó la opción `--docker-container-logging` a `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1136">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="d2dde-1137">Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1137">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="d2dde-1138">Se mejoraron los mensajes de error de `deployment user set`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1138">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="d2dde-1139">Se agregó compatibilidad para crear aplicaciones de función Linux</span><span class="sxs-lookup"><span data-stu-id="d2dde-1139">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="d2dde-1140">`list-locations` fija</span><span class="sxs-lookup"><span data-stu-id="d2dde-1140">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-1141">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-1141">Batch</span></span>

* <span data-ttu-id="d2dde-1142">Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1142">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="d2dde-1143">Batchai</span><span class="sxs-lookup"><span data-stu-id="d2dde-1143">Batchai</span></span>

* <span data-ttu-id="d2dde-1144">Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1144">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="d2dde-1145">Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1145">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="d2dde-1146">Se corrigió la documentación de `job list-files` y `job stream-file`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1146">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="d2dde-1147">Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1147">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="d2dde-1148">Nube</span><span class="sxs-lookup"><span data-stu-id="d2dde-1148">Cloud</span></span>

* <span data-ttu-id="d2dde-1149">Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios</span><span class="sxs-lookup"><span data-stu-id="d2dde-1149">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-1150">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-1150">Container</span></span>

* <span data-ttu-id="d2dde-1151">Se agregó compatibilidad para abrir varios puertos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1151">Added support to open multiple ports</span></span>
* <span data-ttu-id="d2dde-1152">Se agregó la directiva de reinicio de grupo de contenedores</span><span class="sxs-lookup"><span data-stu-id="d2dde-1152">Added container group restart policy</span></span>
* <span data-ttu-id="d2dde-1153">Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen</span><span class="sxs-lookup"><span data-stu-id="d2dde-1153">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="d2dde-1154">Se actualizaron los documentos auxiliares</span><span class="sxs-lookup"><span data-stu-id="d2dde-1154">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d2dde-1155">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d2dde-1155">Data Lake Analytics</span></span>

* <span data-ttu-id="d2dde-1156">Se cambió `[job|account] list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="d2dde-1156">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d2dde-1157">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d2dde-1157">Data Lake Store</span></span>

* <span data-ttu-id="d2dde-1158">Se cambió `account list` para devolver información más concisa</span><span class="sxs-lookup"><span data-stu-id="d2dde-1158">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-1159">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1159">Extension</span></span>

* <span data-ttu-id="d2dde-1160">Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft</span><span class="sxs-lookup"><span data-stu-id="d2dde-1160">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="d2dde-1161">Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre</span><span class="sxs-lookup"><span data-stu-id="d2dde-1161">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-1162">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-1162">IoT</span></span>

* <span data-ttu-id="d2dde-1163">Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados</span><span class="sxs-lookup"><span data-stu-id="d2dde-1163">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-1164">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1164">Monitor</span></span>

* <span data-ttu-id="d2dde-1165">Se agregaron los comandos `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1165">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1166">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1166">Network</span></span>

* <span data-ttu-id="d2dde-1167">Se agregó compatibilidad para los registros DNS CAA</span><span class="sxs-lookup"><span data-stu-id="d2dde-1167">Added support for CAA DNS records</span></span>
* <span data-ttu-id="d2dde-1168">Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1168">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="d2dde-1169">Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1169">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="d2dde-1170">Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1170">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="d2dde-1171">Reservations</span><span class="sxs-lookup"><span data-stu-id="d2dde-1171">Reservations</span></span>

* <span data-ttu-id="d2dde-1172">Versión preliminar inicial</span><span class="sxs-lookup"><span data-stu-id="d2dde-1172">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1173">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1173">Resource</span></span>

* <span data-ttu-id="d2dde-1174">Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1174">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-1175">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-1175">SQL</span></span>

* <span data-ttu-id="d2dde-1176">Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1176">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1177">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1177">Storage</span></span>

* <span data-ttu-id="d2dde-1178">Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado</span><span class="sxs-lookup"><span data-stu-id="d2dde-1178">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="d2dde-1179">Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii</span><span class="sxs-lookup"><span data-stu-id="d2dde-1179">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="d2dde-1180">Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1180">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="d2dde-1181">Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1181">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="d2dde-1182">Se corrigió un problema al habilitar las métricas con `storage metrics update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1182">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="d2dde-1183">Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1183">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="d2dde-1184">Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1184">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1185">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1185">VM</span></span>

* <span data-ttu-id="d2dde-1186">Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1186">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="d2dde-1187">Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación</span><span class="sxs-lookup"><span data-stu-id="d2dde-1187">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="d2dde-1188">Se agregaron los comandos `vm secret `[add|remove|list]'</span><span class="sxs-lookup"><span data-stu-id="d2dde-1188">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="d2dde-1189">Se cambió el nombre de `vm format-secret` a `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1189">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="d2dde-1190">Se agregó el argumento `--encrypt format` a `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1190">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="d2dde-1191">24 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1191">October 24, 2017</span></span>

<span data-ttu-id="d2dde-1192">Versión 2.0.20</span><span class="sxs-lookup"><span data-stu-id="d2dde-1192">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-1193">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1193">Core</span></span>

* <span data-ttu-id="d2dde-1194">Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1194">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-1195">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-1195">ACR</span></span>

* <span data-ttu-id="d2dde-1196">Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API</span><span class="sxs-lookup"><span data-stu-id="d2dde-1196">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="d2dde-1197">Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica</span><span class="sxs-lookup"><span data-stu-id="d2dde-1197">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="d2dde-1198">Se cambió el nombre de la SKU de registro a Basic, Standard y Premium</span><span class="sxs-lookup"><span data-stu-id="d2dde-1198">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1199">ACS</span></span>

* <span data-ttu-id="d2dde-1200">[Versión preliminar] Se agregaron los comandos `az aks`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1200">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="d2dde-1201">Se corrigió `get-credentials` de Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d2dde-1201">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1202">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1202">Appservice</span></span>

* <span data-ttu-id="d2dde-1203">Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1203">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="d2dde-1204">Componente</span><span class="sxs-lookup"><span data-stu-id="d2dde-1204">Component</span></span>

* <span data-ttu-id="d2dde-1205">Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación</span><span class="sxs-lookup"><span data-stu-id="d2dde-1205">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-1206">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1206">Monitor</span></span>

* <span data-ttu-id="d2dde-1207">Se agregaron los comandos `action-group`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1207">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1208">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1208">Resource</span></span>

* <span data-ttu-id="d2dde-1209">Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1209">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="d2dde-1210">Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas</span><span class="sxs-lookup"><span data-stu-id="d2dde-1210">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1211">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1211">VM</span></span>

* <span data-ttu-id="d2dde-1212">Se agregó el argumento `--accelerated-networking` a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1212">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="d2dde-1213">9 de octubre de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1213">October 9, 2017</span></span>

<span data-ttu-id="d2dde-1214">Versión 2.0.19</span><span class="sxs-lookup"><span data-stu-id="d2dde-1214">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-1215">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1215">Core</span></span>

* <span data-ttu-id="d2dde-1216">Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d2dde-1216">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1217">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1217">Appservice</span></span>

* <span data-ttu-id="d2dde-1218">Se ha agregado una actualización genérica con el nuevo comando `webapp update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1218">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-1219">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-1219">Batch</span></span>

* <span data-ttu-id="d2dde-1220">Se ha actualizado a la versión SDK de Batch 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d2dde-1220">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="d2dde-1221">Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version</span><span class="sxs-lookup"><span data-stu-id="d2dde-1221">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="d2dde-1222">Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-1222">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="d2dde-1223">Se ha eliminado la compatibilidad con Batch del modelo de componente</span><span class="sxs-lookup"><span data-stu-id="d2dde-1223">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="d2dde-1224">Batchai</span><span class="sxs-lookup"><span data-stu-id="d2dde-1224">Batchai</span></span>

* <span data-ttu-id="d2dde-1225">Versión inicial del módulo de inteligencia artificial de Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-1225">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-1226">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d2dde-1226">Keyvault</span></span>

* <span data-ttu-id="d2dde-1227">Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1227">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="d2dde-1228">(#4448)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1228">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="d2dde-1229">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1229">Network</span></span>

* <span data-ttu-id="d2dde-1230">Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1230">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="d2dde-1231">Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes</span><span class="sxs-lookup"><span data-stu-id="d2dde-1231">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1232">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1232">Resource</span></span>

* <span data-ttu-id="d2dde-1233">Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1233">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="d2dde-1234">Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción</span><span class="sxs-lookup"><span data-stu-id="d2dde-1234">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="d2dde-1235">Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1235">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="d2dde-1236">Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1236">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-1237">Sql</span><span class="sxs-lookup"><span data-stu-id="d2dde-1237">Sql</span></span>

* <span data-ttu-id="d2dde-1238">Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key</span><span class="sxs-lookup"><span data-stu-id="d2dde-1238">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="d2dde-1239">Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas</span><span class="sxs-lookup"><span data-stu-id="d2dde-1239">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="d2dde-1240">Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1240">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1241">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1241">Storage</span></span>

* <span data-ttu-id="d2dde-1242">Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1242">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1243">Vm</span><span class="sxs-lookup"><span data-stu-id="d2dde-1243">Vm</span></span>

* <span data-ttu-id="d2dde-1244">Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan</span><span class="sxs-lookup"><span data-stu-id="d2dde-1244">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="d2dde-1245">[VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1245">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="d2dde-1246">Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1246">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="d2dde-1247">Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1247">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="d2dde-1248">Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1248">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="d2dde-1249">22 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1249">September 22, 2017</span></span>

<span data-ttu-id="d2dde-1250">Versión 2.0.18</span><span class="sxs-lookup"><span data-stu-id="d2dde-1250">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1251">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1251">Resource</span></span>

* <span data-ttu-id="d2dde-1252">Se agregó compatibilidad para mostrar las definiciones de directivas integradas</span><span class="sxs-lookup"><span data-stu-id="d2dde-1252">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="d2dde-1253">Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva</span><span class="sxs-lookup"><span data-stu-id="d2dde-1253">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="d2dde-1254">Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1254">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="d2dde-1255">[CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1255">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1256">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1256">Network</span></span>

* <span data-ttu-id="d2dde-1257">Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1257">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="d2dde-1258">Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1258">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="d2dde-1259">Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1259">Added `asg` application security group commands</span></span>
* <span data-ttu-id="d2dde-1260">Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1260">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="d2dde-1261">Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1261">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d2dde-1262">Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1262">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="d2dde-1263">Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1263">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1264">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1264">Storage</span></span>

* <span data-ttu-id="d2dde-1265">Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK</span><span class="sxs-lookup"><span data-stu-id="d2dde-1265">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="d2dde-1266">Eventgrid</span><span class="sxs-lookup"><span data-stu-id="d2dde-1266">Eventgrid</span></span>

* <span data-ttu-id="d2dde-1267">Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"</span><span class="sxs-lookup"><span data-stu-id="d2dde-1267">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-1268">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-1268">SQL</span></span>

* <span data-ttu-id="d2dde-1269">Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1269">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="d2dde-1270">Si no se especifica, se devolverán todos los servidores de SQL de la suscripción</span><span class="sxs-lookup"><span data-stu-id="d2dde-1270">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="d2dde-1271">Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1271">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-1272">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d2dde-1272">Keyvault</span></span>

* <span data-ttu-id="d2dde-1273">Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy</span><span class="sxs-lookup"><span data-stu-id="d2dde-1273">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1274">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1274">VM</span></span>

* <span data-ttu-id="d2dde-1275">Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1275">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="d2dde-1276">Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error</span><span class="sxs-lookup"><span data-stu-id="d2dde-1276">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="d2dde-1277">Se agregó el argumento `--asgs` a `vm create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1277">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="d2dde-1278">Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1278">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="d2dde-1279">[VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1279">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="d2dde-1280">Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1280">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1281">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1281">ACS</span></span>

* <span data-ttu-id="d2dde-1282">[VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1282">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1283">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1283">Appservice</span></span>

* <span data-ttu-id="d2dde-1284">Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1284">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="d2dde-1285">Copia de seguridad</span><span class="sxs-lookup"><span data-stu-id="d2dde-1285">Backup</span></span>

* <span data-ttu-id="d2dde-1286">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1286">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="d2dde-1287">11 de septiembre de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1287">September 11, 2017</span></span>

<span data-ttu-id="d2dde-1288">Versión 2.0.17</span><span class="sxs-lookup"><span data-stu-id="d2dde-1288">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="d2dde-1289">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1289">Core</span></span>

* <span data-ttu-id="d2dde-1290">Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1290">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="d2dde-1291">Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1291">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1292">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1292">Acs</span></span>

* <span data-ttu-id="d2dde-1293">Se agregó el comando `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1293">Added `acs list-locations` command</span></span>
* <span data-ttu-id="d2dde-1294">Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1294">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1295">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1295">Appservice</span></span>

* <span data-ttu-id="d2dde-1296">Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1296">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="d2dde-1297">CDN</span><span class="sxs-lookup"><span data-stu-id="d2dde-1297">CDN</span></span>

* <span data-ttu-id="d2dde-1298">Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1298">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="d2dde-1299">Extensión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1299">Extension</span></span>

* <span data-ttu-id="d2dde-1300">Versión inicial</span><span class="sxs-lookup"><span data-stu-id="d2dde-1300">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-1301">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d2dde-1301">Keyvault</span></span>

* <span data-ttu-id="d2dde-1302">Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1302">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1303">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1303">Network</span></span>

* <span data-ttu-id="d2dde-1304">Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1304">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d2dde-1305">Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1305">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="d2dde-1306">Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1306">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="d2dde-1307">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1307">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d2dde-1308">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1308">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1309">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1309">Resource</span></span>

* <span data-ttu-id="d2dde-1310">Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1310">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="d2dde-1311">Se permite pasar valores de parámetro para `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1311">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="d2dde-1312">Se permite pasar código JSON o archivo para todos los parámetros.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1312">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="d2dde-1313">Versión de API incrementada</span><span class="sxs-lookup"><span data-stu-id="d2dde-1313">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-1314">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-1314">SQL</span></span>

* <span data-ttu-id="d2dde-1315">Se agregaron los comandos `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1315">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1316">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1316">VM</span></span>

* <span data-ttu-id="d2dde-1317">Corregido: No asignar acceso a menos que se proporcione `--scope`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1317">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="d2dde-1318">Corregido: Usar para las extensiones la misma nomenclatura que el portal.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1318">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="d2dde-1319">Se quitó `subscription` de la salida `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1319">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="d2dde-1320">Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1320">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="d2dde-1321">Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1321">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="d2dde-1322">31 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1322">August 31, 2017</span></span>

<span data-ttu-id="d2dde-1323">Versión 2.0.16</span><span class="sxs-lookup"><span data-stu-id="d2dde-1323">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-1324">Keyvault</span><span class="sxs-lookup"><span data-stu-id="d2dde-1324">Keyvault</span></span>

* <span data-ttu-id="d2dde-1325">Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1325">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="d2dde-1326">Sf</span><span class="sxs-lookup"><span data-stu-id="d2dde-1326">Sf</span></span>

* <span data-ttu-id="d2dde-1327">Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1327">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1328">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1328">Storage</span></span>

* <span data-ttu-id="d2dde-1329">Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1329">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="d2dde-1330">Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1330">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="d2dde-1331">28 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1331">August 28, 2017</span></span>

<span data-ttu-id="d2dde-1332">Version 2.0.15</span><span class="sxs-lookup"><span data-stu-id="d2dde-1332">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="d2dde-1333">CLI</span><span class="sxs-lookup"><span data-stu-id="d2dde-1333">CLI</span></span>

* <span data-ttu-id="d2dde-1334">Se ha agregado una nota legal a `--version`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1334">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1335">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1335">ACS</span></span>

* <span data-ttu-id="d2dde-1336">Se han corregido las regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1336">Corrected preview regions</span></span>
* <span data-ttu-id="d2dde-1337">Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1337">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="d2dde-1338">Se ha optimizado la salida del comando acs</span><span class="sxs-lookup"><span data-stu-id="d2dde-1338">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1339">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1339">Appservice</span></span>

* <span data-ttu-id="d2dde-1340">[CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1340">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="d2dde-1341">Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1341">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="d2dde-1342">Se expuso `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1342">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="d2dde-1343">Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1343">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="d2dde-1344">Corregido: Las configuración de los espacios se detecta correctamente.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1344">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-1345">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-1345">IoT</span></span>

* <span data-ttu-id="d2dde-1346">Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1346">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1347">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1347">Network</span></span>

* <span data-ttu-id="d2dde-1348">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1348">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="d2dde-1349">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1349">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="d2dde-1350">Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1350">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="d2dde-1351">Se agregó compatibilidad para SKU a `lb create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1351">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="d2dde-1352">Se agregó compatibilidad para SKU a `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1352">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-1353">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-1353">Profile</span></span>

* <span data-ttu-id="d2dde-1354">Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1354">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d2dde-1355">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d2dde-1355">Service Fabric</span></span>

* <span data-ttu-id="d2dde-1356">Versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1356">Preview release</span></span>
* <span data-ttu-id="d2dde-1357">Se simplificaron las reglas de usuario y contraseña de registro para los comandos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1357">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="d2dde-1358">Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1358">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="d2dde-1359">Se agregó compatibilidad para valores vacíos de `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1359">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1360">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1360">Storage</span></span>

* <span data-ttu-id="d2dde-1361">Se habilitó la configuración de la capa de blobs.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1361">Enabled setting blob tier</span></span>
* <span data-ttu-id="d2dde-1362">Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1362">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="d2dde-1363">Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1363">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="d2dde-1364">Se habilitó el cifrado del servicio por clave administrada de cliente.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1364">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="d2dde-1365">[CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1365">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="d2dde-1366">Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis</span><span class="sxs-lookup"><span data-stu-id="d2dde-1366">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1367">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1367">VM</span></span>

* <span data-ttu-id="d2dde-1368">Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1368">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="d2dde-1369">Se agregó compatibilidad para `--lb-sku` a `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1369">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="d2dde-1370">Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1370">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="d2dde-1371">Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1371">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="d2dde-1372">Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1372">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="d2dde-1373">Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1373">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="d2dde-1374">15 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1374">August 15, 2017</span></span>

<span data-ttu-id="d2dde-1375">Versión 2.0.14</span><span class="sxs-lookup"><span data-stu-id="d2dde-1375">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1376">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1376">ACS</span></span>

* <span data-ttu-id="d2dde-1377">Se corrigió el número de puerto sshMaster0 para Kubernetes</span><span class="sxs-lookup"><span data-stu-id="d2dde-1377">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1378">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1378">Appservice</span></span>

* <span data-ttu-id="d2dde-1379">Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1379">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="d2dde-1380">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d2dde-1380">Event Grid</span></span>

* <span data-ttu-id="d2dde-1381">Se agregaron dependencias del SDK.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1381">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="d2dde-1382">11 de agosto de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1382">August 11, 2017</span></span>

<span data-ttu-id="d2dde-1383">Versión 2.0.13</span><span class="sxs-lookup"><span data-stu-id="d2dde-1383">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1384">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1384">ACS</span></span>

* <span data-ttu-id="d2dde-1385">Se agregaron más regiones en versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1385">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-1386">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-1386">Batch</span></span>

* <span data-ttu-id="d2dde-1387">Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1387">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="d2dde-1388">Se agregó un nuevo comando que muestra el número de tareas de un trabajo.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1388">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="d2dde-1389">Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1389">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="d2dde-1390">El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1390">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="d2dde-1391">Compatibilidad para agregar listas de más de 100 tareas a un trabajo.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1391">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="d2dde-1392">Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1392">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="d2dde-1393">Componente</span><span class="sxs-lookup"><span data-stu-id="d2dde-1393">Component</span></span>

* <span data-ttu-id="d2dde-1394">Se agregó una advertencia de comandos 'az component' en desuso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1394">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="d2dde-1395">Contenedor</span><span class="sxs-lookup"><span data-stu-id="d2dde-1395">Container</span></span>

* <span data-ttu-id="d2dde-1396">`create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1396">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="d2dde-1397">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d2dde-1397">Data Lake Store</span></span>

* <span data-ttu-id="d2dde-1398">Control de progreso habilitado.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1398">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="d2dde-1399">Event Grid</span><span class="sxs-lookup"><span data-stu-id="d2dde-1399">Event Grid</span></span>

* <span data-ttu-id="d2dde-1400">Versión inicial.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1400">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1401">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1401">Network</span></span>

* <span data-ttu-id="d2dde-1402">`lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1402">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="d2dde-1403">`application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1403">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="d2dde-1404">`application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1404">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="d2dde-1405">Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1405">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-1406">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-1406">Profile</span></span>

* <span data-ttu-id="d2dde-1407">`account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1407">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1408">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1408">Storage</span></span>

* <span data-ttu-id="d2dde-1409">Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1409">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1410">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1410">VM</span></span>

* <span data-ttu-id="d2dde-1411">`availability-set`: número de dominios de error expuesto al convertir.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1411">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="d2dde-1412">Se expuso el comando `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1412">Exposed `list-skus` command</span></span>
* <span data-ttu-id="d2dde-1413">Compatibilidad para asignar identidades sin crear asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1413">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="d2dde-1414">Aplicación de SKU de almacenamiento al conectar discos de datos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1414">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="d2dde-1415">Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1415">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="d2dde-1416">28 de julio de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1416">July 28, 2017</span></span>

<span data-ttu-id="d2dde-1417">Versión 2.0.12</span><span class="sxs-lookup"><span data-stu-id="d2dde-1417">Version 2.0.12</span></span>

* <span data-ttu-id="d2dde-1418">Se agregaron comandos de contenedor.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1418">Added container commands</span></span>
* <span data-ttu-id="d2dde-1419">Se agregaron módulos de facturación y consumo.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1419">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="d2dde-1420">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1420">Core</span></span>

* <span data-ttu-id="d2dde-1421">Información de autenticación de SDK de salida para entidades de servicio con certificados.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1421">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="d2dde-1422">Se corrigieron las excepciones de progreso de la implementación.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1422">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="d2dde-1423">Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1423">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="d2dde-1424">Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1424">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="d2dde-1425">Actualización del identificador de solicitud de cliente para cada ejecución de comando.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1425">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="d2dde-1426">Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1426">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="d2dde-1427">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1427">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d2dde-1428">Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1428">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="d2dde-1429">Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1429">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="d2dde-1430">Creación de clientes de suscripción con el perfil de SDK correcto.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1430">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="d2dde-1431">Traslado de todos los archivos de registro existentes a la última carpeta.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1431">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="d2dde-1432">Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1432">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="d2dde-1433">Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1433">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="d2dde-1434">Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1434">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="d2dde-1435">Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1435">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="d2dde-1436">Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1436">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="d2dde-1437">ACR</span><span class="sxs-lookup"><span data-stu-id="d2dde-1437">ACR</span></span>

* <span data-ttu-id="d2dde-1438">Se agregó el comando `show-usage` para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1438">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="d2dde-1439">Compatibilidad con la actualización de SKU para los registros administrados.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1439">Support SKU update for managed registries</span></span>
* <span data-ttu-id="d2dde-1440">Se agregaron registros administrados con SKU administradas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1440">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="d2dde-1441">Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1441">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="d2dde-1442">Se agregó autenticación de AAD con el comando arc login.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1442">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="d2dde-1443">Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1443">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1444">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1444">ACS</span></span>

* <span data-ttu-id="d2dde-1445">Compatibilidad con la versión de API 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1445">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1446">Appservice</span><span class="sxs-lookup"><span data-stu-id="d2dde-1446">Appservice</span></span>

* <span data-ttu-id="d2dde-1447">Se corrigió el error por el que webapp de Linux no devolvía nada.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1447">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="d2dde-1448">Compatibilidad para recuperar credenciales de acr.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1448">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="d2dde-1449">Eliminación de todos los comandos en `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1449">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="d2dde-1450">Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1450">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="d2dde-1451">Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1451">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="d2dde-1452">Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1452">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="d2dde-1453">Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1453">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="d2dde-1454">Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1454">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="d2dde-1455">Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1455">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="d2dde-1456">Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1456">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="d2dde-1457">Batch</span><span class="sxs-lookup"><span data-stu-id="d2dde-1457">Batch</span></span>

* <span data-ttu-id="d2dde-1458">Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1458">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="d2dde-1459">Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1459">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="d2dde-1460">Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1460">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="d2dde-1461">CDN</span><span class="sxs-lookup"><span data-stu-id="d2dde-1461">CDN</span></span>

* <span data-ttu-id="d2dde-1462">Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe</span><span class="sxs-lookup"><span data-stu-id="d2dde-1462">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="d2dde-1463">Nube</span><span class="sxs-lookup"><span data-stu-id="d2dde-1463">Cloud</span></span>

* <span data-ttu-id="d2dde-1464">Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1464">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="d2dde-1465">No es necesario el punto de conexión de la galería.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1465">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="d2dde-1466">Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1466">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="d2dde-1467">Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1467">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="d2dde-1468">Se expuso `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1468">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d2dde-1469">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d2dde-1469">CosmosDB</span></span>

* <span data-ttu-id="d2dde-1470">Se corrigió poder crear una colección con clave de partición personalizada.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1470">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="d2dde-1471">Se ha agregado compatibilidad para TTL predeterminado de colección</span><span class="sxs-lookup"><span data-stu-id="d2dde-1471">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d2dde-1472">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d2dde-1472">Data Lake Analytics</span></span>

* <span data-ttu-id="d2dde-1473">Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1473">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="d2dde-1474">Se agregó `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1474">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="d2dde-1475">Se agregó `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1475">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d2dde-1476">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d2dde-1476">Data Lake Store</span></span>

* <span data-ttu-id="d2dde-1477">Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1477">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="d2dde-1478">Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1478">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="d2dde-1479">Se agregó el comando `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1479">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="d2dde-1480">Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1480">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="d2dde-1481">Interactive</span><span class="sxs-lookup"><span data-stu-id="d2dde-1481">Interactive</span></span>

* <span data-ttu-id="d2dde-1482">Se mejoró el tiempo de inicio mediante el uso de comandos en caché.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1482">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="d2dde-1483">Mayor cobertura de las pruebas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1483">Increased test coverage</span></span>
* <span data-ttu-id="d2dde-1484">Se mejoró el gesto "?" para insertar también en el siguiente comando.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1484">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="d2dde-1485">Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1485">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="d2dde-1486">Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1486">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="d2dde-1487">El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1487">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="d2dde-1488">Informes de progreso para las implementaciones de plantilla (n.º 3510).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1488">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="d2dde-1489">Se agregó la marca `--progress`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1489">Added `--progress` flag</span></span>
* <span data-ttu-id="d2dde-1490">Se quitó `--debug` y `--verbose` de la finalización.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1490">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="d2dde-1491">Se quitó `interactive` de las finalizaciones (n.º 3324).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1491">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="d2dde-1492">IoT</span><span class="sxs-lookup"><span data-stu-id="d2dde-1492">IoT</span></span>

* <span data-ttu-id="d2dde-1493">La creación de directivas ya no borra las directivas existentes.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1493">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="d2dde-1494">(n.º 3934)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1494">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="d2dde-1495">Almacén de claves</span><span class="sxs-lookup"><span data-stu-id="d2dde-1495">Key vault</span></span>

* <span data-ttu-id="d2dde-1496">Se agregaron comandos para características de recuperación de almacén de claves:</span><span class="sxs-lookup"><span data-stu-id="d2dde-1496">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="d2dde-1497">Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1497">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="d2dde-1498">Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1498">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d2dde-1499">Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1499">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="d2dde-1500">Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1500">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="d2dde-1501">Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1501">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="d2dde-1502">Se actualizó el plano de datos del almacén de claves a 0.3.2</span><span class="sxs-lookup"><span data-stu-id="d2dde-1502">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="d2dde-1503">(n.º 3307).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1503">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="d2dde-1504">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1504">Lab</span></span>

* <span data-ttu-id="d2dde-1505">Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1505">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="d2dde-1506">Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1506">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-1507">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1507">Monitor</span></span>

* <span data-ttu-id="d2dde-1508">Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1508">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="d2dde-1509">Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1509">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="d2dde-1510">Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1510">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="d2dde-1511">Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1511">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="d2dde-1512">Se cambió el nombre de `monitor alert-rules` a `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1512">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="d2dde-1513">Se cambió `monitor alert create`:</span><span class="sxs-lookup"><span data-stu-id="d2dde-1513">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="d2dde-1514">los subcomandos `condition` y `action` ya no aceptan JSON.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1514">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="d2dde-1515">Se agregaron varios parámetros para simplificar el proceso de creación de reglas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1515">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="d2dde-1516">`location` ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1516">`location` no longer required</span></span>
  * <span data-ttu-id="d2dde-1517">Se agregó compatibilidad para el nombre y el identificador de destino.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1517">Add name and ID support for target</span></span>
  * <span data-ttu-id="d2dde-1518">Se eliminó `--alert-rule-resource-name`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1518">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="d2dde-1519">Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1519">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="d2dde-1520">El valor predeterminado de `description` ahora se en la condición proporcionada.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1520">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="d2dde-1521">Se agregaron ejemplos para ayudar a aclarar el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1521">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="d2dde-1522">Se admiten nombres o identificadores para los comandos `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1522">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="d2dde-1523">Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1523">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1524">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1524">Network</span></span>

* <span data-ttu-id="d2dde-1525">Se agregó el comando `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1525">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="d2dde-1526">Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1526">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="d2dde-1527">Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1527">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="d2dde-1528">Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1528">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="d2dde-1529">Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1529">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="d2dde-1530">Se agregaron los comandos `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1530">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="d2dde-1531">Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1531">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="d2dde-1532">Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1532">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="d2dde-1533">Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1533">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="d2dde-1534">Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1534">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="d2dde-1535">Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1535">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="d2dde-1536">Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1536">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="d2dde-1537">Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1537">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="d2dde-1538">Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1538">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="d2dde-1539">Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1539">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="d2dde-1540">Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1540">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="d2dde-1541">Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1541">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="d2dde-1542">Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1542">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="d2dde-1543">Se agregó compatibilidad para `--dns-servers` a `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1543">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="d2dde-1544">Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1544">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="d2dde-1545">Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1545">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="d2dde-1546">Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1546">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="d2dde-1547">Se mejoró el formato de salida de `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1547">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="d2dde-1548">Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1548">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="d2dde-1549">Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1549">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="d2dde-1550">Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1550">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="d2dde-1551">Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1551">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-1552">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-1552">Profile</span></span>

* <span data-ttu-id="d2dde-1553">Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1553">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="d2dde-1554">Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1554">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="d2dde-1555">Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".</span><span class="sxs-lookup"><span data-stu-id="d2dde-1555">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="d2dde-1556">Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1556">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="d2dde-1557">Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1557">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="d2dde-1558">RDBMS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1558">RDBMS</span></span>

* <span data-ttu-id="d2dde-1559">Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1559">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="d2dde-1560">Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1560">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="d2dde-1561">Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1561">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="d2dde-1562">Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1562">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1563">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1563">Resource</span></span>

* <span data-ttu-id="d2dde-1564">Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1564">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="d2dde-1565">Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1565">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="d2dde-1566">Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1566">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="d2dde-1567">Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1567">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="d2dde-1568">Se corrigieron algunos mensajes de error y de análisis (n.º 3584).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1568">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="d2dde-1569">Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1569">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="d2dde-1570">Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1570">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="d2dde-1571">Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1571">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-1572">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-1572">Role</span></span>

* <span data-ttu-id="d2dde-1573">Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1573">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="d2dde-1574">Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1574">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="d2dde-1575">Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1575">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="d2dde-1576">Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1576">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="d2dde-1577">Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1577">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="d2dde-1578">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d2dde-1578">Service Fabric</span></span>
* <span data-ttu-id="d2dde-1579">Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1579">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="d2dde-1580">Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1580">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="d2dde-1581">Se corrigieron numerosos comandos de Service Fabric (n.º 3234).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1581">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-1582">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-1582">SQL</span></span>

* <span data-ttu-id="d2dde-1583">Se quitó el parámetro `sql server create` `--identity` roto.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1583">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="d2dde-1584">Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1584">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="d2dde-1585">Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1585">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1586">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1586">Storage</span></span>

* <span data-ttu-id="d2dde-1587">Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1587">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="d2dde-1588">Se habilitó la creación de una cuenta de almacenamiento solo https.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1588">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="d2dde-1589">Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1589">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="d2dde-1590">Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1590">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="d2dde-1591">El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1591">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="d2dde-1592">Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1592">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1593">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1593">VM</span></span>

* <span data-ttu-id="d2dde-1594">Compatibilidad para configurar nsg</span><span class="sxs-lookup"><span data-stu-id="d2dde-1594">Support configuring nsg</span></span>
* <span data-ttu-id="d2dde-1595">Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1595">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="d2dde-1596">Compatibilidad para identidades de servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1596">Support managed service identities</span></span>
* <span data-ttu-id="d2dde-1597">Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1597">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="d2dde-1598">Los discos de datos que se crean con `vm image create` comienzan con lun 0</span><span class="sxs-lookup"><span data-stu-id="d2dde-1598">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="d2dde-1599">10 de mayo de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1599">May 10, 2017</span></span>

<span data-ttu-id="d2dde-1600">Versión 2.0.6</span><span class="sxs-lookup"><span data-stu-id="d2dde-1600">Version 2.0.6</span></span>

* <span data-ttu-id="d2dde-1601">Se cambia el nombre de DocumentDB por CosmosDB.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1601">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="d2dde-1602">Se agrega RDBMS (MySQL y Postgres).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1602">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="d2dde-1603">Se incluyen los módulos de Data Lake Analytics y Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d2dde-1603">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="d2dde-1604">Se incluye el módulo de Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="d2dde-1604">Include Cognitive Services module</span></span>
* <span data-ttu-id="d2dde-1605">Se incluye el módulo de Service Fabric</span><span class="sxs-lookup"><span data-stu-id="d2dde-1605">Include Service Fabric module</span></span>
* <span data-ttu-id="d2dde-1606">Se incluye el módulo de Interactive (se cambia el nombre de az-shell)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1606">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="d2dde-1607">Se agrega compatibilidad para los comandos de CDN</span><span class="sxs-lookup"><span data-stu-id="d2dde-1607">Add support for CDN commands</span></span>
* <span data-ttu-id="d2dde-1608">Se quita el módulo de Container</span><span class="sxs-lookup"><span data-stu-id="d2dde-1608">Remove Container module</span></span>
* <span data-ttu-id="d2dde-1609">Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1609">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="d2dde-1610">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1610">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="d2dde-1611">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1611">Core</span></span>

* <span data-ttu-id="d2dde-1612">core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente</span><span class="sxs-lookup"><span data-stu-id="d2dde-1612">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="d2dde-1613">perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1613">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="d2dde-1614">Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1614">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="d2dde-1615">Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1615">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="d2dde-1616">Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1616">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="d2dde-1617">login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1617">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="d2dde-1618">core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1618">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="d2dde-1619">core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1619">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="d2dde-1620">core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1620">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="d2dde-1621">core: rendimiento mejorado</span><span class="sxs-lookup"><span data-stu-id="d2dde-1621">core: Improved performance</span></span>
* <span data-ttu-id="d2dde-1622">core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE</span><span class="sxs-lookup"><span data-stu-id="d2dde-1622">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="d2dde-1623">core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido</span><span class="sxs-lookup"><span data-stu-id="d2dde-1623">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1624">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1624">ACS</span></span>

* <span data-ttu-id="d2dde-1625">Corregir el número principal y de agentes para que sea un entero en lugar de una cadena</span><span class="sxs-lookup"><span data-stu-id="d2dde-1625">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="d2dde-1626">Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica</span><span class="sxs-lookup"><span data-stu-id="d2dde-1626">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="d2dde-1627">Exponer "az acs create --validate" para validaciones de simulacro</span><span class="sxs-lookup"><span data-stu-id="d2dde-1627">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="d2dde-1628">Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1628">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1629">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-1629">AppService</span></span>

* <span data-ttu-id="d2dde-1630">functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1630">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="d2dde-1631">Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"</span><span class="sxs-lookup"><span data-stu-id="d2dde-1631">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="d2dde-1632">Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1632">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="d2dde-1633">Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web</span><span class="sxs-lookup"><span data-stu-id="d2dde-1633">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="d2dde-1634">Exponer "webapp list-runtimes"</span><span class="sxs-lookup"><span data-stu-id="d2dde-1634">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="d2dde-1635">Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1635">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="d2dde-1636">Admitir el intercambio de espacios con versión preliminar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1636">support slot swap with preview</span></span>
* <span data-ttu-id="d2dde-1637">Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1637">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="d2dde-1638">Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1638">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="d2dde-1639">CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d2dde-1639">CosmosDB</span></span>

* <span data-ttu-id="d2dde-1640">Se cambia el nombre del módulo de DocumentDB por CosmosDB</span><span class="sxs-lookup"><span data-stu-id="d2dde-1640">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="d2dde-1641">Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1641">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="d2dde-1642">Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos</span><span class="sxs-lookup"><span data-stu-id="d2dde-1642">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="d2dde-1643">Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix</span><span class="sxs-lookup"><span data-stu-id="d2dde-1643">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="d2dde-1644">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d2dde-1644">Data Lake Analytics</span></span>

* <span data-ttu-id="d2dde-1645">Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error</span><span class="sxs-lookup"><span data-stu-id="d2dde-1645">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="d2dde-1646">Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete</span><span class="sxs-lookup"><span data-stu-id="d2dde-1646">Add support for new catalog item type: package.</span></span> <span data-ttu-id="d2dde-1647">al que se accede a través de: `az dla catalog package`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1647">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="d2dde-1648">Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):</span><span class="sxs-lookup"><span data-stu-id="d2dde-1648">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="d2dde-1649">Tabla</span><span class="sxs-lookup"><span data-stu-id="d2dde-1649">Table</span></span>
  * <span data-ttu-id="d2dde-1650">Función con valores de tabla</span><span class="sxs-lookup"><span data-stu-id="d2dde-1650">Table valued function</span></span>
  * <span data-ttu-id="d2dde-1651">Ver</span><span class="sxs-lookup"><span data-stu-id="d2dde-1651">View</span></span>
  * <span data-ttu-id="d2dde-1652">Estadísticas de tabla.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1652">Table Statistics.</span></span> <span data-ttu-id="d2dde-1653">Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla</span><span class="sxs-lookup"><span data-stu-id="d2dde-1653">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="d2dde-1654">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d2dde-1654">Data Lake Store</span></span>

* <span data-ttu-id="d2dde-1655">Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor</span><span class="sxs-lookup"><span data-stu-id="d2dde-1655">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="d2dde-1656">Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1656">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="d2dde-1657">Falta ayuda para mostrar el acceso.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1657">missed help for access show.</span></span> <span data-ttu-id="d2dde-1658">Se va a agregar.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1658">adding it.</span></span> <span data-ttu-id="d2dde-1659">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1659">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="d2dde-1660">Buscar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1660">Find</span></span>

* <span data-ttu-id="d2dde-1661">Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda</span><span class="sxs-lookup"><span data-stu-id="d2dde-1661">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="d2dde-1662">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d2dde-1662">KeyVault</span></span>

* <span data-ttu-id="d2dde-1663">BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones</span><span class="sxs-lookup"><span data-stu-id="d2dde-1663">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="d2dde-1664">BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros</span><span class="sxs-lookup"><span data-stu-id="d2dde-1664">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="d2dde-1665">Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy</span><span class="sxs-lookup"><span data-stu-id="d2dde-1665">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="d2dde-1666">Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"</span><span class="sxs-lookup"><span data-stu-id="d2dde-1666">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="d2dde-1667">Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1667">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="d2dde-1668">Laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1668">Lab</span></span>

* <span data-ttu-id="d2dde-1669">Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1669">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="d2dde-1670">Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1670">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="d2dde-1671">Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1671">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="d2dde-1672">Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1672">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="d2dde-1673">Se agregan comandos para administrar secretos en un laboratorio</span><span class="sxs-lookup"><span data-stu-id="d2dde-1673">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="d2dde-1674">Supervisión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1674">Monitor</span></span>

* <span data-ttu-id="d2dde-1675">Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1675">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="d2dde-1676">Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1676">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="d2dde-1677">Red</span><span class="sxs-lookup"><span data-stu-id="d2dde-1677">Network</span></span>

* <span data-ttu-id="d2dde-1678">Se agrega el comando `network watcher test-connectivity`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1678">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="d2dde-1679">Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1679">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="d2dde-1680">Se agrega compatibilidad para el drenaje de conexiones de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="d2dde-1680">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="d2dde-1681">Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway</span><span class="sxs-lookup"><span data-stu-id="d2dde-1681">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="d2dde-1682">Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute</span><span class="sxs-lookup"><span data-stu-id="d2dde-1682">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="d2dde-1683">Se agrega compatibilidad para el enrutado geográfico de TrafficManager</span><span class="sxs-lookup"><span data-stu-id="d2dde-1683">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="d2dde-1684">Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="d2dde-1684">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="d2dde-1685">Se agrega compatibilidad para directivas IPSec de conexiones VPN</span><span class="sxs-lookup"><span data-stu-id="d2dde-1685">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="d2dde-1686">Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1686">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="d2dde-1687">Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas</span><span class="sxs-lookup"><span data-stu-id="d2dde-1687">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="d2dde-1688">Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1688">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="d2dde-1689">BC: corregir errores en la salida de `vpn-connection create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1689">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="d2dde-1690">Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente</span><span class="sxs-lookup"><span data-stu-id="d2dde-1690">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="d2dde-1691">Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente</span><span class="sxs-lookup"><span data-stu-id="d2dde-1691">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="d2dde-1692">Se corrige el error por el que `traffic-manager endpoint update` no funcionaba</span><span class="sxs-lookup"><span data-stu-id="d2dde-1692">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="d2dde-1693">Se agregan los comandos en versión preliminar "network watcher"</span><span class="sxs-lookup"><span data-stu-id="d2dde-1693">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="d2dde-1694">Perfil</span><span class="sxs-lookup"><span data-stu-id="d2dde-1694">Profile</span></span>

* <span data-ttu-id="d2dde-1695">Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1695">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="d2dde-1696">Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1696">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="d2dde-1697">Redis</span><span class="sxs-lookup"><span data-stu-id="d2dde-1697">Redis</span></span>

* <span data-ttu-id="d2dde-1698">Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache</span><span class="sxs-lookup"><span data-stu-id="d2dde-1698">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="d2dde-1699">Se deja de usar el comando "update-settings"</span><span class="sxs-lookup"><span data-stu-id="d2dde-1699">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="d2dde-1700">Recurso</span><span class="sxs-lookup"><span data-stu-id="d2dde-1700">Resource</span></span>

* <span data-ttu-id="d2dde-1701">Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1701">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="d2dde-1702">Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1702">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="d2dde-1703">Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1703">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="d2dde-1704">Corregir análisis de recursos y búsqueda de versiones de API</span><span class="sxs-lookup"><span data-stu-id="d2dde-1704">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="d2dde-1705">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1705">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="d2dde-1706">Agregar documentos para actualización de az lock</span><span class="sxs-lookup"><span data-stu-id="d2dde-1706">Add docs for az lock update.</span></span> <span data-ttu-id="d2dde-1707">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1707">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="d2dde-1708">Error generado si trata de enumerar recursos de un grupo que no existe</span><span class="sxs-lookup"><span data-stu-id="d2dde-1708">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="d2dde-1709">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1709">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="d2dde-1710">[Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM</span><span class="sxs-lookup"><span data-stu-id="d2dde-1710">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="d2dde-1711">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1711">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="d2dde-1712">Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1712">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="d2dde-1713">Rol</span><span class="sxs-lookup"><span data-stu-id="d2dde-1713">Role</span></span>

* <span data-ttu-id="d2dde-1714">create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1714">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="d2dde-1715">RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1715">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="d2dde-1716">role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1716">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="d2dde-1717">create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario</span><span class="sxs-lookup"><span data-stu-id="d2dde-1717">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="d2dde-1718">SQL</span><span class="sxs-lookup"><span data-stu-id="d2dde-1718">SQL</span></span>

* <span data-ttu-id="d2dde-1719">Se agregan los comandos az sql server list-usages y az sql db list-usages</span><span class="sxs-lookup"><span data-stu-id="d2dde-1719">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="d2dde-1720">SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1720">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="d2dde-1721">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1721">Storage</span></span>

* <span data-ttu-id="d2dde-1722">Ubicación predeterminada del grupo de recursos para `storage account create`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1722">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="d2dde-1723">Agregar compatibilidad para la copia de blob incremental</span><span class="sxs-lookup"><span data-stu-id="d2dde-1723">Add support for incremental blob copy</span></span>
* <span data-ttu-id="d2dde-1724">Agregar compatibilidad para la carga grande de blobs en bloques</span><span class="sxs-lookup"><span data-stu-id="d2dde-1724">Add support for large block blob upload</span></span>
* <span data-ttu-id="d2dde-1725">Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB</span><span class="sxs-lookup"><span data-stu-id="d2dde-1725">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1726">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1726">VM</span></span>

* <span data-ttu-id="d2dde-1727">avail-set: convertir en opcional el recuento de dominios de UD&FD</span><span class="sxs-lookup"><span data-stu-id="d2dde-1727">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="d2dde-1728">nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:</span><span class="sxs-lookup"><span data-stu-id="d2dde-1728">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="d2dde-1729">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="d2dde-1729">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="d2dde-1730">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="d2dde-1730">az vm/vmss disk</span></span>
  3. <span data-ttu-id="d2dde-1731">Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar</span><span class="sxs-lookup"><span data-stu-id="d2dde-1731">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="d2dde-1732">vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH</span><span class="sxs-lookup"><span data-stu-id="d2dde-1732">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="d2dde-1733">vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1733">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="d2dde-1734">3 de abril de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1734">April 3, 2017</span></span>

<span data-ttu-id="d2dde-1735">Versión 2.0.2</span><span class="sxs-lookup"><span data-stu-id="d2dde-1735">Version 2.0.2</span></span>

<span data-ttu-id="d2dde-1736">Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión</span><span class="sxs-lookup"><span data-stu-id="d2dde-1736">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="d2dde-1737">Núcleo</span><span class="sxs-lookup"><span data-stu-id="d2dde-1737">Core</span></span>

* <span data-ttu-id="d2dde-1738">Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada</span><span class="sxs-lookup"><span data-stu-id="d2dde-1738">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="d2dde-1739">Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1739">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="d2dde-1740">Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1740">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="d2dde-1741">Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1741">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d2dde-1742">Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1742">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="d2dde-1743">Se han agregado solicitudes de parámetros de plantilla perdidos.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1743">Add prompting for missing template parameters.</span></span> <span data-ttu-id="d2dde-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1744">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="d2dde-1745">Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada</span><span class="sxs-lookup"><span data-stu-id="d2dde-1745">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="d2dde-1746">Admite el inicio de sesión en un inquilino específico</span><span class="sxs-lookup"><span data-stu-id="d2dde-1746">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="d2dde-1747">ACS</span><span class="sxs-lookup"><span data-stu-id="d2dde-1747">ACS</span></span>

* <span data-ttu-id="d2dde-1748">[ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1748">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="d2dde-1749">Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1749">Add support for ssh key password prompting.</span></span> <span data-ttu-id="d2dde-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1750">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="d2dde-1751">Se ha agregado compatibilidad con clústeres de Windows.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1751">Add support for windows clusters.</span></span> <span data-ttu-id="d2dde-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1752">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="d2dde-1753">Posibilidad de cambiar del rol Propietario al de Colaborador.</span><span class="sxs-lookup"><span data-stu-id="d2dde-1753">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="d2dde-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1754">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="d2dde-1755">AppService</span><span class="sxs-lookup"><span data-stu-id="d2dde-1755">AppService</span></span>

* <span data-ttu-id="d2dde-1756">appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1756">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="d2dde-1757">appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1757">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="d2dde-1758">appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1758">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="d2dde-1759">AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1759">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="d2dde-1760">DataLake</span><span class="sxs-lookup"><span data-stu-id="d2dde-1760">DataLake</span></span>

* <span data-ttu-id="d2dde-1761">Versión inicial del módulo de Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="d2dde-1761">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="d2dde-1762">Versión inicial del módulo de Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="d2dde-1762">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="d2dde-1763">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="d2dde-1763">DocuemntDB</span></span>

* <span data-ttu-id="d2dde-1764">DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1764">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="d2dde-1765">máquina virtual</span><span class="sxs-lookup"><span data-stu-id="d2dde-1765">VM</span></span>

* <span data-ttu-id="d2dde-1766">[Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1766">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="d2dde-1767">[VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1767">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="d2dde-1768">VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1768">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="d2dde-1769">Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1769">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="d2dde-1770">Conjunto de escalado de máquinas virtuales: admiten \* para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1770">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="d2dde-1771">Adición de secretos a máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212} (https://github.com/Azure/azure-cli/pull/2212))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1771">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="d2dde-1772">Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span><span class="sxs-lookup"><span data-stu-id="d2dde-1772">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="d2dde-1773">27 de febrero de 2017</span><span class="sxs-lookup"><span data-stu-id="d2dde-1773">February 27, 2017</span></span>

<span data-ttu-id="d2dde-1774">Versión 2.0.0</span><span class="sxs-lookup"><span data-stu-id="d2dde-1774">Version 2.0.0</span></span>

<span data-ttu-id="d2dde-1775">Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:</span><span class="sxs-lookup"><span data-stu-id="d2dde-1775">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="d2dde-1776">Container Service (acs)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1776">Container Service (acs)</span></span>
- <span data-ttu-id="d2dde-1777">Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1777">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="d2dde-1778">Redes</span><span class="sxs-lookup"><span data-stu-id="d2dde-1778">Networking</span></span>
- <span data-ttu-id="d2dde-1779">Storage</span><span class="sxs-lookup"><span data-stu-id="d2dde-1779">Storage</span></span>

<span data-ttu-id="d2dde-1780">Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1780">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="d2dde-1781">Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="d2dde-1781">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="d2dde-1782">Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando</span><span class="sxs-lookup"><span data-stu-id="d2dde-1782">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="d2dde-1783">Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro</span><span class="sxs-lookup"><span data-stu-id="d2dde-1783">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="d2dde-1784">Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="d2dde-1784">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="d2dde-1785">Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="d2dde-1785">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="d2dde-1786">Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1786">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="d2dde-1787">Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span><span class="sxs-lookup"><span data-stu-id="d2dde-1787">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="d2dde-1788">Envíe sus comentarios desde la línea de comandos con el comando `az feedback`</span><span class="sxs-lookup"><span data-stu-id="d2dde-1788">Provide feedback from the command line with the `az feedback` command</span></span>

