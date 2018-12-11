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
# <a name="azure-cli-release-notes"></a>Notas de la versión de la CLI de Azure
## <a name="december-4-2018"></a>4 de diciembre de 2018

Versión 2.0.52
### <a name="core"></a>Núcleo
* Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino
* Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente

### <a name="appservice"></a>Appservice
* [VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación
* Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end

### <a name="network"></a>Red
* Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF

### <a name="role"></a>Rol
* Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña 

### <a name="vm"></a>máquina virtual
* [EN DESUSO] El parámetro `vm extension [show|wait] --expand` está en desuso
* Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden
* Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH
* Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen

## <a name="november-20-2018"></a>20 de noviembre de 2018

Versión 2.0.51
### <a name="core"></a>Núcleo
* Se ha cambiado el inicio de sesión de MSI para no reutilizar el nombre de suscripción en la identidad.

### <a name="acr"></a>ACR
* Se ha agregado un token de contexto al paso de la tarea.
* Se ha agregado compatibilidad para la configuración de secretos en la ejecución de acr para reflejar la tarea de acr.
* Se ha mejorado la compatibilidad mejorada para `--top` y `--orderby` para los comandos `show-tags` y `show-manifests`.

### <a name="appservice"></a>Appservice
* Se ha cambiado el tiempo de espera predeterminado de la implementación de zip para sondear el estado a 5 minutos, agregando también una propiedad de tiempo de espera para personalizar este valor.
* Se ha actualizado el valor predeterminado `node_version`. El restablecimiento de la acción de intercambio de ranura, durante un intercambio de dos fases conserva todos los ajustes de la aplicación y las cadenas de conexión.
* Se ha quitado la comprobación de SKU de cliente para crear el plan de servicio de aplicaciones de Linux.
* Se ha corregido un error al intentar obtener el estado de zipdeploy.

### <a name="iotcentral"></a>IotCentral
* Se ha agregado la comprobación de disponibilidad de subdominios al crear una aplicación de IoT Central

### <a name="keyvault"></a>KeyVault
* Se ha corregido un error donde se han ignorado los errores.

### <a name="network"></a>Red
* Se han agregado los subcomandos `root-cert` a `application-gateway` para controlar los certificados de raíz de confianza.
* Se han agregado las opciones `--min-capacity` y `--custom-error-pages` a `application-gateway [create|update]`:
* Se ha agregado `--zones` a `application-gateway create` para compatibilidad con la zona de disponibilidad. 
* Se han agregado los argumentos `--file-upload-limit`, `--max-request-body-size` y `--request-body-check` a `application-gateway waf-config set`.

### <a name="rdbms"></a>Rdbms
* Se han agregado comandos de red virtual de mariadb.

### <a name="rbac"></a>Rbac
* Se ha corregido un problema al intentar actualizar credenciales inmutables en `ad app update`.
* Se han agregado advertencias de salida para comunicar los cambios importantes en un futuro próximo para `ad [app|sp] list`. 

### <a name="storage"></a>Storage
* Se ha mejorado el tratamiento de los casos excepcionales para los comandos de copia de almacenamiento.
* Se ha solucionado un problema con `storage blob copy start-batch` que no utilizaba las credenciales de inicio de sesión cuando las cuentas de destino y de origen eran las mismas.
* Se ha corregido un error con `storage [blob|file] url` donde `sas_token` no estaba incorporado en la dirección URL.
* Se ha agregado la advertencia de cambio importante a `[blob|container] list`: pronto se generarán los primeros 5000 resultados de manera predeterminada.

### <a name="vm"></a>máquina virtual
* Se ha agregado compatibilidad a `[vm|vmss] create --storage-sku` para especificar la SKU de la cuenta de almacenamiento para el sistema operativo administrado y los discos de datos de forma independiente.
* Se ha cambiado el nombre de los parámetros de la versión a `sig image-version` para ser `--image-version -e`.
* Ha quedado en desuso `sig image-version` argumento `--image-version-name` y se reemplazado por `--image-version`.
* Se ha agregado compatibilidad para usar el disco local del sistema operativo en `[vm|vmss] create --ephemeral-os-disk`.
* Se agregó compatibilidad para `--no-wait` a `snapshot create/update`.
* Se agregó el comando `snapshot wait`.
* Se ha agregado compatibilidad para usar el nombre de instancia con `[vm|vmss] extension set --extension-instance-name`.

## <a name="november-6-2018"></a>6 de noviembre de 2018

Versión 2.0.50

### <a name="core"></a>Núcleo
* Se ha agregado compatibilidad para la autorización sn+issuer de la entidad de servicio

### <a name="acr"></a>ACR
* Se ha agregado compatibilidad para eventos de git de solicitud de confirmación y extracción para el desencadenador de origen de la tarea
* Se ha modificado para usar el archivo Dockerfile predeterminado si no se especifica en el comando build

### <a name="acs"></a>ACS
* [CAMBIO IMPORTANTE] Se ha eliminado `enable_cloud_console_aks_browse` para habilitar "az aks browse" de forma predeterminada

### <a name="advisor"></a>Advisor
* Versión de disponibilidad general

### <a name="ams"></a>AMS
* Se han agregado nuevos grupos de comandos:
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* Se han agregado nuevos comandos:
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* Se ha agregado compatibilidad con los parámetros de cifrado a `ams streaming-policy create`
* Se ha agregado compatibilidad a `ams transform output remove` y ahora se puede realizar pasando el índice de salida a eliminar
* Se han agregado los argumentos `--correlation-data` y `--label` al grupo de comandos `ams job`
* Se han agregado los argumentos `--storage-account` y `--container` al grupo de comandos `ams asset`
* Se han agregado valores predeterminados para la hora de expiración (ahora +23 h) y los permisos (lectura) al comando `ams asset get-sas-url` 
* [CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming locator` por `ams streaming-locator`
* [CAMBIO IMPORTANTE] Se ha actualizado el argumento `--content-keys` de `ams streaming locator`
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--content-policy-name` a `--content-key-policy-name` en el comando `ams streaming locator`
* [CAMBIO IMPORTANTE] Se ha reemplazado el comando `ams streaming policy` por `ams streaming-policy`
* [CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--preset-names` por `--preset` en el grupo de comandos `ams transform`. Ahora solo puede establecer una salida o valor preestablecido cada vez (para agregar más tendrá que ejecutar `ams transform output add`). Ademas, puede pasar la ruta de acceso al código JSON personalizado para establecer un StandardEncoderPreset personalizado
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--output-asset-names ` a `--output-assets` en el comando `ams job start`. Ahora acepta una lista separada por espacios de recursos en formato "assetName=label". Se puede enviar un recurso sin etiqueta del siguiente modo: "assetName="

### <a name="appservice"></a>AppService
* Se ha corregido un error en `az webapp config backup update` que impide establecer una programación de copia de seguridad si no hay ninguna establecida

### <a name="configure"></a>Configuración
* Se ha agregado YAML a las opciones de formato de salida

### <a name="container"></a>Contenedor
* Se ha cambiado para mostrar la identidad al exportar un grupo de contenedores a YAML

### <a name="eventhub"></a>EventHub
* Se ha agregado la marca `--enable-kafka` para admitir Kafka en `eventhub namespace [create|update]`

### <a name="interactive"></a>Interactive
* Interactive ahora instala la extensión `interactive`, que permitirá actualizaciones más rápidas y soporte técnico

### <a name="monitor"></a>Supervisión
* Se ha agregado compatibilidad para los nombres de métricas que incluyen los caracteres de barra diagonal (/) y punto (.) a `--condition` en `monitor metrics alert [create|update]`

### <a name="network"></a>Red
* Entran en desuso los nombres de comando `network interface-endpoint` en favor de `network private-endpoint`
* Se ha corregido el problema por el que el argumento `--peer-circuit` de `express-route peering connection create` no aceptaba un identificador
* Se ha corregido el problema por el que `--ip-tags` no funcionaba correctamente con `public-ip create` 

### <a name="profile"></a>Perfil
* Se ha agregado `--use-cert-sn-issuer` a `az login` para el inicio de sesión de la entidad de servicio con certificados automatizados

### <a name="rdbms"></a>RDBMS
* Se han agregado los comandos de réplica de mysql

### <a name="resource"></a>Recurso
* Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`

### <a name="role"></a>Rol
* Se ha agregado compatibilidad para la administración de permisos de API, usuario de inicio de sesión, contraseña de aplicación y administración de credenciales de certificados
* Se ha cambiado `ad sp create-for-rbac` para aclarar la confusión entre el nombre para mostrar y el nombre de la entidad de servicio
* Se ha agregado compatibilidad para conceder permisos a las aplicaciones AAD

### <a name="storage"></a>Storage
* Se ha agregado compatibilidad para conectarse a los servicios de almacenamiento solo con SAS y puntos de conexión (sin un nombre de cuenta o una clave), como se describe en `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`

### <a name="vm"></a>máquina virtual
* Se ha agregado el argumento `storage-sku` a `image create` para establecer el tipo de cuenta de almacenamiento predeterminado de la imagen
* Se ha corregido el error en `vm resize` por el que la opción `--no-wait` hacía que el comando se bloquease
* Se ha cambiado el formato de salida de tabla de `vm encryption show` para mostrar el estado
* Se ha cambiado `vm secret format` para requerir la salida json/jsonc. Se advierte al usuario y se establece la salida predeterminada en JSON si se selecciona un formato de salida no deseado
* Se ha mejorado la validación de argumentos de `vm create --image`

## <a name="october-23-2018"></a>23 de octubre de 2018

Versión 2.0.49

### <a name="core"></a>Núcleo
* Se ha corregido el problema con `--ids` en el que `--subscription` tendría prioridad sobre la suscripción en `--ids`
* Se han agregado advertencias explícitas cuando se ignoran los parámetros debido al uso de `--ids`

### <a name="acr"></a>ACR
* Se ha corregido un problema de codificación de compilación de ACR en Python2

### <a name="cdn"></a>CDN
* [CAMBIO IMPORTANTE] Se ha cambiado el comportamiento del almacenamiento en caché de la cadena de consulta predeterminada de `cdn endpoint create` para que el valor predeterminado ya no sea "IgnoreQueryString". Ahora lo establece el servicio

### <a name="container"></a>Contenedor
* Se ha agregado `Private` como un tipo válido para pasar a "--ip-address"
* Se ha modificado para permitir únicamente el uso del identificador de subred para configurar una red virtual para el grupo de contenedores
* Se ha modificado para permitir el uso del nombre de red virtual o el identificador de recurso para habilitar el uso de redes virtuales de grupos de recursos distintos
* Se ha agregado `--assign-identity` para agregar una identidad de MSI a un grupo de contenedores
* Se ha agregado `--scope` para crear una asignación de roles para la identidad de MSI asignada por el sistema
* Se ha agregado una advertencia al crear un grupo de contenedores con una imagen sin un proceso de ejecución prolongada
* Se han corregido problemas en la salida de la tabla para los comandos `list` y `show`

### <a name="cosmosdb"></a>CosmosDB
* Se ha agregado compatibilidad de `--enable-multiple-write-locations` con `cosmosdb create`

### <a name="interactive"></a>Interactive
* Se ha modificado para asegurarse de que el parámetro de suscripción global aparece en los parámetros

### <a name="iot-central"></a>IoT Central
* Se han agregado opciones de plantilla y nombre para mostrar para la creación de aplicaciones de IoT Central
* [CAMBIO IMPORTANTE] Se ha eliminado la compatibilidad con la SKU F1; utilice en su lugar la SKU S1

### <a name="monitor"></a>Supervisión
* Cambios en `monitor activity-log list`:
  * Se ha agregado compatibilidad para enumerar todos los eventos en el nivel de suscripción
  * Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente
  * Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos
  * Se ha agregado `--namespace` como alias para la opción en desuso `--resource-provider`
  * Se deja en desuso `--filters` porque el servicio no admite otros valores que los que tienen opciones fuertemente tipadas
* Cambios en `monitor metrics list`:
  * Se ha agregado el parámetro `--offset` para crear consultas de tiempo más fácilmente
  * Se ha mejorado la validación en `--start-time` y `--end-time` para usar un conjunto de formatos ISO8601 más amplio y formatos de fecha y hora más sencillos
* Se ha mejorado de validación en los argumentos `--event-hub` y `--event-hub-rule` en `monitor diagnostic-settings create`

### <a name="network"></a>Red
* Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic create` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC
* Se han agregado los argumentos `--app-gateway-address-pools` y `--gateway-name` en `nic ip-config create/update` para admitir la adición de grupos de direcciones de back-end de puerta de enlace de aplicación a una NIC

### <a name="servicebus"></a>ServiceBus
* Se ha agregado la propiedad de solo lectura `migration_state` a MigrationConfigProperties para mostrar el estado actual de la migración del espacio de nombres de Service Bus Estándar a Premium

### <a name="sql"></a>SQL
* Se han corregido `sql failover-group create` y `sql failover-group update` para trabajar con la directiva de conmutación por error manual

### <a name="storage"></a>Storage
* Se ha corregido el formato de salida de `az storage cors list` para que todos los elementos muestren la clave "Service" correcta
* Se ha agregado el parámetro `--bypass-immutability-policy` para la eliminación de un contenedor bloqueado por la directiva de inmutabilidad

### <a name="vm"></a>máquina virtual
* Se exige que el modo de almacenamiento en caché de disco modo sea `None` en las máquinas de la serie Lv/Lv2 en `[vm|vmss] create`
* Se ha actualizado la lista de tamaños admitidos que admiten el acelerador de redes para `vm create`
* Se han agregado argumentos fuertemente tipados para configuraciones de ultrassd iops y mbps para `disk create`

## <a name="october-16-2018"></a>16 de octubre de 2018

Versión 2.0.48

### <a name="vm"></a>máquina virtual
* Se ha corregido el problema del SDK que provocaba errores en la instalación de Homebrew

## <a name="october-9-2018"></a>9 de octubre de 2018

Versión 2.0.47

### <a name="core"></a>Núcleo
* Ha mejorado el control de errores para los errores de "Solicitud incorrecta"

### <a name="acr"></a>ACR
* Se ha agregado compatibilidad para el formato de tablas similares como el cliente de helm

### <a name="acs"></a>ACS
* Se ha agregado `aks [create|scale] --nodepool-name` para configurar el nombre del grupo de nodos, truncado a 12 caracteres, con un valor predeterminado de: nodepool1 
* Se ha corregido para realizar la reversión a "scp" cuando se produce un error en Parimiko
* Se ha cambiado `aks create` para que no requiera `--aad-tenant-id` en adelante
* Se ha mejorado la combinación de credenciales de Kubernetes cuando hay entradas duplicadas

### <a name="container"></a>Contenedor
* Se ha cambiado `functionapp create` para permitir la creación de un tipo de plan de consumo de Linux con un runtime específico
* [VERSIÓN PRELIMINAR] Se ha agregado compatibilidad para el hospedaje de aplicaciones web en contenedores Windows

### <a name="event-hub"></a>Centro de eventos
* Se ha corregido el comando `eventhub update`
* [CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía

### <a name="extensions"></a>Extensiones
* Se ha corregido un problema al intentar agregar una extensión que ya está instalada

### <a name="hdinsight"></a>HDInsight
* Versión inicial.

### <a name="iot"></a>IoT
* Se ha agregado un comando de instalación de extensiones al banner de primera ejecución

### <a name="keyvault"></a>KeyVault
* Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente

### <a name="network"></a>Red
* Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada. Consulte el número 6052
* `--remote-vnet-id` en desuso para `network vnet peering create`
* Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador
* Se ha agregado compatibilidad con varios prefijos de subred a `network vnet create` con `--subnet-prefixes`
* Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`
* Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`
* Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`

### <a name="role"></a>Rol
* Se ha agregado compatibilidad para enumerar los propietarios de aplicaciones de Azure AD a `ad app owner`
* Se ha agregado compatibilidad para enumerar los propietarios de entidades de servicio de Azure AD a `ad sp owner`
* Se ha modificado para asegurarse de que los comandos de creación y actualización de definiciones de rol aceptan varias configuraciones de permisos
* Se ha modificado `ad sp create-for-rbac` para asegurarse de que el identificador URI de la página principal siempre es "https"

### <a name="service-bus"></a>Azure Service Bus
* [CAMBIO IMPORTANTE] Se han cambiado los comandos `list` para controlar los errores de recurso no encontrado (404) de la manera habitual en lugar de mostrar una lista vacía

### <a name="vm"></a>máquina virtual
* Se ha corregido el campo `accessSas` vacío en `disk grant-access`
* Se ha modificado `vmss create` para reservar un intervalo de puertos de front-end lo suficientemente grande como para controlar el aprovisionamiento en exceso
* Se ha corregido los comandos de actualización de `sig`
* Se ha agregado compatibilidad con `--no-wait` para la administración de versiones de imágenes en `sig`
* Se ha modificado `vm list-ip-addresses` para mostrar la zona de disponibilidad de las direcciones IP públicas
* Se ha modificado `[vm|vmss] disk attach` para establecer el LUN predeterminado del disco en la primera zona disponible

## <a name="september-21-2018"></a>21 de septiembre de 2018

Versión 2.0.46

### <a name="acr"></a>ACR
* Se han agregado comandos de tareas de ACR
* Se ha agregado un comando de ejecución rápida
* Grupo de comandos `build-task` en desuso
* Se ha agregado el grupo de comandos `helm` para poder administrar gráficos de Helm con ACR
* Se ha agregado compatibilidad para la creación idempotente de un Registro administrado
* Se ha agregado una marca sin formato para mostrar los registros de compilación

### <a name="acs"></a>ACS
* Se ha cambiado el comando `install-connector` para establecer el FQDN del maestro de AKS
* Se ha corregido el error de creación de asignación de roles para vnet-subnet-id cuando no se especificaba la entidad de servicio y skip-role-assignment

### <a name="appservice"></a>AppService

* Se ha agregado compatibilidad para la administración de operaciones de webjobs (continua y desencadenada)
* az webapp config set admite la propiedad --fts-state. También se ha agregado compatibilidad para az functionapp config set y show
* Se ha agregado compatibilidad para traer su propio almacenamiento para aplicaciones web
* Se ha agregado compatibilidad para enumerar y restaurar aplicaciones web eliminadas

### <a name="batch"></a>Batch
* Se ha cambiado la adición de tareas mediante `--json-file` para admitir la sintaxis de AddTaskCollectionParameter
* Se ha actualizado la documentación de los formatos de `--json-file` aceptados
* Se ha agregado `--max-tasks-per-node-option` a `batch pool create`
* Se ha cambiado el comportamiento de `batch account` para mostrar la cuenta que ha iniciado sesión si no se especifica ninguna opción

### <a name="batch-ai"></a>Batch AI 
* Se ha corregido el error de creación automática de la cuenta de almacenamiento en el comando `batchai cluster create`

### <a name="cognitive-services"></a>Cognitive Services
* Se ha agregado la función de autocompletar a los argumentos `--sku`, `--kind`, `--location`
* Se ha agregado el comando `cognitiveservices account list-usage`
* Se ha agregado el comando `cognitiveservices account list-kinds`
* Se ha agregado el comando `cognitiveservices account list`
* `cognitiveservices list` está en desuso.
* Se ha cambiado `--name` para que sea opcional para `cognitiveservices account list-skus`

### <a name="container"></a>Contenedor
* Se ha agregado la capacidad de reiniciar y detener un grupo de contenedores en ejecución
* Se ha agregado `--network-profile` para pasar un perfil de red
* Se han agregado `--subnet`, `--vnet_name`, para poder crear grupos de contenedores en una red virtual
* Se ha cambiado la salida de la tabla para mostrar el estado del grupo de contenedores

### <a name="datalake"></a>DataLake
* Se han agregado comandos para las reglas de red virtual

### <a name="interactive-shell"></a>Shell interactivo
* Se ha corregido el error en Windows por el que los comandos no se ejecutaban correctamente
* Se ha corregido el problema de carga de comandos en modo interactivo causado por objetos en desuso

### <a name="iot"></a>IoT
* Se ha agregado compatibilidad para el enrutamiento de centros de IoT

### <a name="key-vault"></a>Key Vault
* Se ha corregido la importación de claves de Key Vault para las claves RSA

### <a name="network"></a>Red
* Se han agregado comandos `network public-ip prefix` para admitir las características de prefijos de direcciones IP públicas
* Se han agregado comandos `network service-endpoint` para admitir las características de directiva de punto de conexión de servicio
* Se han agregado comandos `network lb outbound-rule` para admitir la creación de reglas de salida de Standard Load Balancer
* Se ha agregado `--public-ip-prefix` a `network lb frontend-ip create/update` para admitir configuraciones de IP de front-end mediante prefijos IP públicos
* Se ha agregado `--enable-tcp-reset` a `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* Se ha agregado `--disable-outbound-snat` a `network lb rule create/update`
* Se ha permitido usar `network watcher flow-log show/configure` con NSG clásicos
* Se agrega el comando `network watcher run-configuration-diagnostic`
* Se ha corregido el comando `network watcher test-connectivity` y se han agregado las propiedades `--method`, `--valid-status-codes` y `--headers`
* `network express-route create/update`: se ha agregado la marca `--allow-global-reach`
* `network vnet subnet create/update`: se ha agregado compatibilidad para `--delegation`
* Se agregó el comando `network vnet subnet list-available-delegations`.
* `network traffic-manager profile create/update`: se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` a Monitor Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`
* `network lb frontend-ip create/update`: se ha corregido la lógica para establecer el método de asignación de IP privada. Si se proporciona una dirección IP privada, la asignación será estática. Si no se proporciona ninguna dirección IP privada o se proporciona una cadena vacía, la asignación será dinámica.
* `dns record-set * create/update`: se ha agregado compatibilidad para `--target-resource`
* Se han agregado comandos `network interface-endpoint` a los objetos de punto de conexión de interfaz de consulta
* Se ha agregado `network profile show/list/delete` para la administración parcial de perfiles de red
* Se han agregado comandos `network express-route peering connection` para administrar las conexiones de emparejamiento entre instancias de ExpressRoute

### <a name="rdbms"></a>RDBMS
* Se ha agregado compatibilidad para el servicio MariaDB

### <a name="reservation"></a>Reserva
* Se ha agregado CosmosDB en el tipo de enumeración de recursos reservados
* Se ha agregado la propiedad de nombre en el modelo de revisión

### <a name="manage-app"></a>Administración de aplicaciones
* Se ha corregido el error en `managedapp create --kind MarketPlace` que provocaba un bloqueo al crear instancias de un Marketplace administrado
* Se han cambiado los comandos `feature` para que se limiten a los perfiles admitidos

### <a name="role"></a>Rol
* Se ha agregado compatibilidad para enumerar los miembros de un grupo de usuarios

### <a name="signalr"></a>SignalR
* Primera versión

### <a name="storage"></a>Storage
* Se ha agregado el parámetro `--auth-mode login` para usar las credenciales de inicio de sesión del usuario para la autorización de blobs y colas
* Se ha agregado `storage container immutability-policy/legal-hold` para administrar el almacenamiento inmutable

### <a name="vm"></a>máquina virtual
* Se ha corregido el problema por el que `vm create --generate-ssh-keys` sobrescribe el archivo de clave privada si falta el archivo de clave pública (n.º 4725 y n.º 6780)
* Se ha agregado compatibilidad para la galería de imágenes compartidas mediante `az sig`

## <a name="august-28-2018"></a>28 de agosto de 2018

Versión 2.0.45

### <a name="core"></a>Núcleo

* Se ha corregido un problema al cargar el archivo de configuración vacío
* Se ha agregado compatibilidad al perfil `2018-03-01-hybrid` de Azure Stack

### <a name="acr"></a>ACR

* Se ha agregado una solución alternativa para las operaciones en tiempo de ejecución sin solicitudes ARM
* Se ha cambiado para excluir los archivos de control de versiones (por ejemplo, .git, .gitignore) del tar cargado de manera predeterminada en el comando `build`

### <a name="acs"></a>ACS

* Se ha cambiado `aks create` a los valores predeterminados de las máquinas virtuales `Standard_DS2_v2`
* Se ha cambiado `aks get-credentials` para llamar ahora a las nuevas API para obtener las credenciales de clúster

### <a name="appservice"></a>AppService

* Se ha agregado compatibilidad con CORS en functionapp y webapp
* Se ha agregado compatibilidad con la etiqueta ARM al crear los comandos
* Se ha cambiado `[webapp|functionapp] identity show` para salir con código 3 cuando falta un recurso

### <a name="backup"></a>Copia de seguridad

* Se ha cambiado `backup vault backup-properties show` para salir con código 3 cuando falta un recurso

### <a name="bot-service"></a>Servicio de bots

* Versión inicial de la CLI del servicio de bots

### <a name="cognitive-services"></a>Cognitive Services

* Se ha agregado un nuevo parámetro `--api-properties,`, que es necesario para la creación de algunos de los servicios

### <a name="iot"></a>IoT

* Se ha corregido un problema con los centros vinculados asociados

### <a name="monitor"></a>Supervisión

* Se han agregado comandos `monitor metrics alert` para las alertas de métricas prácticamente en tiempo real
* Comandos `monitor alert` en desuso

### <a name="network"></a>Red

* Se ha cambiado `network application-gateway ssl-policy predefined show` para salir con código 3 cuando falta un recurso

### <a name="resource"></a>Recurso

* Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso

### <a name="storage"></a>Storage

* Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso

### <a name="vm"></a>máquina virtual

* Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso 
* `--storage-caching` en desuso para `vm create`

## <a name="auguest-14-2018"></a>14 de agosto de 2018

Versión 2.0.44

### <a name="core"></a>Núcleo

* Se ha corregido una presentación numérica en la salida `table`
* Se ha agregado el formato de salida de YAML

### <a name="telemetry"></a>Telemetría

* Se han mejorado los informes de telemetría

### <a name="acr"></a>ACR

* Se agregaron los comandos `content-trust policy`.
* Se ha solucionado un problema por el que `.dockerignore` no se controlaba correctamente

### <a name="acs"></a>ACS

* Se ha cambiado `az acs/aks install-cli` para instalar bajo `%USERPROFILE%\.azure-kubectl` en Windows
* Se ha cambiado `az aks install-connector` para detectar si el clúster tiene RBAC y configurar correctamente el conector ACI
* Se ha cambiado a la asignación de roles a la subred cuando se proporciona
* Se ha agregado una nueva opción a "omitir la asignación de roles" para la subred cuando se proporciona                                 
* Se ha cambiado para omitir la asignación de roles para la subred cuando la asignación ya existe                

### <a name="appservice"></a>AppService

* Se ha corregido un error que impedía crear una aplicación de función mediante cuentas de almacenamiento en grupos de recursos externos
* Se ha corregido un bloqueo en la implementación de zip

### <a name="batchai"></a>BatchAI

* Se ha cambiado la salida del registrador para la creación de una cuenta de almacenamiento automático para especificar el "*grupo* de recursos".        

### <a name="container"></a>Contenedor

* Se ha agregado `--secure-environment-variables` para pasar variables de entorno seguras en un contenedor      

### <a name="iot"></a>IoT

* [CAMBIO IMPORTANTE] Se han quitado los comandos en desuso que se han movido a la extensión iot
* Se han actualizado los elementos para que no asuman el dominio `azure-devices.net`

### <a name="iot-central"></a>Iot Central

* Versión inicial del módulo de IoT Central

### <a name="keyvault"></a>KeyVault


* Se han agregado comandos para administrar las cuentas de almacenamiento y definiciones de sas
* Se han agregado comandos para las reglas de red                                                           
* Se ha agregado el parámetro `--id` para operaciones de certificado, clave y secreto
* Se ha agregado compatibilidad para la versión de varias api de administración de KV
* Se ha agregado compatibilidad para la versión de varias api de plano de datos de KV

### <a name="relay"></a>Retransmisión

* Versión inicial.

### <a name="sql"></a>Sql

* Se agregaron los comandos `sql failover-group`.

### <a name="storage"></a>Storage

* [CAMBIO IMPORTANTE] Se ha cambiado `storage account show-usage` para requerir el parámetro `--location` y mostrará una lista por región
* Se ha cambiado el parámetro `--resource-group` para que sea opcional para los comandos `storage account`
* Se han quitado las advertencias de "Error en la condición previa' para los errores individuales en los comandos de lote para un solo mensaje agregado
* Se han cambiado los comandos `[blob|file] delete-batch` para dejar de dar salida a la matriz de nulos
* Se han cambiado los comandos `blob [download|upload|delete-batch]` para leer el token de sas de la dirección url del contenedor

### <a name="vm"></a>máquina virtual

* Se han agregado filtros comunes a `vm list-skus` para facilitar su uso

## <a name="july-31-2018"></a>31 de julio de 2018

Versión 2.0.43

### <a name="acr"></a>ACR

* Se ha agregado la marca `--with-secure-properties` al comando `acr build-task show`.
* Se agregó el comando `acr build-task update-build`.

### <a name="acs"></a>ACS

* Se ha realizado un cambio para devolver 0 (correcto) cuando `az aks browse` finaliza presionando [Ctrl + C].

### <a name="batch"></a>Batch

* Se ha corregido el error al mostrar el token de AAD en cloudshell.

### <a name="container"></a>Contenedor

* Se ha eliminado el requisito de nombre o identificador de `--log-analytics-workspace-key` al configurar la suscripción.

### <a name="network"></a>Red

* Se ha agregado compatibilidad con dns al perfil 2017-03-09-profile de Azure Stack. 

### <a name="resource"></a>Recurso

* Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.
* Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.

### <a name="role"></a>Rol

* Se ha agregado compatibilidad al perfil 2017-03-09-profile de Stack.
* Se ha corregido el problema por el que los parámetros de actualización genéricos de `app update` no funcionaban correctamente.

### <a name="search"></a>Search

* Se han agregado comandos al servicio Azure Search.

### <a name="service-bus"></a>Azure Service Bus

* S ha agregado un grupo de comandos de migración para migrar un espacio de nombres de Service Bus Estándar a Premium.
* Se han agregado nuevas propiedades opcionales a la cola y suscripción de Service Bus.
  *  `--enable-batched-operations` y `--enable-dead-lettering-on-message-expiration` en `queue`
  *  `--dead-letter-on-filter-exceptions` en `subscriptions`

### <a name="storage"></a>Storage

* Se ha agregado compatibilidad para la descarga de archivos grandes con una sola conexión.
* Se han convertido los comandos `show` que no producían un error con código de salida 3 cuando faltaba un recurso.

### <a name="vm"></a>máquina virtual

* Se ha agregado compatibilidad para enumerar los conjuntos de disponibilidad por suscripción.
* Se ha agregado compatibilidad con `StandardSSD_LRS`
* Se ha agregado compatibilidad con los grupos de seguridad de la aplicación al crear un conjunto de escalado de máquinas virtuales.
* [CAMBIO IMPORTANTE] Se ha cambiado `[vm|vmss] create`, `[vm|vmss] identity assign`, y `[vm|vmss] identity remove` para obtener las identidades asignadas por el usuario en formato de diccionario.

## <a name="july-18-2018"></a>18 de julio de 2018

Versión 2.0.42

### <a name="core"></a>Núcleo

* Se ha agregado compatibilidad con el inicio de sesión desde explorador en la ventana de bash de WSL
* Se ha agregado la marca `--force-string` a todos los comandos de actualización genéricos
* [CAMBIO IMPORTANTE] Han cambiado los comandos "show" para registrar el mensaje de error y se producirá un error con un código de salida de 3 si falta algún recurso

### <a name="acr"></a>ACR

* [CAMBIO IMPORTANTE] Se ha actualizado "--no - push" en una marca pura en el comando "acr build"
* Se han agregado los comandos `show` y `update` en el grupo `acr repository`
* Se ha agregado la marca `--detail` a `show-manifests` y `show-tags` para mostrar información más detallada
* Se ha agregado el parámetro `--image` para admitir la obtención de detalles o registros de una compilación por parte de una imagen

### <a name="acs"></a>ACS

* Ha cambiado `az aks create` a la salida de error si `--max-pods` es menor que 5

### <a name="appservice"></a>AppService

* Se ha agregado compatibilidad con las SKU de PremiumV2

### <a name="batch"></a>Batch

* Se ha corregido el error del uso del credencial de token en el modo de shell en la nube
* Se ha cambiado la entrada JSON para que no distinga mayúsculas de minúsculas

### <a name="batch-ai"></a>Batch AI

* Se ha corregido el comando `az batchai job exec`

### <a name="container"></a>Contenedor

* Se ha quitado el requisito de nombre de usuario y contraseña en los registros que no sean de dockerhub
* Se ha corregido el error que se producía al crear grupos de contenedores desde el archivo yaml

### <a name="network"></a>Red

* Se ha agregado compatibilidad de `--no-wait` con `network nic [create|update|delete]` 
* Se agregó `network nic wait`.
* El argumento `--ids` desuso `network vnet [subnet|peering] list` ha pasado a estar en desuso
* Se ha agregado la marca `--include-default` para incluir las reglas de seguridad predeterminadas en la salida de `network nsg rule list`  

### <a name="resource"></a>Recurso

* Se ha agregado compatibilidad de `--no-wait` con `group deployment delete`
* Se ha agregado compatibilidad de `--no-wait` con `deployment delete`
* Se agregó el comando `deployment wait`.
* Se ha corregido un problema de que los comandos `az deployment` del nivel de suscripción aparecían para el perfil 2017-03-09-profile

### <a name="sql"></a>SQL

* Se ha corregido el error "El nombre del grupo de recursos proporcionado ... no coincidía con el nombre de la dirección URL' al especificar el nombre del grupo elástico en los comandos `sql db copy` y `sql db replica create`
* Permite la configuración de servidor de SQL Server predeterminado mediante la ejecución de `az configure --defaults sql-server=<name>`
* Se han implementado formateadores de tabla para los comandos `sql server`, `sql server firewall-rule`, `sql list-usages` y `sql show-usage`

### <a name="storage"></a>Storage

* Se ha agregado la propiedad `pageRanges` a la salida de `storage blob show` que se rellenará en los blobs en páginas

### <a name="vm"></a>máquina virtual

* [CAMBIO IMPORTANTE] Ha cambiado `vmss create` para usar `Standard_DS1_v2` como tamaño de instancia predeterminado
* Se ha agregado compatibilidad con `--no-wait` a `vm extension [set|delete]` y `vmss extension [set|delete]`
* Se agregó `vm extension wait`.

## <a name="july-3-2018"></a>3 de julio de 2018

Versión 2.0.41

### <a name="aks"></a>AKS

* Se ha cambiado la supervisión para utilizar el identificador de suscripción

## <a name="july-3-2018"></a>3 de julio de 2018

Versión 2.0.40

### <a name="core"></a>Núcleo

* Se ha agregado un nuevo flujo de código de autorización para el inicio de sesión interactivo

### <a name="acr"></a>ACR

* Se ha agregado el estado de compilación de sondeo
* Se ha agregado compatibilidad para los valores de enumeración sin distinguir mayúsculas y minúsculas
* Se han agregado los parámetros `--top` y `--orderby` para `show-manifests`

### <a name="acs"></a>ACS

* [CAMBIO IMPORTANTE] Se ha habilitado el control de acceso basado en rol de Kubernetes de forma predeterminada.
* Se ha agregado el argumento `--disable-rbac` y `--enable-rbac` está en desuso porque ahora es el valor predeterminado
* Se han actualizado las opciones del comando `aks browse`. Se ha agregado compatibilidad con `--listen-port`
* Se ha actualizado el paquete del gráfico de helm predeterminado para el comando `aks install-connector`. Use virtual-kubelet-for-aks-latest.tgz
* Se han agregado los comandos `aks enable-addons` y `aks disable-addons` para actualizar un clúster existente

### <a name="appservice"></a>AppService

* Se ha agregado compatibilidad para deshabilitar la identidad mediante `webapp identity remove`
* Se ha quitado la etiqueta `preview` para la característica de identidad

### <a name="backup"></a>Copia de seguridad

* Se ha actualizado la definición del módulo

### <a name="batchai"></a>BatchAI

* Se ha corregido la salida de la tabla para los comandos `batchai cluster node list` y `batchai job node list`

### <a name="cloud"></a>Nube

* Se ha agregado el sufijo de servidor `acr login` a la configuración de nube

### <a name="container"></a>Contenedor

* Se ha cambiado `container create` al valor predeterminado para operaciones de larga ejecución
* Se han agregado los parámetros de Log Analytics `--log-analytics-workspace` y `--log-analytics-workspace-key`
* Se ha agregado el parámetro `--protocol` para especificar qué protocolo de red desea usar

### <a name="extension"></a>Extensión

* Se ha cambiado `extension list-available` para mostrar solo las extensiones compatibles con la versión de la CLI

### <a name="network"></a>Red

* Se ha corregido el problema por el que los tipos de registro distinguían entre mayúsculas y minúsculas ([n.º 6602](https://github.com/Azure/azure-cli/issues/6602))

### <a name="rdbms"></a>Rdbms

* Se agregaron los comandos `[postgres|myql] server vnet-rule`.

### <a name="resource"></a>Recurso

* Se ha agregado un nuevo grupo de operaciones `deployment`

### <a name="vm"></a>máquina virtual

* Se ha agregado compatibilidad para quitar la identidad asignada por el sistema

## <a name="june-25-2018"></a>25 de junio de 2018

Versión 2.0.39

### <a name="cli"></a>CLI

* Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión

## <a name="june-19-2018"></a>19 de junio de 2018

Versión 2.0.38

### <a name="core"></a>Núcleo

* Se ha agregado compatibilidad global con `--subscription` a la mayoría de los comandos

### <a name="acr"></a>ACR

* Se ha agregado `azure-storage-blob` como dependencia
* Se cambió la configuración de CPU predeterminada con `acr build-task create` para utilizar 2 núcleos

### <a name="acs"></a>ACS

* Se actualizaron las opciones del comando `aks use-dev-spaces`. Se ha agregado compatibilidad con `--update`
* Se cambió `aks get-credentials --admin` para que no reemplace el contexto de usuario en `$HOME/.kube/config`
* Se ha expuesto la propiedad `nodeResourceGroup` de solo lectura en clústeres administrados
* Se ha corregido el error del comando `acs browse`
* Se ha hecho que `--connector-name` sea opcional para `aks install-connector`, `aks upgrade-connector` y `aks remove-connector`
* Se han agregado nuevas regiones de Azure Container Instances para `aks install-connector`
* Se ha agregado la ubicación normalizada en el nombre de la versión y el nombre de nodo de Helm a `aks install-connector`

### <a name="appservice"></a>AppService

* Se ha agregado compatibilidad con las versiones más recientes de urllib
* Se ha agregado compatibilidad a `functionapp create` para que utilice el plan appservice de grupos de recursos externos

### <a name="batch"></a>Batch

* Se ha eliminado la dependencia de `azure-batch-extensions`

### <a name="batch-ai"></a>Batch AI

* Se ha agregado compatibilidad para áreas de trabajo. Las áreas de trabajo permiten agrupar clústeres, servidores de archivos y experimentos en grupos, y eliminar el límite de recursos que se pueden crear.
* Se ha agregado compatibilidad para experimentos. Los experimentos permiten agrupar los trabajos en colecciones y eliminan el límite de trabajos creados
* Se ha agregado compatibilidad para configurar `/dev/shm` para la ejecución de trabajos en un contenedor de Docker
* Se han agregado los comandos `batchai cluster node exec` y `batchai job node exec`. Estos comandos no permiten ejecutar comandos directamente en los nodos y proporcionan la funcionalidad de enrutamiento de puertos.
* Se ha agregado compatibilidad para `--ids` a los comandos `batchai`.
* [CAMBIO IMPORTANTE] Todos los clústeres y servidores de archivos deben crearse en áreas de trabajo.
* [CAMBIO IMPORTANTE] Los trabajos deben crearse en experimentos.
* [CAMBIO IMPORTANTE] Se ha eliminado `--nfs-resource-group` de los comandos `cluster create` y `job create`. Para montar un NFS que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del servidor de archivos con la opción `--nfs`.
* [CAMBIO IMPORTANTE] Se ha eliminado `--cluster-resource-group` del comando `job create`. Para enviar un trabajo para un clúster que pertenezca a un grupo de recursos o a un área de trabajo diferente, proporcione el identificador de ARM del clúster con la opción `--cluster`.
* [CAMBIO IMPORTANTE] Se ha eliminado el atributo `location` de los trabajos, clústeres y servidores de archivos. Ahora, la ubicación ahora es un atributo de un área de trabajo.
* [CAMBIO IMPORTANTE] Se ha eliminado `--location` de los comandos `job create`, `cluster create` y `file-server create`.
* [CAMBIO IMPORTANTE] Se cambiaron los nombres de las opciones cortas para que la interfaz sea más homogénea:
  - Se cambió el nombre de [`--config`, `-c`] a [`--config-file`, `-f`]
  - Se cambió el nombre de [`--cluster`, `-r`] a [`--cluster`, `-c`]
  - Se cambió el nombre de [`--cluster`, `-n`] a [`--cluster`, `-c`]
  - Se cambió el nombre de [`--job`, `-n`] a [`--job`, `-j`]

### <a name="maps"></a>Mapas

* [CAMBIO IMPORTANTE] Se cambió `maps account create` para requerir que se acepten los términos del servicio mediante un aviso interactivo o con la marca `--accept-tos`.

### <a name="network"></a>Red

* Se ha agregado compatibilidad para `https` a `network lb probe create` [n.º 6571](https://github.com/Azure/azure-cli/issues/6571)
* Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas. [n.º 6502](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a>Reservations

* [CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.
* Se ha agregado el parámetro `Location` a `reservations catalog show`.
* [CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.
* [CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.
* Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.

### <a name="role"></a>Rol

* Se ha mejorado el control de errores

### <a name="sql"></a>SQL

* Se ha corregido un error que producía confusión al ejecutar `az sql db list-editions` para una ubicación que no está disponible en su suscripción

### <a name="storage"></a>Storage

* Se ha cambiado la salida de la tabla para `storage blob download` para que sea más legible

### <a name="vm"></a>máquina virtual

* Se ha mejorado la comprobación del tamaño de máquina virtual para permitir redes aceleradas en `vm create`
* Se ha agregado la advertencia para `vmss create` que indica que se cambiará el tamaño de máquina virtual predeterminado de `Standard_D1_v2` a `Standard_DS1_v2`
* Se ha agregado `--force-update` a `[vm|vmss] extension set` para actualizar la extensión aunque la configuración no haya cambiado

## <a name="june-13-2018"></a>13 de junio de 2018

Versión 2.0.37

### <a name="core"></a>Núcleo

* Se ha mejorado la telemetría interactiva

## <a name="june-13-2018"></a>13 de junio de 2018

Versión 2.0.36

### <a name="aks"></a>AKS

* Se han agregado opciones de red avanzadas a `aks create`
* Se han agregado argumentos a `aks create` para habilitar la supervisión y el enrutamiento de HTTP
* Se agregó el argumento `--no-ssh-key` a `aks create`
* Se agregó el argumento `--enable-rbac` a `aks create`
* [VISTA PREVIA] Se agregó compatibilidad para la autenticación de Azure Active Directory a `aks create`

### <a name="appservice"></a>AppService

* Se corrigió un problema con las versiones de urllib incompatibles

## <a name="june-5-2018"></a>5 de junio de 2018

Versión 2.0.35

### <a name="interactive"></a>Interactive

* Se agregaron límites a las dependencias de modo interactivo

## <a name="june-5-2018"></a>5 de junio de 2018

Versión 2.0.34

### <a name="core"></a>Núcleo

* Se ha agregado compatibilidad para referencias a recursos entre inquilinos
* Se ha mejorado la confiabilidad de la carga de datos de telemetría

### <a name="acr"></a>ACR

* Se ha agregado compatibilidad para VSTS como ubicación de origen remoto
* Se agregó el comando `acr import`.

### <a name="aks"></a>AKS

* Se ha cambiado `aks get-credentials` para crear el archivo de configuración de Kube con permisos más seguros del sistema de archivos

### <a name="batch"></a>Batch

* Se ha corregido el error en el formato de la tabla de lista de grupos [[Problema 4378](https://github.com/Azure/azure-cli/issues/4378)]

### <a name="iot"></a>IoT

* Se ha agregado compatibilidad para crear centros de IoT de nivel básico

### <a name="network"></a>Red

* Se ha mejorado `network vnet peering`

### <a name="policy-insights"></a>Información de directiva

* Versión inicial

### <a name="arm"></a>ARM

* Se han agregado comandos `account management-group`.

### <a name="sql"></a>SQL

* Se han agregado nuevos comandos de instancia administrada:
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* Se han agregado nuevos comandos de base de datos administrada:
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a>Storage

* Se han agregado tipos de MIME adicionales para JSON y JavaScript para poder derivarlos de las extensiones de archivo

### <a name="vm"></a>máquina virtual

* Se ha cambiado `vm list-skus` para usar columnas fijas y agregar la advertencia de que `Tier` y `Size` se van a quitar
* Se agregó la opción `--accelerated-networking` a `vm create`
* Se ha agregado `--tags` a `identity create`

## <a name="may-22-2018"></a>22 de mayo de 2018

Versión 2.0.33

### <a name="core"></a>Núcleo

* Se ha agregado compatibilidad para expandir `@` en nombres de archivo

### <a name="acs"></a>ACS

* Se han agregado los nuevos comandos Dev-Spaces `aks use-dev-spaces` y `aks remove-dev-spaces`
* Se ha corregido el error tipográfico en el mensaje de ayuda

### <a name="appservice"></a>AppService

* Se han mejorado los comandos de actualización genéricos
* Se ha añadido compatibilidad con async para `webapp deployment source config-zip`

### <a name="container"></a>Contenedor

* Se ha agregado compatibilidad para exportar un grupo de contenedores al formato yaml
* Se ha agregado compatibilidad para usar un archivo yaml para crear o actualizar un grupo de contenedores

### <a name="extension"></a>Extensión

* Se ha mejorado la eliminación de extensiones

### <a name="interactive"></a>Interactive

* Se ha cambiado el registro para silenciar el analizador en las finalizaciones
* Se ha mejorado el control de los almacenamientos en caché incorrectos de la ayuda

### <a name="keyvault"></a>KeyVault

* Se han corregido los comandos de keyvault para trabajar en Cloud Shell o en máquinas virtuales con identidad

### <a name="network"></a>Red

* Se ha corregido el problema por el que `network watcher show-topology` no funcionaba con el nombre de red virtual o subred [6326](https://github.com/Azure/azure-cli/issues/6326)
* Se ha corregido el problema por el que algunos comandos `network watcher` indicaban que Network Watcher no está habilitado en regiones donde sí lo está [6264](https://github.com/Azure/azure-cli/issues/6264)

### <a name="sql"></a>SQL

* [CAMBIO IMPORTANTE] Se cambiaron los objetos de respuesta devueltos por los comandos `db` y `dw`:
    * Se ha cambiado el nombre de la propiedad `serviceLevelObjective` a `currentServiceObjectiveName`
    * Se han quitado las propiedades `currentServiceObjectiveId` y `requestedServiceObjectiveId`
    * Se ha cambiado la propiedad `maxSizeBytes` para que sea un valor entero en lugar de una cadena
* [CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `db` y `dw` siguientes para que sean de solo lectura:
    * `requestedServiceObjectiveName`.  Para actualizar, use el parámetro `--service-objective` o establezca la propiedad `sku.name`
    * `edition`. Para actualizar, use el parámetro `--edition` o establezca la propiedad `sku.tier`
    * `elasticPoolName`. Para actualizar, use el parámetro `--elastic-pool` o establezca la propiedad `elasticPoolId`
* [CAMBIO IMPORTANTE] Se han cambiado las siguientes propiedades de `elastic-pool` para que sean de solo lectura:
    * `edition`. Para actualizar, use el parámetro `--edition`
    * `dtu`. Para actualizar, use el parámetro `--capacity`
    *  `databaseDtuMin`. Para actualizar, use el parámetro `--db-min-capacity`
    *  `databaseDtuMax`. Para actualizar, use el parámetro `--db-max-capacity`
* Se han agregados los parámetros `--family` y `--capacity` a los comandos `db`, `dw` y `elastic-pool`.
* Se han agregados formateadores de tabla a los comandos `db`, `dw` y `elastic-pool`.

### <a name="storage"></a>Storage

* Se ha agregado la función de autocompletar al argumento `--account-name`
* Se ha corregido un problema con `storage entity query`

### <a name="vm"></a>máquina virtual

* [CAMBIO IMPORTANTE] Se ha eliminado `--write-accelerator` de `vm create`. Se puede obtener la misma compatibilidad mediante `vm update` o `vm disk attach`
* Se ha corregido la correspondencia de imágenes de extensión en `[vm|vmss] extension`
* Se ha agregado `--boot-diagnostics-storage` a `vm create` para capturar el registro de arranque
* Se ha agregado `--license-type` a `[vm|vmss] update`

## <a name="may-7-2018"></a>7 de mayo de 2018

Versión 2.0.32

### <a name="core"></a>Núcleo

* Se ha corregido una excepción no controlada al recuperar los secretos de una cuenta de entidad de servicio con certificado
* Se ha agregado compatibilidad limitada con argumentos posicionales
* Se ha corregido el problema en el que `--query` no se podía usar con `--ids`. [N.º 5591](https://github.com/Azure/azure-cli/issues/5591)
* Se han mejorado los escenarios de canalización desde comandos cuando se usa `--ids`. Se admite `-o tsv` con una consulta específica o `-o json` sin especificar una consulta
* Se han agregado sugerencias de comandos en caso de error si los usuarios tienen errores de escritura en los comandos
* Se han mejorado los errores cuando los usuarios escriben `az ''`
* Se ha agregado compatibilidad con tipos de recursos personalizados para las extensiones y los módulos de comandos

### <a name="acr"></a>ACR

* Se han agregado comandos ACR Build
* Se han mejorado los mensajes de error para un recurso no encontrado
* Se ha mejorado el rendimiento en la creación de recursos y el control de errores
* Se ha mejorado el inicio de sesión de acr en consolas no estándares y WSL
* Se han mejorado los mensajes de error de los comandos del repositorio
* Se han actualizado las columnas de tabla y la ordenación

### <a name="acs"></a>ACS

* Se ha agregado una advertencia que indica que `az aks` es un servicio en versión preliminar
* Se ha corregido el problema de permisos en `aks install-connector` cuando no se especifica `--aci-resource-group`

### <a name="ams"></a>AMS

* Versión inicial: administración de recursos de Azure Media Services

### <a name="appservice"></a>Appservice

* Se ha corregido un error en `webapp delete` cuando se indica `--slot`
* Se ha eliminado `--runtime-version` en `webapp auth update`
* Se ha agregado compatibilidad con min\_tls\_version y https2.0
* Se ha agregado compatibilidad con multicontenedores

### <a name="batch-ai"></a>Batch AI

* Se ha modificado `batchai create cluster` para respetar la prioridad de máquinas virtuales configurada en el archivo de configuración del clúster

### <a name="cognitive-services"></a>Cognitive Services

* Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [N.º 5603](https://github.com/Azure/azure-cli/issues/5603)

### <a name="consumption"></a>Consumo

* Se han agregado nuevos comandos a la API de presupuestos

### <a name="container"></a>Contenedor

* Se ha eliminado el requisito de `--registry-server` en `container create` cuando un servidor de registro se incluye en el nombre de imagen

### <a name="cosmos-db"></a>Cosmos DB

* Presentación de la compatibilidad con redes virtuales en la CLI de Azure: Cosmos DB

### <a name="dms"></a>DMS

* Versión inicial: se agrega compatibilidad con el escenario de migración de SQL a Azure SQL

### <a name="extension"></a>Extensión

* Se ha corregido el error en el que los metadatos de la extensión dejaban de mostrarse

### <a name="interactive"></a>Interactive

* Se permiten autocompletadores interactivos para los argumentos posicionales
* Se presenta una salida de uso sencillo cuando los usuarios escriben '\'
* Se ha corregido la finalización de parámetros sin ayuda
* Se han corregido las descripciones de los grupos de comandos

### <a name="lab"></a>Laboratorio

* Se han corregido las regresiones en la conversión de Knack

### <a name="network"></a>Red

* [CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--ids` en:
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a>Perfil

* Se ha corregido la detección de origen en `disk create`
* [CAMBIO IMPORTANTE] Se han eliminado `--msi-port` y `--identity-port` por no utilizarse
* Se ha corregido el error de escritura en el resumen breve de `account get-access-token`

### <a name="redis"></a>Redis

* Entra en desuso `redis patch-schedule patch-schedule show` en favor de `redis patch-schedule show`
* Entra en desuso `redis list-all`. Esta funcionalidad se ha situado en `redis list`
* Entra en desuso `redis import-method` en favor de `redis import`
* Se ha agregado compatibilidad con `--ids` en varios comandos

### <a name="role"></a>Rol

* [CAMBIO IMPORTANTE] Se ha eliminado `ad sp reset-credentials` por desuso

### <a name="storage"></a>Storage

* Se permite que el token de sas de destino se aplique al origen en la copia de blobs si no se especifican el sas de origen y la clave de cuenta
* Se expone --socket-timeout en la carga y descarga de blobs
* Los nombres de blob que comienzan con separadores de ruta de acceso se tratan como rutas de acceso relativas
* Se permite `storage blob copy --source-sas` con el carácter de consulta inicial "?"
* Se ha corregido `storage entity query --marker` para que acepte una lista de clave=valores

### <a name="vm"></a>máquina virtual

* Se ha corregido una lógica de detección no válida en el identificador URI de blobs no administrados
* Se ha agregado compatibilidad con el cifrado de disco sin entidades de servicio proporcionadas por el usuario
* [CAMBIO IMPORTANTE] No utilizar "ManagedIdentityExtension" de la máquina virtual para compatibilidad con MSI
* Se ha agregado compatibilidad con la directiva de expulsión para `vmss`
* [CAMBIO IMPORTANTE] Se ha eliminado `--ids` en:
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* Se ha agregado compatibilidad con el acelerador de escritura
* Se agregó `vmss perform-maintenance`.
* Se ha corregido `vm diagnostics set` para que detecte el tipo de sistema operativo de la máquina virtual de forma confiable
* Se ha cambiado `vm resize` para comprobar si el tamaño solicitado es diferente del establecido actualmente y actualizar solo en caso de cambio


## <a name="april-10-2018"></a>10 de abril de 2018

Versión 2.0.31

### <a name="acr"></a>ACR

* Control de errores mejorado de la conmutación por recuperación con wincred

### <a name="acs"></a>ACS

* Se cambió AKS, se crearon SPN para que sean válidas durante 5 años

### <a name="appservice"></a>Appservice

* [CAMBIO IMPORTANTE]: Removed `assign-identity`
* Se ha corregido la excepción no detectada de planes de webapp no existentes

### <a name="batchai"></a>BatchAI

* Se ha agregado compatibilidad con la API 2018-03-01

  - Montaje en el nivel de trabajo
  - Variables de entorno con valores de secreto
  - Configuración de contadores de rendimiento
  - Creación de informes de segmentos de ruta de acceso específicas del trabajo
  - Compatibilidad con subcarpetas en API de lista de archivos
  - Uso y los límites de informes
  - Permitir especificar el tipo de almacenamiento en caché de los servidores NFS
  - Compatibilidad con imágenes personalizadas
  - Se ha agregado compatibilidad con el kit de herramientas de pyTorch

* Se ha agregado el comando `job wait` que permite esperar a que termine el trabajo y notifica el código de salida del trabajo
* Se ha agregado el comando `usage show` para enumerar el uso actual de los recursos de Batch AI y los límites de las diferentes regiones
* Se admiten las nubes nacionales
* Se han agregado argumentos de línea de comandos al trabajo para montar sistemas de archivos en el nivel de trabajo, además de los archivos de configuración
* Se han agregado más opciones para personalizar los clústeres: prioridad de las máquinas virtuales, subred, número inicial de nodos para los clústeres de escalado automático, especificar la imagen personalizada
* Se ha agregado la opción de línea de comandos para especificar el tipo de almacenamiento en caché para NFS administrado por Batch AI
* Se ha simplificado el montaje de sistemas de archivos en los archivos de configuración. Ahora, puede omitir las credenciales para el recurso compartido de archivos de Azure y los contenedores de blobs de Azure. La CLI rellenará las credenciales que faltan con la clave de cuenta de almacenamiento proporcionada con los parámetros de línea de comandos o con la variable de entorno, o bien consultará la clave en Azure Storage (si la cuenta de almacenamiento pertenece a la suscripción actual)
* Ahora, el comando de transmisión de archivos del trabajo se completa automáticamente cuando el trabajo finaliza (realizado correctamente, realizado con errores, terminado o eliminado)
* Se mejoró la salida `table` de las operaciones `show`.
* Se agregó la opción `--use-auto-storage` para la creación de clústeres. Esta opción facilita la administración de cuentas de almacenamiento y el montaje de recursos compartidos de archivos de Azure y contenedores de blobs de Azure en clústeres
* Se agregó la opción `--generate-ssh-keys` a `cluster create` y `file-server create`
* Se agregó la posibilidad de proporcionar la tarea de configuración de nodo mediante la línea de comandos
* [CAMBIO IMPORTANTE] Los comandos `job stream-file` y `job list-files` se han trasladado al grupo `job file`
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--admin-user-name` a `--user-name` en el comando `file-server create` para que sea coherente con el comando `cluster create`

### <a name="billing"></a>Facturación

* Se han agregado comandos de inscripción de cuenta

### <a name="consumption"></a>Consumo

* Se agregaron los comandos `marketplace`.
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations summaries` a `reservation summary`
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `reservations details` a `reservation detail`
* [CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--reservation-order-id` y `--reservation-id` de los comandos `reservation`
* [CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--grain` de los comandos `reservation summary`
* [CAMBIO IMPORTANTE] Se han quitado las opciones cortas `--include-meter-details` de los comandos `pricesheet`

### <a name="container"></a>Contenedor

* Se han agregado parámetros de montaje de volúmenes del repositorio git `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` y `--gitrepo-mount-path`
* Se ha corregido el error [5926](https://github.com/Azure/azure-cli/issues/5926): Error de `az container exec` cuando se especifica --container-name

### <a name="extension"></a>Extensión

* Se ha cambiado el mensaje de comprobación de la distribución a nivel de depuración

### <a name="interactive"></a>Interactive

* Se ha cambiado para detener la finalización de los comandos no reconocidos
* Se han agregado enlaces de evento antes y después de crear el subárbol de comandos
* Se ha agregado finalización para los parámetros `--ids`

### <a name="network"></a>Red

* Se ha corregido el error [5936](https://github.com/Azure/azure-cli/issues/5936): No se pudieron establecer las etiquetas `application-gateway create`
* Se ha agregado el argumento `--auth-certs` para asociar los certificados de autenticación para `application-gateway http-settings [create|update]`. [4910](https://github.com/Azure/azure-cli/issues/4910)
* Se han agregado los comandos `ddos-protection` para crear planes de DDoS Protection
* Se ha agregado compatibilidad con `--ddos-protection-plan` a `vnet [create|update]` para asociar una red virtual a un plan de DDoS Protection
* Se ha corregido el error con la marca `--disable-bgp-route-propagation` en `network route-table [create|update]`
* Se han retirado los argumentos ficticios `--public-ip-address-type` y `--subnet-type` de `network lb [create|update]`
* Se ha agregado compatibilidad de los registros TXT con las secuencias de escape de RFC 1035 a `network dns zone [import|export]` y `network dns record-set txt add-record`

### <a name="profile"></a>Perfil

* Se ha agregado compatibilidad para las cuentas de Azure clásico en `account list`
* [CAMBIO IMPORTANTE] Se han quitado los argumentos `--msi` & `--msi-port`

### <a name="rdbms"></a>RDBMS

* Se agregó el comando `georestore`.
* Se ha elimina la restricción de tamaño de almacenamiento del comando `create`

### <a name="resource"></a>Recurso

* Se agregó compatibilidad para `--metadata` a `policy definition create`.
* Se ha agregado compatibilidad para `--metadata`, `--set`, `--add`, `--remove` a `policy definition update`

### <a name="sql"></a>SQL

* Se han agregado `sql elastic-pool op list` y `sql elastic-pool op cancel`

### <a name="storage"></a>Storage

* Se han mejorado los mensajes de error para las cadenas de conexión que tienen un formato incorrecto

### <a name="vm"></a>máquina virtual

* Se ha agregado compatibilidad para configurar el número de dominios de error de la plataforma en `vmss create`
* Se ha cambiado `vmss create` para que el valor predeterminado sea LB Estándar para conjuntos de escalado zonales, grandes o con grupos de ubicación únicos deshabilitados
* [CAMBIO IMPORTANTE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* Se ha agregado compatibilidad para la SKU de IP pública a `vm create`
* Se han agregado los argumentos `--keyvault` y `--resource-group` a `vm secret format` para admitir escenarios en los que el comando no puede resolver el identificador de almacén. [5718](https://github.com/Azure/azure-cli/issues/5718)
* Errores mejorados para `[vm|vmss create]` cuando la ubicación de un grupo de recursos no admite zonas


## <a name="march-27-2018"></a>27 de marzo de 2018

Versión 2.0.30

### <a name="core"></a>Núcleo

* Mostrar un mensaje para las extensiones marcadas como versión preliminar en la Ayuda

### <a name="acs"></a>ACS

* Se ha corregido el error de comprobación de certificado SSL para `aks install-cli` en Cloud Shell

### <a name="appservice"></a>Appservice

* Se ha agregado compatibilidad solo para HTTPS a `webapp update`
* Se ha agregado compatibilidad para espacios `az webapp identity [assign|show]` y `az functionapp identity [assign|show]`

### <a name="backup"></a>Copia de seguridad

* Se ha agregado un nuevo comando `az backup protection isenabled-for-vm`. Este comando se puede usar para comprobar si algún almacén de la suscripción está haciendo la copia de seguridad de una máquina virtual
* Se han habilitado los identificadores de objeto de Azure para los parámetros `--resource-group` y `--vault-name` para los siguientes comandos:
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
* Se han cambiado los parámetros `--name` para que acepten el formato de salida de los comandos `backup ... show`

### <a name="container"></a>Contenedor

* Se ha agregado el comando `container exec`. Ejecuta comandos en un contenedor para un grupo de contenedores de ejecución
* Permitir la salida con formato de tabla para crear y actualizar un grupo de contenedores

### <a name="extension"></a>Extensión

* Se ha agregado un mensaje para `extension add` si la extensión está en versión preliminar
* Se ha cambiado `extension list-available` para mostrar los datos completos de la extensión con `--show-details`
* [CAMBIO IMPORTANTE] Se ha cambiado `extension list-available` para mostrar los datos simplificados de la extensión de forma predeterminada

### <a name="interactive"></a>Interactive

* Se han cambiado las finalizaciones para activar tan pronto como termine la carga de la tabla de comandos
* Se ha corregido el error al usar el parámetro `--style`
* Si no existía, se creaba una instancia de lexer interactiva después de volcado de la tabla de comandos
* Compatibilidad mejorada para completer

### <a name="lab"></a>Laboratorio

* Se han corregido los errores del comando `create environment`

### <a name="monitor"></a>Supervisión

* Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)
* Se ha corregido el [problema 4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar
* Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [n.º 5785](https://github.com/Azure/azure-cli/issues/5785)

### <a name="network"></a>Red

* Se ha agregado compatibilidad para zonas DNS privadas

### <a name="profile"></a>Perfil

* Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`

### <a name="rdbms"></a>RDBMS

* Se ha agregado el modelo de negocio GA API versión 2017-12-01

### <a name="resource"></a>Recurso

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a>Rol

* Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`
* Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto
* Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`
* [CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`
* Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`

### <a name="storage"></a>Storage

* Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB
* Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): las cargas de blobs de anexión ignoraban los parámetros de condición

### <a name="vm"></a>máquina virtual

* Se ha agregado una advertencia a `vmss create` de próximos cambios importantes para conjuntos con más de 100 instancias
* Se ha agregado compatibilidad con zonas resistentes a `vm [snapshot|image]`
* Se ha cambiado la vista de instancia de disco para que informe mejor del estado de cifrado
* [CAMBIO IMPORTANTE] Se ha cambiado `vm extension delete` para que ya no devuelva una salida

## <a name="march-13-2018"></a>13 de marzo de 2018

Versión 2.0.29

### <a name="acr"></a>ACR

* Se ha agregado compatibilidad con el parámetro `--image` a `repository delete`.
* Los parámetros `--manifest` y `--tag` del comando `repository delete` están en desuso.
* Se ha agregado el comando `repository untag` para quitar una etiqueta sin eliminar los datos.

### <a name="acs"></a>ACS

* Se ha agregado el comando `aks upgrade-connector` para actualizar un conector existente.
* Se han cambiado los archivos de configuración `kubectl` para usar código YAML con un estilo de bloque más legible.

### <a name="advisor"></a>Advisor

* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration get` a `advisor configuration list`
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `advisor configuration set` a `advisor configuration update`
* [CAMBIO IMPORTANTE] Se quitó `advisor recommendation generate`
* Se ha agregado el parámetro `--refresh` a `advisor recommendation list`
* Se agregó el comando `advisor recommendation show`.

### <a name="appservice"></a>Appservice

* `[webapp|functionapp] assign-identity` está en desuso.
* Se han agregado los comandos de identidad administrada `webapp identity [assign|show]` y `functionapp identity [assign|show]`.

### <a name="eventhubs"></a>Event Hubs

* Versión inicial.

### <a name="extension"></a>Extensión

* Se ha agregado una comprobación para advertir al usuario si usa una distribución diferente de la que está almacenada en el archivo de origen del paquete, porque podría provocar errores.

### <a name="interactive"></a>Interactive

* Se ha corregido el problema [5625](https://github.com/Azure/azure-cli/issues/5625): el historial se conserva entre sesiones diferentes.
* Se ha corregido el problema [3016](https://github.com/Azure/azure-cli/issues/3016): el historial no se registra mientras está en el ámbito.
* Se ha corregido el problema [5688](https://github.com/Azure/azure-cli/issues/5688): las finalizaciones no aparecen si el comando de carga de tabla detecta una excepción.
* Se ha corregido el indicador de progreso durante operaciones de ejecución prolongada.

### <a name="monitor"></a>Supervisión

* Los comandos `monitor autoscale-settings` están en desuso.
* Se agregaron los comandos `monitor autoscale`.
* Se agregaron los comandos `monitor autoscale profile`.
* Se agregaron los comandos `monitor autoscale rule`.

### <a name="network"></a>Red

* [CAMBIO IMPORTANTE] Se quitó el parámetro `--tags` de `route-filter rule create`
* Se han quitado algunos valores erróneos predeterminado de los siguientes comandos:
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* Se han agregado comandos `network watcher connection-monitor`.
* Se han agregado los parámetros `--vnet` y `--subnet` a `network watcher show-topology`.

### <a name="profile"></a>Perfil

* El parámetro `--msi` de `az login` está en desuso.
* Se ha agregado el parámetro `--identity` a `az login` para reemplazar a `--msi`.

### <a name="rdbms"></a>RDBMS

* [VERSIÓN PRELIMINAR] Se ha cambiado para usar la API 2017-12-01-preview

### <a name="service-bus"></a>Azure Service Bus

* Versión inicial.

### <a name="storage"></a>Storage

* Se ha corregido el problema [4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` ahora admite otras nubes de Azure.
* Se ha corregido el problema [5286](https://github.com/Azure/azure-cli/issues/5286): los comandos `storage blob [delete-batch|download-batch|upload-batch]` de Batch ya no producen errores después de errores de condición previa.

### <a name="vm"></a>máquina virtual

* Se agregó compatibilidad para `[vm|vmss] create` para conectar los discos de datos no administrados y configurar el almacenamiento en caché.
* `[vm|vmss] assign-identity` y `[vm|vmss] remove-identity` están en desuso.
* Se han agregado los comandos `vm identity [assign|remove|show]` y `vmss identity [assign|remove|show]` para reemplazar los comandos en desuso.
* Se ha cambiado la prioridad predeterminada en `vmss create` a None.

## <a name="february-27-2018"></a>27 de febrero de 2018

Versión 2.0.28

### <a name="core"></a>Núcleo

* Se ha corregido [#5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew
* Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas
* Se ha agregado el registro de HTTP a `--debug`

### <a name="acs"></a>ACS

* Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada
* Problema corregido: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI
* Se han agregados los parámetros `--aci-container-group`, `--location` y `--image-tag` a `aks install-connector`
* Se ha eliminado el aviso de desuso de `aks get-versions`

### <a name="appservice"></a>Appservice

* Actualizaciones de la nueva versión del SDK (azure-mgmt-web 0.35.0)
* Se ha corregido [#5538](https://github.com/Azure/azure-cli/issues/5538): se notificaba `Free` como SKU no válida

### <a name="cognitive-services"></a>Cognitive Services

* Se ha actualizado el "aviso" cuando se crea una nueva cuenta de Cognitive Services

### <a name="consumption"></a>Consumo

* Se han agregado nuevos comandos a la API PriceSheet
* Se han actualizados los formatos existentes para Detalles de uso y Detalles de la reserva

### <a name="container"></a>Contenedor

* Se han agregado los argumentos `--secrets` y `--secrets-mount-path` a `container create` para usar secretos en ACI

### <a name="network"></a>Red

* Se ha corregido [#5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`

### <a name="resource"></a>Recurso

* Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error

### <a name="role"></a>Rol

* Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio

### <a name="sql"></a>SQL

* Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización

### <a name="storage"></a>Storage

* Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`

### <a name="vm"></a>máquina virtual

* Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS


## <a name="february-13-2018"></a>13 de febrero de 2018

Versión 2.0.27

### <a name="core"></a>Núcleo

* Se ha cambiado la autenticación a clave en el inicio de sesión de MSI, tanto en el identificador de suscripción como en el nombre

### <a name="acs"></a>ACS

* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `aks get-versions` a `aks get-upgrades` para mayor precisión
* Se ha cambiado `aks get-versions` para mostrar las versiones disponibles de Kubernetes para `aks create`
* Se han cambiado los valores predeterminados de `aks create` para permitir que el servidor elija la versión de Kubernetes
* Se han actualizado los mensajes de ayuda que hacen referencia a la entidad de servicio generada por AKS
* Se han cambiado los tamaños de nodo predeterminados para `aks create` de "Standard\_D1\_v2" a "Standard\_DS1\_v2"
* Se ha mejorado la confiabilidad al localizar el pod del panel en `az aks browse`
* Se ha corregido `aks get-credentials` para controlar los errores de Unicode al cargar archivos de configuración de Kubernetes
* Se ha agregado un mensaje a `az aks install-cli` para ayudar a obtener `kubectl` en `$PATH`

### <a name="appservice"></a>Appservice

* Se ha corregido un problema por el que `webapp [backup|restore]` producía un error debido a una referencia nula
* Se ha agregado compatibilidad con los planes de App Service predeterminados mediante `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a>CDN

* Se agregaron los comandos `cdn custom-domain [enable-https|disable-https]`.

### <a name="container"></a>Contenedor

* Se ha agregado la opción `--follow` a `az container logs` para la transmisión por streaming de los registros
* Se ha agregado el comando `container attach`, que conecta los flujos de salida y de error estándar locales a un contenedor en un grupo de contenedores

### <a name="cosmosdb"></a>CosmosDB

* Se ha agregado compatibilidad para la configuración de funcionalidades

### <a name="extension"></a>Extensión

* Se ha agregado compatibilidad con el parámetro `--pip-proxy` a los comandos `az extension [add|update]`
* Se ha agregado compatibilidad con el argumento `--pip-extra-index-urls` a los comandos `az extension [add|update]`

### <a name="feedback"></a>Comentarios

* Se ha agregado información de la extensión a los datos de telemetría

### <a name="interactive"></a>Interactive

* Se ha corregido un problema por el que se solicita al usuario que inicie sesión cuando se usa el modo interactivo en Cloud Shell
* Se ha corregido la regresión con el completado de los parámetros que faltan

### <a name="iot"></a>IoT

* Se ha corregido un problema por el que `iot dps access policy [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.
* Se ha corregido un problema por el que `iot dps linked-hub [create|update]` devolvía un error "no encontrado" en ejecuciones correctas.
* Se ha agregado compatibilidad con `--no-wait` a `iot dps access policy [create|update]` y `iot dps linked-hub [create|update]`
* Se ha cambiado `iot hub create` para permitir especificar el número de particiones

### <a name="monitor"></a>Supervisión

* Se ha corregido el comando `az monitor log-profiles create`

### <a name="network"></a>Red

* Se ha corregido la opción `--tags` en los siguientes comandos:
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a>Perfil

* Se ha habilitado `az login` en el modo interactivo

### <a name="resource"></a>Recurso

* Se ha agregado de nuevo `feature show`

### <a name="role"></a>Rol

* Se agregó el argumento `--available-to-other-tenants` a `ad app update`

### <a name="sql"></a>SQL

* Se agregaron los comandos `sql server dns-alias`.
* Se agregó `sql db rename`.
* Se ha agregado compatibilidad con el argumento `--ids` a todos los comandos sql

### <a name="storage"></a>Storage

* Se han agregado los comandos `storage blob service-properties delete-policy` y `storage blob undelete` para habilitar la eliminación temporal

### <a name="vm"></a>máquina virtual

* Se ha corregido un bloqueo cuando el cifrado de la máquina virtual no estaba totalmente inicializado
* Se ha agregado la salida del identificador de la entidad de seguridad al habilitar MSI
* `vm boot-diagnostics get-boot-log` fija


## <a name="january-31-2018"></a>31 de enero de 2018

Versión 2.0.26

### <a name="core"></a>Núcleo

* Se ha agregado compatibilidad con la recuperación de token sin formato en el contexto de MSI
* Se ha eliminado la cadena de indicador de sondeo después de finalizar LRO en cmd.exe de Windows
* Se ha agregado una advertencia que aparece cuando se usa un valor predeterminado configurado se ha cambiado a una entrada en el nivel de información. Use `--verbose` para verlo
* Se ha agregado un indicador de progreso para los comandos de espera

### <a name="acs"></a>ACS

* Se ha aclarado el argumento `--disable-browser`
* Se ha mejorado el completado con tabulación para los argumentos `--vm-size`

### <a name="appservice"></a>Appservice

* `webapp log [tail|download]` fija
* Se ha eliminado la comprobación `kind` en aplicaciones web y funciones

### <a name="cdn"></a>CDN

* Se ha corregido un problema de cliente no encontrado en `cdn custom-domain create`

### <a name="cosmosdb"></a>CosmosDB

* Se ha corregido la descripción de parámetros en las directivas de conmutación por error

### <a name="interactive"></a>Interactive

* Se ha corregido un problema por el que no aparecía el completado de las opciones del comando

### <a name="network"></a>Red

* Se ha agregado protección para `--cert-password` en `application-gateway create`
* Se ha corregido un problema con `application-gateway update` en el que `--sku` aplicaba de un modo erróneo un valor predeterminado
* Se ha agregado protección para `--shared-key` y `--authorization-key` en `vpn-connection create`
* Se ha corregido un problema de cliente no encontrado en `asg create`
* Se ha agregado el parámetro `--file-name / -f` a los nombres exportados en `dns zone export`
* Se han corregido los problemas siguientes en `dns zone export`:
  * Se ha corregido un problema por el que se exportaban incorrectamente los registros TXT largos
  * Se ha corregido un problema por el que los registros TXT entre comillas se exportaban incorrectamente sin comillas de escape
* Se ha corregido un problema por el que algunos registros se importaban dos veces en `dns zone import`
* Se han restaurado los comandos `vnet-gateway root-cert` y `vnet-gateway revoked-cert`

### <a name="profile"></a>Perfil

* Se ha corregido `get-access-token` para funcionar en un máquina virtual con identidad

### <a name="resource"></a>Recurso

* Se ha corregido un error en `deployment [create|validate]` por el que aparecía incorrectamente una advertencia cuando un campo "type" de la plantilla contenía valores en mayúsculas

### <a name="storage"></a>Storage

* Se ha corregido un problema en la migración de cuentas de Storage V1 a Storage V2
* Se ha agregado un informe de progreso a todos los comandos de carga y descarga
* Se ha corregido un error en la opción "-n" en `storage account check-name`
* Se ha agregado la columna "snapshot" a la salida de tabla de `blob [list|show]`
* Se han corregido errores en varios parámetros que debían analizarse como enteros

### <a name="vm"></a>máquina virtual

* Se ha agregado el comando `vm image accept-terms` para permitir la creación de máquinas virtuales desde imágenes con cargos adicionales
* Se ha corregido `[vm|vmss create]` para asegurarse de que se pueden ejecutar comandos en un proxy con certificados sin firmar
* [VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con "baja" prioridad a los conjuntos de escalado de máquinas virtuales
* Se ha agregado protección para `--admin-password` en `[vm|vmss] create`


## <a name="january-17-2018"></a>17 de enero de 2018

Versión 2.0.25

### <a name="acr"></a>ACR

* Se ha agregado el inicio de sesión de acr de reserva en los errores de credenciales de Windows
* Se han habilitado los registros del registro

### <a name="acs"></a>ACS

* Se ha corregido el comando `get-credentials`
* Se ha eliminado el requisito de rol SPN

### <a name="appservice"></a>Appservice

* Se ha corregido el error en `config ssl upload` cuando `hosting_environment_profile` era NULL
* Se ha agregado compatibilidad con direcciones URL personalizadas para `browse`
* Se ha corregido la compatibilidad con ranuras en `log tail`

### <a name="backup"></a>Copia de seguridad

* Se ha cambiado la opción `--container-name` de `backup item list` para que sea opcional
* Se han agregado opciones de la cuenta de almacenamiento a `backup restore restore-disks`
* Se ha corregido la comprobación de ubicación en `backup protection enable-for-vm` para que no distinga entre mayúsculas y minúsculas
* Se ha corregido un problema que se daba cuando los comandos producían un error con un nombre de contenedor no válido
* Se ha cambiado `backup item list` para incluir el "Estado de mantenimiento" de forma predeterminada

### <a name="batch"></a>Batch

* Se ha cambiado `batch login` para devolver los detalles de la autenticación

### <a name="cloud"></a>Nube

* Se ha modificado para que no se necesiten los puntos de conexión al establecer `--profile` en una nube

### <a name="consumption"></a>Consumo

* Se han agregado nuevos comandos para las reservas: `consumption reservations summaries` y `consumption reservations details`

### <a name="event-grid"></a>Event Grid

* [CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid topic event-subscription` a `eventgrid event-subscription`
* [CAMBIO IMPORTANTE] Se han movido los comandos `az eventgrid resource event-subscription` a `eventgrid event-subscription`
* [CAMBIO IMPORTANTE] Se ha eliminado el comando `eventgrid event-subscription show-endpoint-url`. Use `eventgrid event-subscription show --include-full-endpoint-url` en su lugar
* Se ha agregado el comando `eventgrid topic update`
* Se ha agregado el comando `eventgrid event-subscription update`
* Se ha agregado el parámetro `--ids` a los comandos `eventgrid topic`
* Se ha agregado compatibilidad con la función de autocompletar para los nombres de tema

### <a name="interactive"></a>Interactive

* Se ha corregido un problema en el que el modo interactivo no funcionaba con Python 2.x
* Se han corregido errores en el inicio
* Se ha corregido un problema con algunos comandos que no se ejecutaban en modo interactivo

### <a name="iot"></a>IoT

* Se ha agregado compatibilidad con el servicio de aprovisionamiento de dispositivos
* Se han agregado mensajes de obsolescencia en comandos y la ayuda de comandos
* Se ha agregado la comprobación de IoT para informar a los usuarios de la extensión de IoT

### <a name="monitor"></a>Supervisión

* Se ha agregado compatibilidad con la configuración de múltiples diagnósticos. El parámetro `--name` ahora es obligatorio en `az monitor diagnostic-settings create`
* Se ha agregado el comando `monitor diagnostic-settings categories` para obtener la categoría de configuración de diagnósticos

### <a name="network"></a>Red

* Se ha corregido un problema que se producía al intentar cambiar entre el modo activo y el modo en espera con `vnet-gateway update`
* Se ha agregado compatibilidad con HTTP2 a `application-gateway [create|update]`

### <a name="profile"></a>Perfil

* Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario

### <a name="role"></a>Rol

* Se ha agregado el argumento `--assignee-object-id` a `role assignment create` para omitir la consulta de Graph

### <a name="service-fabric"></a>Service Fabric

* Se han agregado errores detallados a la respuesta de la validación en la creación del clúster
* Se ha corregido un problema de cliente no encontrado en varios comandos

### <a name="vm"></a>máquina virtual

* [VERSIÓN PRELIMINAR] Compatibilidad entre zonas para `vmss`
* [CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `vmss` de zona única al equilibrador de carga "Estándar"
* [CAMBIO IMPORTANTE] Se ha cambiado `externalIdentities` a `userAssignedIdentities` para EMSI
* [VERSIÓN PRELIMINAR] Se ha agregado compatibilidad con el intercambio de discos de sistema operativo
* Se ha agregado compatibilidad con el uso de imágenes de máquina virtual de otras suscripciones
* Se han agregado los argumentos `--plan-name`, `--plan-product`, `--plan-promotion-code` y `--plan-publisher` a `[vm|vmss] create`
* Se han corregido problemas de error en `[vm|vmss] create`
* Se ha corregido el uso excesivo de recursos producido por `vm image list --all`

## <a name="december-19-2017"></a>19 de diciembre de 2017

Versión 2.0.23

* Se ha agregado compatibilidad con el inicio de sesión con identidades asignadas por el usuario

### <a name="container"></a>Contenedor

* Se corrigió el orden incorrecto de los parámetros en los registros del contenedor

### <a name="network"></a>Red

* Se agregó el argumento `--disable-bgp-route-propagation` a `route-table [create|update]`
* Se agregó el argumento `--ip-tags` a `public-ip [create|update]`

### <a name="storage"></a>Storage

* Se agregó compatibilidad con almacenamiento V2

### <a name="vm"></a>máquina virtual

* [Versión preliminar] Se agregó compatibilidad para identidades asignadas por el usuario para máquinas virtuales y conjuntos de escalado de máquinas virtuales


## <a name="december-5-2017"></a>5 de diciembre de 2017

Versión 2.0.22

* Se quitaron los comandos `az component`. Use `az extension` en su lugar

### <a name="core"></a>Núcleo
* Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us
* Se corrigió el problema por el que se podía enviar datos de telemetría continuamente

### <a name="acs"></a>ACS

* Se agregaron los comandos `aks install-connector` y `aks remove-connector`
* Se mejoraron los informes de errores de `acs create`
* Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa

### <a name="advisor"></a>Advisor

* Versión inicial.

### <a name="appservice"></a>Appservice

* Se corrigió la generación de nombres de certificado con `webapp config ssl upload`
* Se corrigió `webapp [list|show]` y `functionapp [list|show]` para mostrar las aplicaciones correctas
* Se agregó el valor predeterminado para `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a>Consumo

* Se agregó compatibilidad con la versión de API 2017-11-30

### <a name="container"></a>Contenedor

* Se corrigió la regresión de puertos predeterminados

### <a name="monitor"></a>Supervisión

* Se agregó compatibilidad multidimensional al comando metrics

### <a name="resource"></a>Recurso

* Se agregó el argumento `--include-response-body` a `resource show`

### <a name="role"></a>Rol

* Se agregó la presentación de las asignaciones predeterminadas de los administradores "clásicos" a `role assignment list`
* Se agregó compatibilidad a `ad sp reset-credentials` para agregar las credenciales en lugar de sobrescribir
* Se mejoraron los informes de errores de `ad sp create-for-rbac`

### <a name="sql"></a>SQL

* Se agregaron los comandos `sql db list-usages` y `sql db show-usage`
* Se agregaron los comandos `sql server conn-policy show` y `sql server conn-policy update`

### <a name="vm"></a>máquina virtual

* Se agregó información de zona a `az vm list-skus`


## <a name="november-14-2017"></a>14 de noviembre de 2017

Versión 2.0.21

### <a name="acr"></a>ACR

* Se agregó compatibilidad para crear webhooks en regiones de replicación


### <a name="acs"></a>ACS

* Se cambió el texto de "agente" a "nodo" en AKS
* Opción `--orchestrator-release` en desuso para `acs create`
* Se cambió el tamaño de máquina virtual predeterminado para AKS a `Standard_D1_v2`
* Se corrigió `az aks browse` en Windows
* Se corrigió `az aks get-credentials` en Windows

### <a name="appservice"></a>Appservice

* Se agregó el origen de implementación `config-zip` para aplicaciones móviles y aplicaciones de función
* Se agregó la opción `--docker-container-logging` a `az webapp log config`
* Se quitó la opción `storage` del parámetro `--web-server-logging` de `az webapp log config`
* Se mejoraron los mensajes de error de `deployment user set`
* Se agregó compatibilidad para crear aplicaciones de función Linux
* `list-locations` fija

### <a name="batch"></a>Batch

* Se corrigió el error en el comando de creación de grupos cuando se usaba un identificador de recurso con la marca `--image`

### <a name="batchai"></a>Batchai

* Se agregó la opción corta `-s` para `--vm-size` al proporcionar el tamaño de la máquina virtual en el comando `file-server create`
* Se agregó el nombre de la cuenta de almacenamiento y los argumentos de la clave a los parámetros de `cluster create`
* Se corrigió la documentación de `job list-files` y `job stream-file`
* Se agregó la opción corta `-r` para `--cluster-name` al proporcionar el nombre de clúster en el comando `job create`

### <a name="cloud"></a>Nube

* Se cambió `cloud [register|update]` para impedir el registro de nubes que no tienen los puntos de conexión necesarios

### <a name="container"></a>Contenedor

* Se agregó compatibilidad para abrir varios puertos
* Se agregó la directiva de reinicio de grupo de contenedores
* Se agregó compatibilidad para montar un recurso compartido de Azure File como un volumen
* Se actualizaron los documentos auxiliares

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Se cambió `[job|account] list` para devolver información más concisa

### <a name="data-lake-store"></a>Data Lake Store

* Se cambió `account list` para devolver información más concisa

### <a name="extension"></a>Extensión

* Se agregó `extension list-available` para permitir que se muestre extensiones oficiales de Microsoft
* Se agregó `--name` a `extension [add|update]` para permitir la instalación de extensiones por nombre

### <a name="iot"></a>IoT

* Se agregó compatibilidad para entidades de certificación (CA) y cadenas de certificados

### <a name="monitor"></a>Supervisión

* Se agregaron los comandos `activity-log alert`.

### <a name="network"></a>Red

* Se agregó compatibilidad para los registros DNS CAA
* Se corrigió un problema por el que los puntos de conexión no se podían actualizar con `traffic-manager profile update`
* Se corrigió un problema por el que `vnet update --dns-servers` no funcionaba según cómo se creara la red virtual
* Se corrigió un problema por el que `dns zone import` no importaba correctamente los nombres DNS relativos

### <a name="reservations"></a>Reservations

* Versión preliminar inicial

### <a name="resource"></a>Recurso

* Se agregó compatibilidad para los identificadores de recursos al parámetro `--resource` y bloqueos en el nivel de recurso

### <a name="sql"></a>SQL

* Se ha agregado el parámetro `--ignore-missing-vnet-service-endpoint` a `sql server vnet-rule [create|update]`

### <a name="storage"></a>Storage

* Se cambió `storage account create` para usar la SKU `Standard_RAGRS` como valor predeterminado
* Se corrigieron los errores cuando se trabajaba con nombres de archivo/blob que incluían caracteres no ascii
* Se corrigió un error que impedía el uso de `--source-uri` con `storage [blob|file] copy start-batch`
* Se agregaron comandos para eliminar varios objetos mediante el uso de caracteres comodín con `storage [blob|file] delete-batch`
* Se corrigió un problema al habilitar las métricas con `storage metrics update`
* Se corrigió un problema con los archivos de más de 200 GB cuando se usa `storage blob upload-batch`
* Se corrigió un problema por el que `storage account [create|update]` ignoraba `--bypass` y `--default-action`

### <a name="vm"></a>máquina virtual

* Se corrigió un error de `vmss create` que impedía usar el nivel de tamaños `Basic`
* Se agregaron argumentos `--plan` a `[vm|vmss] create` para las imágenes personalizadas con información de facturación
* Se agregaron los comandos `vm secret `[add|remove|list]'
* Se cambió el nombre de `vm format-secret` a `vm secret format`.
* Se agregó el argumento `--encrypt format` a `vm encryption enable`

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
* [CAMBIO IMPORTANTE] Se ha cambiado el tipo de recurso `managedapp` de `appliances` a `applications` y `applianceDefinitions` a `applicationDefinitions`

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

### <a name="backup"></a>Copia de seguridad

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

* Se ha corregido el error "CustomDomain is not iterable" (No se puede iterar en CustomDomain) para `cdn custom-domain create`

### <a name="extension"></a>Extensión

* Versión inicial

### <a name="keyvault"></a>Keyvault

* Se ha corregido el problema por el que los permisos distinguían entre mayúsculas y minúsculas para `keyvault set-policy`

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

* Se ha agregado una nota legal a `--version`

### <a name="acs"></a>ACS

* Se han corregido las regiones en versión preliminar
* Se ha dado el formato correcto al valor predeterminado de `dns_name_prefix`
* Se ha optimizado la salida del comando acs

### <a name="appservice"></a>Appservice

* [CAMBIO IMPORTANTE] Se han corregido las incoherencias en la salida de `az webapp config appsettings [delete|set]`
* Se agregó un nuevo alias de `-i` para `az webapp config container set --docker-custom-image-name`.
* Se expuso `az webapp log show`.
* Se expusieron nuevos argumentos de `az webapp delete` para conservar el plan de App Service, las métricas o el registro de DNS.
* Corregido: Las configuración de los espacios se detecta correctamente.

### <a name="iot"></a>IoT

* Corrección n.º 3934: La creación de directivas ya no borra las directivas existentes.

### <a name="network"></a>Red

* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--private-access-services` a `--service-endpoints` para `vnet subnet [create|update]`
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
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de la opción `--encryption` a `--encryption-services` para el comando `az storage account create and az storage account update`
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

* Mensaje de error mejorado para `cdn endpoint list` cuando el perfil especificado por `--profile-name` no existe

### <a name="cloud"></a>Nube

* Se cambió la versión de API de punto de conexión de metadatos de nube al formato AAAA-MM-DD.
* No es necesario el punto de conexión de la galería.
* Compatibilidad para el registro de nubes solo con el punto de conexión de Resource Manager.
* Se agregó una opción a `cloud set` para elegir el perfil durante la selección de la nube actual.
* Se expuso `endpoint_vm_image_alias_doc`.

### <a name="cosmosdb"></a>CosmosDB

* Se corrigió poder crear una colección con clave de partición personalizada.
* Se ha agregado compatibilidad para TTL predeterminado de colección

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
* Se ha corregido el problema por el que `cmss create` con un equilibrador de carga existente requería `--backend-pool-name`
* Los discos de datos que se crean con `vm image create` comienzan con lun 0


## <a name="may-10-2017"></a>10 de mayo de 2017

Versión 2.0.6

* Se cambia el nombre de DocumentDB por CosmosDB.
* Se agrega RDBMS (MySQL y Postgres).
* Se incluyen los módulos de Data Lake Analytics y Data Lake Store
* Se incluye el módulo de Cognitive Services
* Se incluye el módulo de Service Fabric
* Se incluye el módulo de Interactive (se cambia el nombre de az-shell)
* Se agrega compatibilidad para los comandos de CDN
* Se quita el módulo de Container
* Se agrega "az -v" como método abreviado de "az --version" ([#2926](https://github.com/Azure/azure-cli/issues/2926)).
* Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).

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

* Se cambia el nombre del módulo de DocumentDB por CosmosDB
* Compatibilidad agregada para API de plano de datos de DocumentDB: administración de colecciones y bases de datos
* Compatibilidad agregada para habilitar la conmutación por error automática en cuentas de bases de datos
* Compatibilidad agregada para la nueva directiva de coherencia ConsistentPrefix

### <a name="data-lake-analytics"></a>Data Lake Analytics

* Se corrige un error por el que el filtrado de resultados y el estado de las listas de trabajos genera un error
* Agregar compatibilidad para el nuevo tipo de elementos de catálogo: paquete al que se accede a través de: `az dla catalog package`
* Se pueden enumerar los elementos del catálogo siguientes desde una base de datos (no se requiere ninguna especificación de esquema):

  * Tabla
  * Función con valores de tabla
  * Ver
  * Estadísticas de tabla. Esto también se puede enumerar con un esquema, pero sin especificar un nombre de tabla

### <a name="data-lake-store"></a>Data Lake Store

* Se actualiza la versión del SDK del sistema de archivos subyacente, que ofrece mayor compatibilidad para escenarios de limitación del lado del servidor
* Se mejora el rendimiento de la carga de paquetes y de la ejecución de comandos ([#2819](https://github.com/Azure/azure-cli/issues/2819)).
* Falta ayuda para mostrar el acceso. Se va a agregar. ([#2743](https://github.com/Azure/azure-cli/issues/2743))

### <a name="find"></a>Buscar

* Mejorar los resultados de búsqueda y permitir el control de versiones del índice de búsqueda

### <a name="keyvault"></a>KeyVault

* BC:`az keyvault certificate download` cambiar -e de la cadena o el binario por PEM o DER para representar mejor las opciones
* BC: Se quitan --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros
* Agregar el parámetro --validity a `keyvault certificate create` para reemplazar de forma selectiva el valor de --policy
* Corrige el problema en `keyvault certificate get-default-policy` por el que se exponían "expires" y "not_before", pero no "validity_in_months"
* Corrección de KeyVault para importar pem y pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))

### <a name="lab"></a>Laboratorio

* Se agregan comandos para crear, mostrar, eliminar y enumerar para el entorno del laboratorio
* Se agregan comandos para mostrar y enumerar para ver las plantillas de ARM en el laboratorio
* Se agrega la marca --environment en `az lab vm list` para filtrar las máquinas virtuales por el entorno en el laboratorio
* Se agrega el comando `az lab formula export-artifacts` para exportar una matriz de artefactos dentro de una fórmula del laboratorio
* Se agregan comandos para administrar secretos en un laboratorio

### <a name="monitor"></a>Supervisión

* Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009))
* Corrección de errores: la creación de la configuración de diagnósticos no acepta registros ni métricas de los comandos mostrar ([#2913](https://github.com/Azure/azure-cli/issues/2913))

### <a name="network"></a>Red

* Se agrega el comando `network watcher test-connectivity`
* Se agrega compatibilidad con el parámetro `--filters` para `network watcher packet-capture create`
* Se agrega compatibilidad para el drenaje de conexiones de Application Gateway
* Se agrega compatibilidad para la configuración de conjuntos de reglas WAF de Application Gateway
* Se agrega compatibilidad para reglas y filtros de ruta de ExpressRoute
* Se agrega compatibilidad para el enrutado geográfico de TrafficManager
* Se agrega compatibilidad para selectores de tráfico basados en directivas de conexiones VPN
* Se agrega compatibilidad para directivas IPSec de conexiones VPN
* Se corrige el error con `vpn-connection create` al usar los parámetros `--no-wait` o `--validate`
* Agregar compatibilidad para puertas de enlace de redes virtuales activas-activas
* Se quitan los valores NULL de la salida de los comandos `network vpn-connection list/show`
* BC: corregir errores en la salida de `vpn-connection create`
* Se corrige el error por el que el argumento "--key-length" de "vpn-connection create" no se analizaba correctamente
* Se corrige el error en `dns zone import` por el que los registros no se importaban correctamente
* Se corrige el error por el que `traffic-manager endpoint update` no funcionaba
* Se agregan los comandos en versión preliminar "network watcher"

### <a name="profile"></a>Perfil

* Admitir inicios de sesión cuando no se encuentran suscripciones ([#2560](https://github.com/Azure/azure-cli/issues/2560))
* Compatibilidad de nombre de parámetro corto en az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))

### <a name="redis"></a>Redis

* Agregar comando de actualización que también agrega la capacidad de escalar Redis Cache
* Se deja de usar el comando "update-settings"

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

* Se agregan los comandos az sql server list-usages y az sql db list-usages
* SQL: capacidad de conectarse directamente al proveedor de recursos ([#2832](https://github.com/Azure/azure-cli/issues/2832))

### <a name="storage"></a>Storage

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

Se publican los componentes ACR, Batch, KeyVault y SQL en esta versión

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

### <a name="core"></a>Núcleo

* Se agregan los módulos ACR, laboratorio, supervisión y búsqueda a la lista predeterminada
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
* AppService: desencadena la sincronización del control de código fuente después de la configuración ([2326 #](https://github.com/Azure/azure-cli/pull/2326))

### <a name="datalake"></a>DataLake

* Versión inicial del módulo de Data Lake Analytics
* Versión inicial del módulo de Data Lake Store

### <a name="docuemntdb"></a>DocumentDB

* DocumentDB: Compatibilidad agregada para enumerar las cadenas de conexión ([#2580](https://github.com/Azure/azure-cli/pull/2580))

### <a name="vm"></a>máquina virtual

* [Compute] Se ha agregado compatibilidad con AppGateway para crear conjuntos de escalado de máquinas virtuales ([#2570](https://github.com/Azure/azure-cli/pull/2570))
* [VM/VMSS] Compatibilidad mejorada con almacenamiento en caché en disco ([#2522](https://github.com/Azure/azure-cli/pull/2522))
* VM/VMSS: Incorporación de la lógica de validación de credenciales utilizada por el portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))
* Se han agregado comandos wait y soporte --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524))
* Conjunto de escalado de máquinas virtuales: admiten * para enumerar vistas de instancias entre máquinas virtuales ([#2467](https://github.com/Azure/azure-cli/pull/2467))
* Se ha agregado --secrets en máquinas virtuales y conjuntos de escalado de máquinas virtuales ([2212}(<https://github.com/Azure/azure-cli/pull/2212>))
* Se permite la creación de máquinas virtuales con un VHD especializado ([#2256](https://github.com/Azure/azure-cli/pull/2256))

## <a name="february-27-2017"></a>27 de febrero de 2017

Versión 2.0.0

Esta versión de la CLI de Azure 2.0 es la primera versión "disponible con carácter general". La disponibilidad general se aplica a estos módulos de comandos:
- Container Service (acs)
- Compute (incluidos Resource Manager, VM, conjuntos de escalado de máquinas virtuales, Managed Disks)
- Redes
- Storage

Estos módulos de comandos puede usarse en producción y son compatibles con el SLA estándar de Microsoft. Los problemas se pueden abrir directamente con el soporte técnico de Microsoft o en nuestra [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/). Puede hacer preguntas en [StackOverflow con la etiqueta azure-cli](http://stackoverflow.com/questions/tagged/azure-cli) o póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Puede enviarnos sus comentarios desde la línea de comandos con el comando `az feedback`

Los comandos de estos módulos son estables y no es previsible que cambie la sintaxis en futuras actualizaciones de esta versión de la CLI de Azure

Para comprobar la versión de la CLI, use `az --version`. La salida muestra la versión de la propia CLI (2.0.0 en este caso), los módulos de comandos individuales y las versiones de Python y GCC que esté usando

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
> Algunos módulos de comandos tienen un sufijo "b*n*" o "rc*n*". Estos módulos de comandos todavía están en versión preliminar y tendrán disponibilidad general en el futuro

Para más información, consulte estas instrucciones sobre la [obtención de compilaciones nocturnas](https://github.com/Azure/azure-cli#nightly-builds) y sobre [configuración del desarrollador y contribución de código](https://github.com/Azure/azure-cli#developer-setup).

Puede notificar los problemas con las versiones preliminares nocturnas de las siguientes maneras:
- Informe de los problemas en la [lista de problemas de GitHub](https://github.com/azure/azure-cli/issues/)
- Póngase en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)
- Envíe sus comentarios desde la línea de comandos con el comando `az feedback`

