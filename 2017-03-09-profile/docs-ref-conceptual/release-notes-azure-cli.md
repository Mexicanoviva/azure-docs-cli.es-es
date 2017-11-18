---
title: "Notas de la versión de la CLI de Azure 2.0"
description: "Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0"
keywords: "CLI de Azure 2.0, notas de la versión"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 429b099dabd27d9356e88791f955ec52acd2a5f9
ms.sourcegitcommit: 9b36c15dc0e10024e23b8018604f5ef63c025de1
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/24/2017
---
# <a name="azure-cli-20-release-notes"></a>Notas de la versión de la CLI de Azure 2.0

## <a name="october-24-2017"></a>24 de octubre de 2017

Versión 2.0.20

### <a name="core"></a>Núcleo

* Se actualizó `2017-03-09-profile` para que utilice la versión `2016-01-01` de la API `MGMT_STORAGE`

### <a name="acr"></a>ACR

* Se actualizó la administración de recursos para que apunte a la versión `2017-10-01` de la API
* Se cambió la SKU de "Traiga su propio almacenamiento" a Clásica
* Se cambió el nombre de la SKU de registro a Basic, Standard y Premium

### <a name="acs"></a>ACS

* [Versión preliminar] Se agregaron los comandos `az aks`
* Se corrigió `get-credentials` de Kubernetes

### <a name="appservice"></a>Appservice

* Se corrigió el problema por el que los registros de `webapp` descargados pueden ser no válidos

### <a name="component"></a>Componente

* Se agregó el mensaje de desuso más claro para todos los instaladores y el mensaje de confirmación

### <a name="monitor"></a>Supervisión

* Se agregaron los comandos `action-group`.

### <a name="resource"></a>Recurso

* Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`
* Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas

### <a name="vm"></a>máquina virtual

* Se agregó el argumento `--accelerated-networking` a `vmss create`


## <a name="october-9-2017"></a>9 de octubre de 2017

Versión 2.0.19

### <a name="core"></a>Núcleo

* Se ha agregado el control de las direcciones URL de la autoridad de ADFS con una barra oblicua final para Azure Stack

### <a name="appservice"></a>Appservice

* Se ha agregado una actualización genérica con el nuevo comando `webapp update`

### <a name="batch"></a>Batch

* Se ha actualizado a la versión SDK de Batch 4.0.0
* Se ha actualizado la opción `--image` de VirtualMachineConfiguration para que sea compatible con las referencias de las imágenes de ARM y con publish:offer:sku:version
* Se ha agregado compatibilidad con el nuevo modelo de extensión de la CLI para los comandos de extensiones de Batch
* Se ha eliminado la compatibilidad con Batch del modelo de componente

### <a name="batchai"></a>Batchai

* Versión inicial del módulo de inteligencia artificial de Batch

### <a name="keyvault"></a>Keyvault

* Se ha corregido el problema de autenticación de Key Vault cuando se usa ADFS en Azure Stack. [(#4448)](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a>Red

* Se ha cambiado el argumento `--server` de `application-gateway address-pool create` para que sea opcional, lo cual permite los grupos de direcciones vacíos
* Se ha actualizado `traffic-manager` para que sea compatible con las características más recientes

### <a name="resource"></a>Recurso

* Se ha agregado a `group` compatibilidad con las opciones `--resource-group/-g` para el nombre de grupo de recurso
* Se han agregado comandos para que `account lock` funcione con los bloqueos en el nivel de suscripción
* Se han agregado comandos para que `group lock` funcione con los bloqueos en el nivel de grupo
* Se han agregado comandos para que `resource lock` funcione con los bloqueos en el nivel de recurso

### <a name="sql"></a>Sql

* Se ha agregado compatibilidad con el Cifrado de datos transparente (TDE) de SQL y TDE con Bring Your Own Key
* Se ha agregado el comando `db list-deleted` y el parámetro `db restore --deleted-time` que permiten la posibilidad de buscar y restaurar bases de datos eliminadas
* Se han agregado las opciones `db op list` y `db op cancel` que permiten la posibilidad de enumerar y cancelar operaciones en curso en la base de datos

### <a name="storage"></a>Storage

* Se ha agregado compatibilidad con instantáneas de recursos compartidos de archivos

### <a name="vm"></a>Vm

* Se ha corregido un error en `vm show` por el que al usar `-d` se producía un bloqueo en las direcciones IP privadas que faltan
* [VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con la actualización gradual a `vmss create`
* Se ha agregado compatibilidad para actualizar la configuración de cifrado con `vm encryption enable`
* Se ha agregado el parámetro `--os-disk-size-gb` a `vm create`
* Se ha agregado el parámetro `--license-type` para que Windows pueda ejecutar `vmss create`


## <a name="september-22-2017"></a>22 de septiembre de 2017

Versión 2.0.18

### <a name="resource"></a>Recurso

* Se agregó compatibilidad para mostrar las definiciones de directivas integradas
* Se agregó compatibilidad con el parámetro de modo para crear definiciones de directiva
* Se agregó compatibilidad para las plantillas y definiciones de interfaz de usuario de `managedapp definition create`
* [NUEVO CAMBIO] Se cambió el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`

### <a name="network"></a>Red

* Se agregó compatibilidad para la zona de disponibilidad a los subcomandos `network lb` y `network public-ip`
* Se agregó compatibilidad con el emparejamiento de Microsoft IPv6 para `express-route`
* Se agregaron los comandos del grupo de seguridad de aplicaciones `asg`
* Se agregó el argumento `--application-security-groups` a `nic [create|ip-config create|ip-config update]`
* Se agregaron los argumentos `--source-asgs` y `--destination-asgs` a `nsg rule [create|update]`
* Se agregaron los argumentos `--ddos-protection` y `--vm-protection` a `vnet [create|update]`
* Se agregaron los comandos `network [vnet-gateway|vpn-client|show-url]`.

### <a name="storage"></a>Storage

* Se corrigió un problema por el que los comandos `storage account network-rule` podían producir un error después de actualizar el SDK

### <a name="eventgrid"></a>Eventgrid

* Se actualizó el SDK de Python de Azure Event Grid para usar la versión más reciente de la API "2017-09-15-preview"

### <a name="sql"></a>SQL

* Se cambió el argumento `--resource-group` de `sql server list` para que sea opcional. Si no se especifica, se devolverán todos los servidores de SQL de la suscripción
* Se agregó el parámetro `--no-wait` a `db [create|copy|restore|update|replica create|create|update]` y `dw [create|update]`

### <a name="keyvault"></a>Keyvault

* Se agregó compatibilidad con comandos de Keyvault desde detrás de un servidor proxy

### <a name="vm"></a>máquina virtual

* Se agregó compatibilidad a la zona de disponibilidad para `[vm|vmss|disk] create`
* Se corrigió el problema por el que el uso de `--app-gateway ID` con `vmss create` podría provocar un error
* Se agregó el argumento `--asgs` a `vm create`
* Se agregó compatibilidad para ejecutar comandos en máquinas virtuales con `vm run-command`
* [VERSIÓN PRELIMINAR] Se agregó compatibilidad con el cifrado de disco VMSS con `vmss encryption`
* Se agregó compatibilidad para realizar el mantenimiento en máquinas virtuales con `vm perform-maintenance`

### <a name="acs"></a>ACS

* [VERSIÓN PRELIMINAR] Se agregó el argumento `--orchestrator-release` a `acs create` para las regiones de la versión preliminar de ACS

### <a name="appservice"></a>Appservice

* Se agregó capacidad para actualizar y mostrar la configuración de autenticación con `webapp auth [update|show]`

### <a name="backup"></a>Backup

* Versión preliminar


## <a name="september-11-2017"></a>11 de septiembre de 2017

Versión 2.0.17

### <a name="core"></a>Núcleo

* Se habilitó el módulo de comandos para establecer su propio identificador de correlación en telemetría.
* Se corrigió el problema de volcado de memoria JSON cuando la telemetría se establece en modo de diagnóstico.

### <a name="acs"></a>ACS

* Se agregó el comando `acs list-locations`.
* Se hizo que `ssh-key-file` vaya con el valor predeterminado esperado.

### <a name="appservice"></a>Appservice

* Se agregó la posibilidad de crear una aplicación web en un grupo de recursos que no sea el plan de servicio activo.

### <a name="cdn"></a>CDN

* Se corrigió el error 'CustomDomain is not iterable' (No se puede iterar en CustomDomain) para `cdn custom-domain create`.

### <a name="extension"></a>Extensión

* Versión inicial.

### <a name="keyvault"></a>Keyvault

* Se corrigió el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`.

### <a name="network"></a>Red

* Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.
* Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.
* Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.
* Se agregó compatibilidad para SKU a `lb create`.
* Se agregó compatibilidad para SKU a `public-ip create`.

### <a name="resource"></a>Recurso

* Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.
* Se permite pasar valores de parámetro para `policy assignment create`.
* Se permite pasar código JSON o archivo para todos los parámetros.
* Versión de API incrementada

### <a name="sql"></a>SQL

* Se agregaron los comandos `sql server vnet-rule`.

### <a name="vm"></a>máquina virtual

* Corregido: No asignar acceso a menos que se proporcione `--scope`.
* Corregido: Usar para las extensiones la misma nomenclatura que el portal.
* Se quitó `subscription` de la salida `[vm|vmss] create`.
* Corregido: La SKU de almacenamiento `[vm|vmss] create` no se aplica en los discos de datos con una imagen.
* Corregido: `vm format-secret --secrets` no aceptaba identificadores separados en distintas líneas.

## <a name="august-31-2017"></a>31 de agosto de 2017

Versión 2.0.16

### <a name="keyvault"></a>Keyvault

* Se corrigió el error que se producía al intentar resolver automáticamente la codificación del secreto con `secret download`.

### <a name="sf"></a>Sf

* Se dejan de usar todos los comandos en favor de la CLI de Service Fabric (sfctl).

### <a name="storage"></a>Storage

* Se corrigió un problema por el que no se podían crear cuentas de almacenamiento en regiones que no admitieran la característica NetworkACLs.
* Determinación del tipo de contenido y la codificación del contenido durante la carga de blobs y archivos si no se especifican ni el tipo de contenido ni la codificación del contenido.

## <a name="august-28-2017"></a>28 de agosto de 2017

Version 2.0.15

### <a name="cli"></a>CLI

* Se agregó una nota legal a `--version`.

### <a name="acs"></a>ACS

* Se corrigieron las regiones en versión preliminar.
* Se dio el formato correcto al valor de `dns_name_prefix` predeterminado.
* Se optimizó la salida del comando acs.

### <a name="appservice"></a>Appservice

* [NUEVO CAMBIO] Se corrigieron las incoherencias en la salida de `az webapp config appsettings [delete|set]`.
* Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.
* Se expuso `az webapp log show`.
* Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.
* Corregido: Las configuración de los espacios se detecta correctamente.

### <a name="iot"></a>IoT

* Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.

### <a name="network"></a>Red

* [NUEVO CAMBIO] Se cambió el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`.
* [NUEVO CAMBIO] Se cambió el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`.
* Se agregó compatibilidad con varios intervalos de direcciones IP y puertos a `nsg rule [create|update]`.
* Se agregó compatibilidad para SKU a `lb create`.
* Se agregó compatibilidad para SKU a `public-ip create`.

### <a name="profile"></a>Perfil

* Se expusieron `--msi` y `--msi-port` para iniciar sesión con la identidad de una máquina virtual.

### <a name="service-fabric"></a>Service Fabric

* Versión preliminar
* Se simplificaron las reglas de usuario y contraseña de registro para los comandos.
* Se corrigió el mensaje de petición de contraseña al usuario incluso después de pasar el parámetro.
* Se agregó compatibilidad para valores vacíos de `registry_cred`.

### <a name="storage"></a>Storage

* Se habilitó la configuración de la capa de blobs.
* Se agregaron los argumento s`--bypass` y `--default-action` a `storage account [create|update]` para admitir la tunelización del servicio.
* Se incorporaron comandos para agregar reglas de red virtual y reglas basadas en IP a `storage account network-rule`.  
* Se habilitó el cifrado del servicio por clave administrada de cliente.
* [NUEVO CAMBIO] Se cambió el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`.
* Corrección n.º 4220: `az storage account update encryption` -error de coincidencia de sintaxis

### <a name="vm"></a>máquina virtual

* Se corrigió el problema que mostraba información errónea para `vmss get-instance-view` al usar `--instance-id *`.
* Se agregó compatibilidad para `--lb-sku` a `vmss create`. 
* Se quitaron los nombres de personas de la lista de nombres de administrador no permitidos para `[vm|vmss] create`. 
* Se corrigió el problema por el que `[vm|vmss] create` producía un error si no podía extraer información del plan de una imagen.
* Se corrigió un bloqueo al crear un scaleset vmms con un equilibrador de carga interno.
* Se corrigió un problema por el que el argumento `--no-wait` no funcionaba con `vm availability-set create`.


## <a name="august-15-2017"></a>15 de agosto de 2017

Versión 2.0.14

### <a name="acs"></a>ACS

* Se corrigió el número de puerto sshMaster0 para Kubernetes

### <a name="appservice"></a>Appservice

* Se corrigió una excepción al crear un nuevo git basado en una aplicación web de Linux.

### <a name="event-grid"></a>Event Grid

* Se agregaron dependencias del SDK.

## <a name="august-11-2017"></a>11 de agosto de 2017

Versión 2.0.13

### <a name="acs"></a>ACS

* Se agregaron más regiones en versión preliminar

### <a name="batch"></a>Batch

* Se actualizó el SDK de Batch 3.1.0 y el SDK de Batch Management SDK 4.1.0.
* Se agregó un nuevo comando que muestra el número de tareas de un trabajo.
* Se corrigió un error en el procesamiento de la dirección URL SAS del archivo de recursos.
* El punto de conexión de la cuenta de Batch ahora admite el prefijo 'https://' opcional.
* Compatibilidad para agregar listas de más de 100 tareas a un trabajo.
* Se agregó un registro de depuración para cargar el módulo de comandos de extensiones.

### <a name="component"></a>Componente

* Se agregó una advertencia de comandos 'az component' en desuso.

### <a name="container"></a>Contenedor

* `create`: se corrigió el problema por el que no se permitía el signo igual en una variable de entorno.


### <a name="data-lake-store"></a>Data Lake Store

* Control de progreso habilitado.

### <a name="event-grid"></a>Event Grid

* Versión inicial.

### <a name="network"></a>Red

* `lb`: se corrigió un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.
* `application-gateway {subresource} delete`: se corrigió un problema por el que no se aplicaba `--no-wait`.
* `application-gateway http-settings update`: se corrigió un problema por el que `--connection-draining-timeout` no podía desactivarse.
* Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.

### <a name="profile"></a>Perfil

* `account list`: se agregó `--refresh` para sincronizar las suscripciones más recientes del servidor.

### <a name="storage"></a>Storage

* Se habilitó la actualización de la cuenta de almacenamiento con la identidad asignada por el sistema.

### <a name="vm"></a>máquina virtual

* `availability-set`: número de dominios de error expuesto al convertir.
* Se expuso el comando `list-skus`.
* Compatibilidad para asignar identidades sin crear asignaciones de roles.
* Aplicación de SKU de almacenamiento al conectar discos de datos.
* Se eliminó el nombre del disco de sistema operativo predeterminado y la SKU de almacenamiento al usar discos administrados.


## <a name="july-28-2017"></a>28 de julio de 2017

Versión 2.0.12

* Se agregaron comandos de contenedor.
* Se agregaron módulos de facturación y consumo.

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

### <a name="core"></a>Núcleo

* Información de autenticación de SDK de salida para entidades de servicio con certificados.
* Se corrigieron las excepciones de progreso de la implementación.
* Uso del punto de conexión de ARM desde la nube actual para crear el cliente de suscripción.
* Se mejoró el tratamiento simultáneo del archivo clouds.config (n.º 3636).
* Actualización del identificador de solicitud de cliente para cada ejecución de comando.
* Creación de clientes de suscripción con el perfil de SDK correcto (n.º 3635).
* Informes de progreso para las implementaciones de plantilla (n.º 3510).
* Se agregó compatibilidad para seleccionar campos de salida de tabla mediante consultas jmespath (n.º 3581).
* Se mejoró el silenciamiento de los argumentos de análisis y se anexó el historial con movimientos (n.º 3434).
* Creación de clientes de suscripción con el perfil de SDK correcto.
* Traslado de todos los archivos de registro existentes a la última carpeta.
* Se corrigió la idempotencia para la creación de VM/VMSS (n.º 3586).
* Las rutas de acceso de comandos ya no distinguen mayúsculas de minúsculas.
* Ciertos parámetros de tipo booleano ya no distinguen mayúsculas de minúsculas.
* Compatibilidad con inicio de sesión en ADFS en servidores locales como Azure Stack.
* Se corrigieron las escrituras simultáneas en clouds.config (n.º 3255).

### <a name="acr"></a>ACR

* Se agregó el comando `show-usage` para los registros administrados.
* Compatibilidad con la actualización de SKU para los registros administrados.
* Se agregaron registros administrados con SKU administradas.
* Se agregaron webhooks para registros administrados con el módulo de comandos acr webhook.
* Se agregó autenticación de AAD con el comando arc login.
* Se agregó el comando de eliminación para repositorios, manifiestos y etiquetas de Docker.

### <a name="acs"></a>ACS

* Compatibilidad con la versión de API 2017-07-01.

### <a name="appservice"></a>Appservice

* Se corrigió el error por el que webapp de Linux no devolvía nada.
* Compatibilidad para recuperar credenciales de acr.
* Eliminación de todos los comandos en `appservice web`.
* Enmascaramiento de contraseñas de registro de Docker en la salida del comando (n.º 3656).
* Comprobación de que el explorador predeterminado se usa en macOS sin errores (n.º 3623).
* Mejora de la ayuda de `webapp log tail` y `webapp log download` (n.º 3624).
* Se expuso el comando `traffic-routing` para configurar enrutamiento estático (n.º 3566).
* Se agregaron correcciones para aumentar la fiabilidad de la configuración del control de código fuente (n.º 3245).
* Se eliminó el argmento `--node-version` no compatible de `webapp config update` para aplicaciones web de Windows. Se usa `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...` en su lugar.

### <a name="batch"></a>Batch

* Se actualizó el SDK de Batch 3.0.0 con compatibilidad para máquinas virtuales de prioridad baja en grupos.
* Se cambió el nombre de la opción `--target-dedicated` de `pool create` a `--target-dedicated-nodes`.
* Se agregaron las opciones `--target-low-priority-nodes` y `--application-licenses` de `pool create`.

### <a name="cdn"></a>CDN

* Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe.

### <a name="cloud"></a>Nube

* Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.
* No es necesario el punto de conexión de la galería.
* Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.
* Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.
* Se expuso `endpoint_vm_image_alias_doc`.

### <a name="cosmosdb"></a>CosmosDB

* Se corrigió poder crear una colección con clave de partición personalizada.
* Se agregó compatibilidad para TTL predeterminado de colección.

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Se agregaron comandos para administración de directivas de proceso en el encabezado `dla account compute-policy`.
* Se agregó `dla job pipeline show`.
* Se agregó `dla job recurrence list`.

### <a name="data-lake-store"></a>Data Lake Store

* Se agregó compatibilidad para la rotación de claves de almacén de claves administrados por el usuario en `dls account update`.
* Se actualizó la versión subyacente del SDK del sistema de archivos de Data Lake Store para solucionar un problema de rendimiento.
* Se agregó el comando `dls enable-key-vault`. Este comando intenta habilitar un almacén de claves proporcionado por el usuario para que utilice el cifrado de datos en una cuenta de Data Lake Store.

### <a name="interactive"></a>Interactive

* Se mejoró el tiempo de inicio mediante el uso de comandos en caché.
* Mayor cobertura de las pruebas.
* Se mejoró el gesto "?" para insertar también en el siguiente comando.
* Se corrigieron los errores interactivos con el perfil 2017-03-09-profile-preview (n.º 3587).
* Se permitió `--version` como parámetro para el modo interactivo (n.º 3645).
* El modo interactivo dejó de producir errores al validar las finalizaciones (n.º 3570).
* Informes de progreso para las implementaciones de plantilla (n.º 3510).
* Se agregó la marca `--progress`.
* Se quitó `--debug` y `--verbose` de la finalización.
* Se quitó `interactive` de las finalizaciones (n.º 3324).

### <a name="iot"></a>IoT

* La creación de directivas ya no borra las directivas existentes. (n.º 3934)

### <a name="key-vault"></a>Almacén de claves

* Se agregaron comandos para características de recuperación de almacén de claves:
  * Subcomandos de `keyvault` `purge`, `recover`, `keyvault list-deleted`
  * Subcomandos de `keyvault secret` `backup`, `restore`, `purge`, `recover`, `list-deleted`
  * Subcomandos de `keyvault certificate` `purge`, `recover`, `list-deleted`
  * Subcomandos de `keyvault key` `purge`, `recover`, `list-deleted`
* Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).
* Se actualizó el plano de datos del almacén de claves a 0.3.2 (n.º 3307).

### <a name="lab"></a>Laboratorio

* Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.
* Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.

### <a name="monitor"></a>Supervisión

* Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).
* Se cambió el nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`.
* Se cambió el nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`.
* Se cambió el nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`.
* Se cambió el nombre de `monitor alert-rules` a `monitor alert`.
* Se cambió `monitor alert create`:
  * los subcomandos `condition` y `action` ya no aceptan JSON.
  * Se agregaron varios parámetros para simplificar el proceso de creación de reglas.
  * `location` ya no es necesario.
  * Se agregó compatibilidad para el nombre y el identificador de destino.
  * Se eliminó `--alert-rule-resource-name`.
  * Se cambió el nombre de `is-enabled` a `enabled`; ya no es necesario.
  * El valor predeterminado de `description` ahora se en la condición proporcionada.
  *  Se agregaron ejemplos para ayudar a aclarar el nuevo formato.
* Se admiten nombres o identificadores para los comandos `monitor metric`.
* Se agregaron argumentos y ejemplos a `monitor alert rule update` por comodidad.

### <a name="network"></a>Red

* Se agregó el comando `list-private-access-services`.
* Se agregó el argumento `--private-access-services` a `vnet subnet create` y `vnet subnet update`.
* Se corrigió el problema por el que `application-gateway redirect-config create` producía un error.
* Se corrigió el problema por el que `application-gateway redirect-config update` con `--no-wait` no funcionaba.
* Se corrigió el error al usar el argumento `--servers` con `application-gateway address-pool create` y `application-gateway address-pool update`.
* Se agregaron los comandos `application-gateway redirect-config`.
* Se agregaron comandos a `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`
* Se agregaron argumentos a `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`
* Se agregaron argumentos a `application-gateway http-settings create` y `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`
* Se agregaron argumentos a `application-gateway url-path-map create` y `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`
* Se agregó el argumento `--redirect-config` a `application-gateway url-path-map rule create`
* Se agregó compatibilidad para `--no-wait` a `application-gateway url-path-map rule delete`.
* Se agregaron argumentos a `application-gateway probe create` y `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`
* Se agregó el argumento `--redirect-config` a `application-gateway rule create` y `application-gateway rule update`.
* Se agregó compatibilidad para `--accelerated-networking` a `nic create` y `nic update`.
* Se quitó el argumento `--internal-dns-name-suffix` de `nic create`.
* Se agregó compatibilidad para `--dns-servers` a `nic update` y `nic create`: se agregó compatibilidad para --dns-servers.
* Se corrigió el error por el que `local-gateway create` pasaba por alto `--local-address-prefixes`.
* Se agregó compatibilidad para `--dns-servers` a `vnet update`.
* Se corrigió el error al crear un emparejamiento sin filtrado de rutas con `express-route peering create`.
* Se corrigió el error por el que los argumentos `--provider` y `--bandwidth` no funcionaban con `express-route update`.
* Se corrigió el error en la lógica de uso de valor predeterminado de `network watcher show-topology`.
* Se mejoró el formato de salida de `network list-usages`.
* Uso de la dirección IP de front-end predeterminada para `application-gateway http-listener create` si solo existe una.
* Uso del grupo de direcciones, la configuración de HTTP y el agente de escucha HTTP predeterminados para `application-gateway rule create` si solo existe uno.
* Uso de la dirección IP de front-end y el grupo de back-end predeterminados para `lb rule create` si solo existe uno.
* Uso de la dirección IP de front-end predeterminada para `lb inbound-nat-rule create` si solo existe una.

### <a name="profile"></a>Perfil

* Compatibilidad para el inicio de sesión desde una máquina virtual con una identidad administrada.
* Compatibilidad para la salida de `account show` en formato de archivo de autenticación del SDK.
* Se muestran advertencias acerca del desuso cuando se utiliza "--expanded-view".
* Se agregó el comando `get-access-token` para proporcionar el token AAD sin formato.
* Compatibilidad para el inicio de sesión con una cuenta de usuario sin suscripciones asociadas.

### <a name="rdbms"></a>RDBMS

* Compatibilidad para enumerar los servidores de una suscripción (n.º 3417).
* Se corrigió el problema por el que `%s` no se procesaba porque falta `% server_type` (n.º 3393).
* Se corrigió la asignación de origen de documentos y se agregó la tarea CI para comprobar (n.º 3361).
* Se corrigió la ayuda de MySQL y PostgreSQL (n.º 3369).

### <a name="resource"></a>Recurso

* Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.
* Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.
* Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.
* Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.
* Se corrigieron algunos mensajes de error y de análisis (n.º 3584).
* Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.
* Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).
* Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.

### <a name="role"></a>Rol

* Compatibilidad para la salida de `create-for-rbac` en formato de archivo de autenticación del SDK.
* Se limpiaron las asignaciones de roles y aplicación de AAD al eliminar una entidad de servicio (n.º 3610).
* Inclusión del formato de hora en las descripciones `--start-date` y `--end-date` de los argumentos de `app create`.
* Se muestran advertencias acerca del desuso cuando se utiliza `--expanded-view`.
* Se agregó integración del almacén de claves para los comandos `create-for-rbac` y `reset-credentials`.

### <a name="service-fabric"></a>Service Fabric
* Se corrigió un problema por el que los archivos grandes de aplicaciones se truncaban al cargarse (n.º 3666).
* Se agregaron pruebas para los comandos de Service Fabric (n.º 3424).
* Se corrigieron numerosos comandos de Service Fabric (n.º 3234).

### <a name="sql"></a>SQL

* Se quitó el parámetro `sql server create` `--identity` roto.
* Se quitaron los valores de contraseña de la salida de los comandos `sql server create` y `sql server update`.
* Se agregaron los comandos `sql db list-editions` y `sql elastic-pool list-editions`.

### <a name="storage"></a>Storage

* Se quitó la opción `--marker` de los comandos `storage blob list`, `storage container list` y `storage share list` (n.º 3745).
* Se habilitó la creación de una cuenta de almacenamiento solo https.
* Se actualizaron las métricas de almacenamiento, el registro y los comandos de CORS (n.º 3495).
* Se cambió la redacción del mensaje de excepción del comando add de CORS (n.º 3638) (n.º 3362).  
* El generador se convirtió en una lista en el modo dryrun del comando download-batch (n.º 3592). 
* Se corrigió el problema de dryrun del comando download-batch para blobs (n.º 3640) (n.º 3592).

### <a name="vm"></a>máquina virtual

* Compatibilidad para configurar nsg
* Se corrigió un error por el que el servidor DNS podría no estar configurado correctamente.
* Compatibilidad para identidades de servicios administrados.
* Se corrigió el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`.
* Los discos de datos que se crean con `vm image create` comienzan con lun 0


## <a name="may-10-2017"></a>10 de mayo de 2017

Versión 2.0.6

* Se cambia el nombre de DocumentDB por CosmosDB.
* Se agrega RDBMS (MySQL y Postgres).
* Se incluyen los módulos de Data Lake Analytics y Data Lake Store.
* Se incluye el módulo de Cognitive Services.
* Se incluye el módulo de Service Fabric.
* Se incluye el módulo de Interactive (se cambia el nombre de az-shell).
* Se agrega compatibilidad con los comandos de la red CDN.
* Se quita el módulo de Container.
* Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).
* Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).

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

### <a name="core"></a>Núcleo

* core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente   
* perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))
* Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))
* Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))
* Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))
* login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))
* core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))
* core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([#2605](https://github.com/Azure/azure-cli/issues/2605))
* core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([#2703](https://github.com/Azure/azure-cli/issues/2703))
* core: rendimiento mejorado
* core: personalizar certificados de CA; admitir la configuración de la variable de entorno REQUESTS_CA_BUNDLE
* core: configuración de nube; usar el punto de conexión de "administrador de recursos" si el punto de conexión de "administración" no está establecido

### <a name="acs"></a>ACS

* Corregir el número principal y de agentes para que sea un entero en lugar de una cadena
* Exponer "az acs create --no-wait" y "az acs wait" para creación asincrónica
* Exponer "az acs create --validate" para validaciones de simulacro
* Quitar perfil de Windows antes de la llamada PUT al comando de escalado ([#2755](https://github.com/Azure/azure-cli/issues/2755))

### <a name="appservice"></a>AppService

* functionapp: agregar la compatibilidad total de functionapp, incluidos crear, mostrar, enumerar, eliminar, nombre de host, SSL, etc.
* Agregar Team Services (vsts) como una opción de entrega continua a "appservice web source-control config"
* Crear "az webapp" para reemplazar "az appservice web" (para compatibilidad con versiones anteriores, "az appservice web" se mantendrá en dos versiones)
* Exponer argumentos para configurar implementaciones y "pilas en tiempo de ejecución" en creación de aplicaciones web
* Exponer "webapp list-runtimes"
* Admitir la configuración de cadenas de conexión ([#2647](https://github.com/Azure/azure-cli/issues/2647))
* Admitir el intercambio de espacios con versión preliminar
* Pulir errores de comandos de AppService ([#2948](https://github.com/Azure/azure-cli/issues/2948))
* Usar el grupo de recursos del plan de App Service para operaciones de certificados ([#2750](https://github.com/Azure/azure-cli/issues/2750))

### <a name="cosmosdb"></a>CosmosDB

* Cambiar el nombre del módulo de DocumentDB por CosmosDB
* Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos
* Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos
* Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Corregir un error cuando el filtrado de resultados y estados en listas de trabajos generaría un error
* Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete al que se accede a través de: `az dla catalog package`
* Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):

  * Tabla
  * Función con valores de tabla
  * Ver
  * Estadísticas de tabla. Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla

### <a name="data-lake-store"></a>Data Lake Store

* Actualizar la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para controlar escenarios de limitación del lado del servidor.
* Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).
* Falta ayuda para mostrar el acceso. Se va a agregar. ([#2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Buscar

* Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda

### <a name="keyvault"></a>KeyVault

* BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones
* BC: quitar --expires y --not-before del `keyvault certificate create`, ya que el servicio no admite estos parámetros
* Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy
* Corregir errores en `keyvault certificate get-default-policy` donde se exponen "expires" y "not_before", pero no "validity_in_months".
* Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Laboratorio

* Agregar los comandos crear, mostrar, eliminar y enumerar para el entorno del laboratorio
* Agregar los comandos mostrar y enumerar para ver las plantillas de ARM en el laboratorio
* Agregar la marca --environment en `az lab vm list` para filtrar máquinas virtuales en función del entorno en el laboratorio
* Agregar el comando de comodidad `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio
* Agregar comandos para administrar secretos en un laboratorio

### <a name="monitor"></a>Supervisión

* Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))
* Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Red

* Agregar comando `network watcher test-connectivity`
* Agregar compatibilidad para el parámetro `--filters` de `network watcher packet-capture create`
* Agregar la compatibilidad del drenaje de conexiones de Application Gateway
* Agregar compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway
* Agregar compatibilidad para reglas y filtros de ruta de ExpressRoute
* Agregar compatibilidad para enrutado geográfico de TrafficManager
* Agregar compatibilidad para selectores de tráfico basados en directivas de conexiones VPN
* Agregar compatibilidad para directivas IPSec de conexiones VPN
* Corregir errores con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`
* Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas
* Quitar valores NULL de la salida de los comandos `network vpn-connection list/show`
* BC: corregir errores en la salida de `vpn-connection create` 
* Corregir errores donde el argumento "--key-length" de "vpn-connection create" no se ha analizado correctamente
* Corregir errores en `dns zone import` donde los registros no se han importado correctamente
* Corregir errores donde `traffic-manager endpoint update` no ha funcionado
* Agregar los comandos de versión preliminar "network watcher"

### <a name="profile"></a>Perfil

* Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))
* Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache
* Dejar de usar el comando "update-settings"

### <a name="resource"></a>Recurso

* Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))
* Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))
* Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))
* Corregir análisis de recursos y búsqueda de versiones de API ([#2781](https://github.com/Azure/azure-cli/issues/2781))
* Agregar documentos para actualización de az lock ([#2702](https://github.com/Azure/azure-cli/issues/2702))
* Error generado si trata de enumerar recursos de un grupo que no existe ([#2769](https://github.com/Azure/azure-cli/issues/2769))
* [Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM ([#2773](https://github.com/Azure/azure-cli/issues/2773))
* Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))

### <a name="role"></a>Rol

* create-for-rbac: garantizar que la fecha final de SP no excederá la fecha de expiración del certificado ([#2989](https://github.com/Azure/azure-cli/issues/2989))
* RBAC: agregar compatibilidad total para "ad group" ([#2016](https://github.com/Azure/azure-cli/issues/2016))
* role: corregir errores en la actualización de definiciones de roles ([#2745](https://github.com/Azure/azure-cli/issues/2745))
* create-for-rbac: garantizar la selección de la contraseña proporcionada por el usuario

### <a name="sql"></a>SQL

* Agregar los comandos az sql server list-usages y az sql db list-usages
* SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Almacenamiento

* Ubicación predeterminada del grupo de recursos para `storage account create`
* Agregar compatibilidad para la copia de blob incremental
* Agregar compatibilidad para la carga grande de blobs en bloques
* Cambiar el tamaño de bloque a 100 MB cuando el archivo que se va a cargar es mayor que 200 GB

### <a name="vm"></a>máquina virtual

* avail-set: convertir en opcional el recuento de dominios de UD&FD

  nota: comandos de VM en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:
  1. az disk/snapshot/image
  2. az vm/vmss disk
  3. Dentro de "az vm/vmss create", usar "—use-unmanaged-disk" para evitar discos administrados. Otros comandos deben funcionar
* vm/vmss: mejorar el texto de advertencia cuando genera pares de claves SSH
* vm/vmss: compatibilidad con la creación a partir de una imagen de Marketplace que requiere información de planificación ([#1209](https://github.com/Azure/azure-cli/issues/1209))


## <a name="april-3-2017"></a>3 de abril de 2017

Versión 2.0.2

Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión.

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

### <a name="core"></a>Núcleo

* Se han agregado los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada.
* Inicio de sesión: omite el inquilino erróneo ([#2634](https://github.com/Azure/azure-cli/pull/2634))
* Inicio de sesión: establece la suscripción predeterminada en una con el estado "Habilitado" ([#2575](https://github.com/Azure/azure-cli/pull/2575))
* Se han agregado comandos wait y soporte --no-wait para más comandos ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Core: compatible con el inicio de sesión mediante una entidad de servicio con un certificado ([#2457](https://github.com/Azure/azure-cli/pull/2457))
* Se han agregado solicitudes de parámetros de plantilla perdidos. ([#2364](https://github.com/Azure/azure-cli/pull/2364))
* Admite valores de configuración predeterminados para argumentos comunes como el grupo de recursos predeterminado, la web predeterminada o la máquina virtual predeterminada
* Admite el inicio de sesión en un inquilino específico
 
### <a name="acs"></a>ACS

* [ACS] Adición de compatibilidad para la configuración de un clúster de ACS predeterminado ([#2554](https://github.com/Azure/azure-cli/pull/2554))
* Se ha agregado compatibilidad para la solicitud de contraseñas de claves SSH. ([#2044](https://github.com/Azure/azure-cli/pull/2044))
* Se ha agregado compatibilidad con clústeres de Windows. ([#2211](https://github.com/Azure/azure-cli/pull/2211))
* Posibilidad de cambiar del rol Propietario al de Colaborador. ([#2321](https://github.com/Azure/azure-cli/pull/2321))
 
### <a name="appservice"></a>AppService

* appservice: soporte para obtener la dirección IP externa utilizada para los registros DNS A ([#2627](https://github.com/Azure/azure-cli/pull/2627))
* appservice: admite certificados de comodín de enlace ([#2625](https://github.com/Azure/azure-cli/pull/2625))
* appservice: admite perfiles de publicación de listas ([#2504](https://github.com/Azure/azure-cli/pull/2504))
* AppService: desencadena la sincronización del control de código fuente después de la configuración ([&#2326;](https://github.com/Azure/azure-cli/pull/2326))
 
### <a name="datalake"></a>DataLake

* Versión inicial del módulo de Data Lake Analytics.
* Versión inicial del módulo de Data Lake Store.
 
### <a name="docuemntdb"></a>DocumentDB

* DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>máquina virtual

* [Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Se ha agregado el comando --secrets para máquinas virtuales y conjuntos de escalado de máquinas virtuales ([#2212} (https://github.com/Azure/azure-cli/pull/2212))
* Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27 de febrero de 2017

Versión 2.0.0

La CLI de Azure 2.0 es la primera versión con disponibilidad general.
La disponibilidad general se aplica a estos módulos de comandos:
- Container Service (acs)
- Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)
- Redes
- Almacenamiento

Estos módulos de comandos se pueden usar en producción y son compatibles con los Acuerdos de Nivel de Servicio de Microsoft.
Puede abrir problemas directamente en el soporte técnico de Microsoft o en nuestras [listas de problemas de GitHub](https://github.com/azure/azure-cli/issues/).
Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.

Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure.

Para comprobar la versión de la CLI, use `az --version`.
El resultado muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando.

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
> Algunos de los módulos de comandos tienen un postfijo "b*n*" o "rc*n*".
> Estos módulos de comandos todavía están en vista previa y tendrán disponibilidad general en el futuro.

También tenemos versiones preliminares nocturnas de la CLI.
Para más información, consulte estas instrucciones sobre [obtención de versiones preliminares nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y código de contribución](https://github.com/Azure/azure-cli#developer-setup).

Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:
- Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)
- Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).
- Envíe comentarios desde la línea de comandos con el comando `az feedback`.

