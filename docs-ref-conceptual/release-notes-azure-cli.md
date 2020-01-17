---
title: Notas de la versión de la CLI de Azure
description: Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 01/13/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3ecb6fb41ee0ae60af58a02c934f2c295133f998
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913720"
---
# <a name="azure-cli-release-notes"></a>Notas de la versión de la CLI de Azure

## <a name="january-13-2020"></a>13 de enero de 2020

Versión 2.0.80

### <a name="compute"></a>Proceso

* disk update: Se han agregado --disk-encryption-set y --encryption-type.
* snapshot create/update: Se han agregado --disk-encryption-set y --encryption-type.

### <a name="storage"></a>Storage

* Se ha actualizado la versión de azure-mgmt-storage a la 7.1.0.
* `az storage account create`: Se han agregado `--encryption-key-type-for-table` y `--encryption-key-type-for-queue` para admitir el servicio de cifrado de tablas y colas.

## <a name="january-07-2020"></a>7 de enero de 2020

Versión 2.0.79

### <a name="acr"></a>ACR

* [CAMBIO IMPORTANTE] Se ha eliminado el parámetro "--os" para "acr build", "acr task create/update", "acr run" y "acr pack". En su lugar, utilice "--platform".

### <a name="appconfig"></a>AppConfig

* Se ha agregado compatibilidad para la importación y exportación de marcas de características.
* Se ha agregado el nuevo comando "az appconfig kv set-keyvault" para crear la referencia de Key Vault.
* Compatibilidad con diversas convenciones de nomenclatura al exportar marcas de características a un archivo.

### <a name="appservice"></a>AppService

* Se ha corregido el problema 7154: actualización de la documentación del comando <> para usar acentos invertidos en lugar de comillas simples.
* Se ha corregido el problema 11287: webapp up: de forma predeterminada, la aplicación creada con up "debe estar habilitada para SSL".
* Se ha corregido el problema 11592: se ha agregado la marca az webapp up para sitios HTML estáticos.

### <a name="arm"></a>ARM

* Se ha corregido `az resource tag`: no se pueden actualizar las etiquetas del almacén de Recovery Services.

### <a name="backup"></a>Copia de seguridad

* Se ha agregado un nuevo comando "backup protection undelete" para habilitar la característica de eliminación temporal para la carga de trabajo de IaasVM.
* Se ha agregado el nuevo parámetro "--soft-delete-feature-state" al comando set backup-properties.
* Se ha agregado compatibilidad con la exclusión de disco para la carga de trabajo de IaasVM.

### <a name="compute"></a>Proceso

* Se ha corregido el error de `vm create` en el perfil de Azure Stack.
* vm monitor metrics tail/list-definitions: compatibilidad con métricas de consultas y definiciones de lista para una máquina virtual.
* Se ha agregado la nueva acción del comando reapply para az vm.

### <a name="hdinsight"></a>HDInsight

* Compatibilidad con la creación de un clúster de Kafka con Kafka Rest Proxy.
* Se ha actualizado azure-mgmt-hdinsight a la versión 1.3.0.

### <a name="misc"></a>Varios:

* Se ha agregado el comando en versión preliminar `az version show` para mostrar las versiones de los módulos de la CLI de Azure y las extensiones en formato JSON de forma predeterminada o con el formato configurado con --output.

### <a name="event-hubs"></a>Event Hubs

* [CAMBIO IMPORTANTE] Se ha eliminado la opción de estado "ReceiveDisabled" de los comandos "az eventhubs eventhub update" y "az eventhubs eventhub create". Esta opción no es válida para entidades de Event Hubs.

### <a name="service-bus"></a>Azure Service Bus

* [CAMBIO IMPORTANTE] Se ha eliminado la opción de estado "ReceiveDisabled" de los comandos "az servicebus topic create", "az servicebus topic update", "az servicebus queue create" y "az servicebus queue update". Esta opción no es válida para temas y colas de Service Bus.

### <a name="rbac"></a>RBAC

* Se ha corregido el error 11712: `az ad app/sp show` no devuelve el código de salida 3 cuando la aplicación o la entidad de servicio no existen.

### <a name="storage"></a>Storage

* `az storage account create`: se ha eliminado la marca en versión preliminar para el parámetro --enable-hierarchical-namespace.
* Se ha actualizado la versión de azure-mgmt-storage a la 7.0.0 para usar la versión de API 2019-06-01.
* Se han agregado los nuevos parámetros `--enable-delete-retention` y `--delete-retention-days` para admitir la administración de la directiva de retención de eliminación para blob-service-properties de la cuenta de almacenamiento.

## <a name="december-17-2019"></a>17 de diciembre de 2019

2.0.78

### <a name="acr"></a>ACR

* Se ha agregado la compatibilidad con el contexto local en acr task run.

### <a name="acs"></a>ACS

* [CAMBIO IMPORTANTE] az openshift create: se ha cambiado el nombre de `--workspace-resource-id` a `--workspace-id`.

### <a name="ams"></a>AMS

* Se han actualizado los comandos show para devolver un código 3 cuando no se encuentra el recurso.

### <a name="appconfig"></a>AppConfig

* Se ha corregido el error al anexar la versión de la API a la dirección URL de la solicitud. La solución existente no funciona con la paginación.
* Se ha agregado compatibilidad para mostrar idiomas además del inglés, ya que el servicio de back-end admite Unicode para la globalización.

### <a name="appservice"></a>AppService

* Se ha corregido el problema 11217: webapp: az webapp config ssl upload debe admitir el parámetro de ranura.
* Se ha corregido el problema 10965: Error: El nombre no puede estar vacío. Se permite la eliminación por ip_address y subnet (dirección IP y subred).
* Se ha agregado compatibilidad con la importación de certificados desde `az webapp config ssl import` de Key Vault.

### <a name="arm"></a>ARM

* Se ha actualizado el paquete azure-mgmt-resource para usar la versión 6.0.0.
* Compatibilidad entre inquilinos para el comando `az group deployment create` mediante la adición del nuevo parámetro `--aux-subs`.
* Se ha agregado un nuevo parámetro `--metadata` para admitir la adición de información de metadatos para definiciones de conjuntos de directivas.

### <a name="backup"></a>Copia de seguridad

* Se ha agregado compatibilidad con la copia de seguridad para cargas de trabajo de SQL y SAP Hana.

### <a name="botservice"></a>BotService

* [Cambio importante] Se ha eliminado la marca "--version" del comando en versión preliminar "az bot create". Solo se admiten los bots del SDK V4.
* Se ha agregado la comprobación de disponibilidad del nombre para "az bot create".
* Se ha agregado compatibilidad para actualizar la dirección URL del icono de un bot mediante "az bot update".
* Se ha agregado compatibilidad para actualizar un canal de Direct Line mediante "az bot directline update".
* Se ha agregado compatibilidad con la marca "--enable-enhanced-auth" para "az bot directline create".
* Los siguientes grupos de comandos están en disponibilidad general y no en versión preliminar: "az bot authsetting".
* Los siguientes comandos de "az bot" están en disponibilidad general y no en versión preliminar: "create", "prepare-deploy", "show", "delete", "update".
* Se ha corregido el cambio realizado por "az bot prepare-deploy" del valor de "--proj-file-path" a minúsculas (por ejemplo, de "Test.csproj" a "test.csproj").

### <a name="compute"></a>Proceso

* vmss create/update: Se ha agregado --scale-in-policy, que decide qué máquinas virtuales se eligen para su eliminación cuando se reduce el tamaño de un conjunto de escalado de máquinas virtuales.
* vm/vmss update: Se ha agregado --priority.
* vm/vmss update: Se ha agregado --max-price.
* Se ha agregado el grupo de comandos disk-encryption-set (create, show, update, delete, list).
* disk create: Se han agregado --encryption-type y --disk-encryption-set.
* vm/vmss create: Se han agregado --os-disk-encryption-set y --data-disk-encryption-sets.

### <a name="core"></a>Core

* Se eliminó la compatibilidad con Python 3.4.
* Complemento HaTS survey en varios comandos.

### <a name="dls"></a>DLS

* Se ha actualizado la versión del SDK de ADLS (0.0.48).

### <a name="install"></a>Instalar

* El script de instalación admite Python 3.8.

### <a name="iot"></a>IoT

* [CAMBIO IMPORTANTE] Se ha eliminado el parámetro --failover-region de manual-failover. Ahora se realizará la conmutación por error a la región secundaria emparejada geográficamente asignada.

### <a name="key-vault"></a>Key Vault

* Se ha corregido el error 8095: `az keyvault storage remove`: mejora del mensaje de ayuda.
* Se ha corregido el error 8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: se ha corregido el error de validación en el parámetro `--maxresults`.
* Se ha corregido el error 10512: `az keyvault set-policy`: mejora del mensaje de error cuando no se especifican `--object-id`, `--spn` ni `--upn`.
* Se ha corregido el error 10846: `az keyvault secret show-deleted`: cuando se especifica `--id`, no se requiere `--name/-n`.
* Se ha corregido el error 11084: `az keyvault secret download`: mejora del mensaje de ayuda del parámetro `--encoding`.

### <a name="network"></a>Red

* az network application-gateway probe: se ha agregado compatibilidad con la opción -port para especificar un puerto para sondear servidores de back-end en la creación y actualización.
* az network application-gateway url-path-map create/update: se ha corregido el error de `--waf-policy`.
* az network application-gateway: se ha agregado compatibilidad con `--rewrite-rule-set`.
* az network list-service-aliases: se ha agregado compatibilidad con los alias de servicio de lista, que se pueden usar para las directivas del punto de conexión de servicio.
* az network dns zone import: se ha agregado compatibilidad con .@ en el nombre de registro.

### <a name="packaging"></a>Packaging

* Se han agregado compilaciones de perímetro posterior para la instalación de pip.
* Se ha agregado el paquete eoan de Ubuntu.

### <a name="policy"></a>Directiva

* Se ha agregado compatibilidad con la versión 2019-09-01 de Policy API.
* az policy set-definition: se ha agregado compatibilidad con la agrupación dentro de definiciones de conjuntos de directivas con el parámetro `--definition-groups`.

### <a name="redis"></a>Redis

* Se ha agregado el parámetro en versión preliminar `--replicas-per-master` al comando `az redis create`.
* Se ha actualizado azure-mgmt-redis de la versión 6.0.0 a la 7.0.0rc1.

### <a name="servicefabric"></a>ServiceFabric

* Se ha corregido la lógica de adición de tipo de nodo, incluido el error 10963: la adición de un nuevo tipo de nodo con el nivel de durabilidad Gold siempre producirá un error de la CLI.
* La versión de ServiceFabricNodeVmExt se ha actualizado al a 1.1 en la plantilla de creación.

### <a name="sql"></a>SQL

* Se han agregado los parámetros "--read-scale" y "--read-replicas" a los comandos create y update de SQL DB para admitir la administración de escalado de lectura.

### <a name="storage"></a>Storage

* Versión de disponibilidad general de la propiedad de recursos compartidos de archivos grandes para el comando de creación y actualización de la cuenta de almacenamiento.
* Versión de disponibilidad general de la compatibilidad de los token de SAS para la delegación de usuarios.
* Se han agregado los nuevos comandos `az storage account blob-service-properties show` y `az storage account blob-service-properties update --enable-change-feed` para administrar las propiedades de Blob Service para la cuenta de almacenamiento.
* [PRÓXIMO CAMBIO IMPORTANTE] `az storage copy`: ya no se admite el carácter `*` como comodín en la dirección URL, pero se agregarán nuevos parámetros --include-pattern y --exclude-pattern con compatibilidad con caracteres comodín `*`.
* Se ha corregido el problema 11043: se ha agregado compatibilidad para eliminar todo el contenedor o el recurso compartido en el comando `az storage remove`.

## <a name="november-26-2019"></a>26 de noviembre de 2019

Versión 2.0.77

### <a name="acr"></a>ACR

* El parámetro `--branch` de acr task create/update ha quedado en desuso.

### <a name="azure-red-hat-openshift"></a>Red Hat OpenShift en Azure

* Se ha agregado la marca `--workspace-resource-id` para permitir la creación de un clúster de Red Hat OpenShift en Azure con supervisión.
* Se ha agregado `monitor_profile` para crear un clúster de Red Hat OpenShift en Azure con supervisión.

### <a name="aks"></a>AKS

* Se ha agregado compatibilidad con la operación de rotación de certificados del clúster mediante "az aks rotate-certs".

### <a name="appconfig"></a>AppConfig

* Se ha agregado compatibilidad con el uso de ":" como separador de `as az appconfig kv import`.
* Se ha corregido un problema para enumerar los valores de clave con varias etiquetas que incluyen la etiqueta nula. 
* Se ha actualizado el SDK del plano de administración, azure-mgmt-appconfiguration, a la versión 0.3.0. 

### <a name="appservice"></a>AppService

* Se ha corregido el problema 11100: Error de atributo para az webapp up al crear el plan de servicio
* az webapp up: cuando se fuerza la creación o implementación en un sitio para lenguajes admitidos, no se usan los valores predeterminados.
* Se ha agregado compatibilidad para App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete

### <a name="backup"></a>Copia de seguridad

* Se ha corregido el problema en los elementos asociados a listas de directivas de az backup. Se ha agregado el parámetro opcional BackupManagementType.

### <a name="compute"></a>Proceso

* Se ha actualizado la versión de la API de proceso, discos e instantáneas a la 2019-07-01.
* vmss create: mejoras para --orchestration-mode
* sig image-definition create: se ha agregado --os-state para poder especificar si las máquinas virtuales creadas con esta imagen están "Generalizadas" o "Especializadas".
* sig image-definition create: se ha agregado --hyper-v-generation para poder especificar la generación del hipervisor.
* sig image-version create: se ha agregado compatibilidad con --os-snapshot y --data-snapshots.
* image create: se ha agregado --data-disk-caching para poder especificar la configuración de almacenamiento en caché de los discos de datos.
* Actualización del SDK de Compute para Python a la versión 10.0.0
* vm/vmss create: se ha agregado "Spot" a la propiedad de la enumeración "Priority".
* [Cambio importante] Se ha cambiado el nombre del parámetro "--max-billing" a "--max-price" para máquinas virtuales y VMSS, para que sean coherentes con los cmdlets de Swagger y Powershell.
* vm monitor log show: se ha agregado compatibilidad para la consulta del registro en el área de trabajo de Log Analytics vinculada.

### <a name="iot"></a>IoT

* Corrección 2531: se han agregado argumentos de utilidad para la actualización del concentrador.
* Corrección 8323: se han agregado los parámetros que faltaban para crear el punto de conexión personalizado de almacenamiento.
* Corrección del error de regresión: se han revertido los cambios que invalidan el punto de conexión de almacenamiento predeterminado.

### <a name="key-vault"></a>Key Vault

* Corrección 11121: ahora, con `az keyvault certificate list`, al pasar `--include-pending` no se requiere un valor `true` o `false`.

### <a name="netappfiles"></a>NetAppFiles

* Se ha actualizado azure-mgmt-netapp a la versión 0.7.0, que incluye algunas propiedades de volumen adicionales asociadas a futuras operaciones de replicación.

### <a name="network"></a>Red

* application-gateway waf-config: en desuso
* application-gateway waf-policy: se han agregado reglas administradas de subgrupo para administrar conjuntos de reglas administradas y reglas de exclusión.
* application-gateway waf-policy: se ha agregado la configuración de directivas de subgrupo para administrar la configuración global de una directiva de WAF.
* [Cambio importante] application-gateway waf-policy: se ha cambiado el nombre de la regla de subgrupo a regla personalizada.
* application-gateway http-listener: se ha agregado --firewall-policy en la creación.
* application-gateway url-path-map rule: se ha agregado --firewall-policy en la creación.

### <a name="packaging"></a>Packaging

* Se ha reescrito az wrapper en Python.
* Se ha agregado compatibilidad para Python 3.8.
* Se ha cambiado a Python 3 para el paquete RPM.

### <a name="profile"></a>Perfil

* Se ha corregido el error al ejecutar `az login -u {} -p {}` con una cuenta Microsoft.
* Se ha corregido el error `SSLError` al ejecutar `az login` detrás de un servidor proxy con certificado raíz autofirmado.
* Corrección 10578: `az login` se bloquea cuando se inicia más de una instancia al mismo tiempo en Windows o WSL.
* Corrección 11059: `az login --allow-no-subscriptions` produce un error si hay suscripciones en el inquilino.
* Corrección 11238: después de cambiar el nombre de una suscripción, al iniciar sesión con MSI aparecerá dos veces la misma suscripción.

### <a name="rbac"></a>RBAC

* Corrección 10996: corrección del error para `--force-change-password-next-login` en `az ad user update` cuando no se especifica `--password`.

### <a name="redis"></a>Redis

* Corrección 2902: se impedía establecer configuraciones de memoria al actualizar la memoria caché de la SKU Básica.

### <a name="reservations"></a>Reservations

* Actualización de la versión del SDK a la 0.6.0
* Se ha agregado información de detalles del plan de facturación después de llamar a Get-Gatalogs.
* Se ha agregado el nuevo comando `az reservations reservation-order calculate` para calcular el precio de una reserva.
* Se ha agregado el nuevo comando `az reservations reservation-order purchase` para adquirir una nueva reserva.

### <a name="rest"></a>Rest
* Se ha cambiado `az rest` a Disponibilidad general.

### <a name="sql"></a>SQL

* Se ha actualizado azure-mgmt-sql a la versión 0.15.0.

### <a name="storage"></a>Storage

* storage account create: se ha agregado --enable-hierarchical-namespace para admitir la semántica del sistema de archivos en Blob Service.
* Se ha eliminado la excepción no relacionada del mensaje de error.
* Se han corregido problemas con el mensaje de error incorrecto: "No tiene los permisos necesarios para realizar esta operación" en bloqueos de las reglas de red o en un error de autenticación.

## <a name="november-4-2019"></a>4 de noviembre de 2019

Versión 2.0.76

### <a name="acr"></a>ACR

* Se ha agregado un parámetro en versión preliminar `--pack-image-tag` al comando `az acr pack build`.
* Se ha agregado compatibilidad para habilitar la auditoría al crear un registro.
* Se admite RBAC en el ámbito del repositorio.

### <a name="aks"></a>AKS

* Se han agregado `--enable-cluster-autoscaler`, `--min-count` y `--max-count` al comando `az aks create`, que habilita el escalador automático de clústeres para el grupo de nodos.
* Se han agregado las marcas anteriores, así como `--update-cluster-autoscaler` y `--disable-cluster-autoscaler`, al comando `az aks update`, lo que permite actualizar el escalador automático de clústeres.

### <a name="appconfig"></a>AppConfig

* Se ha agregado el grupo de comandos de características appConfig para administrar las marcas de características almacenadas en una configuración de aplicación.
* Se ha corregido un error secundario menor del comando de appconfig de exportación de almacén de claves a archivo. Se deja de leer el contenido del archivo de destino durante la exportación.

### <a name="appservice"></a>AppService

* `az appservice plan create`: Se ha agregado compatibilidad para establecer "persitescaling" en plan create de appservice.
* Se ha corregido un problema por el que la operación de enlace de SSL de configuración de aplicación web quitaba las etiquetas existentes del recurso.
* Se ha agregado la marca `--build-remote` a `az functionapp deployment source config-zip` para admitir la acción de compilación remota durante la implementación de la aplicación de función.
* Se ha cambiado la versión predeterminada del nodo en las aplicaciones de función a ~10 para Windows.
* Se ha agregado la propiedad `--runtime-version` a `az functionapp create`.

### <a name="arm"></a>ARM

* `az deployment/group deployment validate`: Se ha agregado el parámetro `--handle-extended-json-format` para admitir varias líneas y comentarios en la plantilla JSON durante la implementación.
* Se ha incrementado la versión de azure-mgmt-resource a 2019-07-01.

### <a name="backup"></a>Copia de seguridad

* Se ha agregado compatibilidad con la copia de seguridad de AzureFiles.

### <a name="compute"></a>Proceso

* `az vm create`: Se ha agregado una advertencia al especificar juntas redes aceleradas y una NIC existente.
* `az vm create`: Se ha agregado `--vmss` para especificar un conjunto de escalado de máquinas virtuales existente al que se debe asignar la máquina virtual.
* `az vm/vmss create`: Se ha agregado una copia local del archivo de alias de imagen para poder tener acceso a él en un entorno de red restringido.
* `az vmss create`: Se ha agregado `--orchestration-mode` para especificar cómo se administran las máquinas virtuales mediante el conjunto de escalado.
* `az vm/vmss update`: Se ha agregado `--ultra-ssd-enabled` para poder actualizar la configuración de SSD.
* [CAMBIO IMPORTANTE] `az vm extension set`: Se ha corregido un error por el que los usuarios no podían establecer una extensión en una máquina virtual con `--ids`.
* Se han agregado nuevos comandos `az vm image terms accept/cancel/show` para administrar los términos de la imagen de Azure Marketplace.
* Se ha actualizado VMAccessForLinux a la versión 1.5.

### <a name="cosmosdb"></a>CosmosDB

* [CAMBIO IMPORTANTE] `az sql container create`: Se ha cambiado el parámetro `--partition-key-path` a obligatorio.
* [CAMBIO IMPORTANTE] `az gremlin graph create`: Se ha cambiado el parámetro `--partition-key-path` a obligatorio.
* `az sql container create`: Se han agregado `--unique-key-policy` y `--conflict-resolution-policy`
* `az sql container create/update`: Se ha actualizado el esquema predeterminado `--idx`.
* `gremlin graph create`: Se agregó `--conflict-resolution-policy`.
* `gremlin graph create/update`: Se ha actualizado el esquema predeterminado `--idx`.
* Se ha corregido el error tipográfico en el mensaje de ayuda
* base de datos: Se ha agregado la información de desuso.
* colección: Se ha agregado la información de desuso.

### <a name="iot"></a>IoT

* Se ha agregado un nuevo tipo de origen de enrutamiento: DigitalTwinChangeEvents
* Se han corregido las características que faltan en `az iot hub create`.

### <a name="key-vault"></a>Key Vault

* Se ha corregido un error inesperado cuando el archivo de certificado no existe.
* Se ha corregido `az keyvault recover/purge` porque no funcionaba.

### <a name="netappfiles"></a>NetAppFiles

* Se ha actualizado azure-mgmt-netapp a 0.6.0 para usar la API versión 2019-07-01. Esta nueva versión de API incluye:

    - La creación del volumen `--protocol-types` ahora acepta "NFSv4.1", no "NFSv4".
    - La propiedad de directiva de exportación de volumen ahora tiene el nombre "nfsv41", no "nfsv4".
    - Se ha cambiado el nombre del volumen `--creation-token` a `--file-path`.
    - La fecha de creación de la instantánea ahora se llamada simplemente "created".

### <a name="network"></a>Red

* `az network private-dns link vnet create/update`: Se ha agregado compatibilidad con la vinculación de redes virtuales entre inquilinos.
* [CAMBIO IMPORTANTE] `az network vnet subnet list`: Se han cambiado `--resource-group` y `--vnet-name` para que ahora sean obligatorios.
* `az network public-ip prefix create`: se ha agregado compatibilidad para especificar la versión de la dirección IP (IPv4, IPv6) durante la creación.
* Se ha aumentado la versión de Azure-MGMT-Network a 7.0.0 y la versión de API a 2019-09-01.
* `az network vrouter`: se ha agregado compatibilidad con un nuevo enrutador virtual de servicio y el emparejamiento de enrutador virtual.
* `az network express-route gateway connection`: Se ha agregado compatibilidad con `--internet-security`

### <a name="profile"></a>Perfil

* Se ha corregido `az account get-access-token --resource-type ms-graph` porque no funcionaba.
* Se ha quitado la advertencia de `az login`.

### <a name="rbac"></a>RBAC

* Se ha corregido `az ad app update --id {} --display-name {}` porque no funcionaba.

### <a name="servicefabric"></a>ServiceFabric

* `az sf cluster create`: Se ha corregido un problema mediante la modificación de VMSS de proceso template.json Windows y Linux de Service Fabric de discos estándar a discos administrados.

### <a name="sql"></a>SQL

* Se han agregado los parámetros `--compute-model`, `--auto-pause-delay`y `--min-capacity` para admitir las operaciones CRUD para la nueva oferta de SQL Database: Modelo de proceso sin servidor.

### <a name="storage"></a>Storage

* `az storage account create/update`: Se ha agregado el parámetro --enable-files-adds y el grupo de argumentos de propiedades de Azure Active Directory para admitir la autenticación de AD DS en Azure Files.
* Se ha expandido `az storage account keys list/renew` para admitir la enumeración o regeneración de claves Kerberos de la cuenta de almacenamiento.

## <a name="october-15-2019"></a>15 de octubre de 2019

Versión 2.0.75

### <a name="aks"></a>AKS

* Se ha cambiado el valor predeterminado de `--load-balancer-sku` a `standard` si es compatible con la versión de Kubernetes.
* Se ha cambiado el valor predeterminado de `--vm-set-type` a `virtualmachinescalesets` si es compatible con la versión de Kubernetes.

### <a name="ams"></a>AMS

* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `job start` a `job create`.
* [CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--ask` de `content-key-policy create` para que use una cadena hexadecimal de 32 caracteres en lugar de UTF8.

### <a name="appservice"></a>AppService

* Se han agregado comandos `webapp config access-restriction show|set|add|remove`.
* Se ha agregado un mejor control de errores a `webapp up`.
* Se ha agregado compatibilidad para la SKU `Isolated` a `appservice plan update`.

### <a name="arm"></a>ARM

* Se ha agregado el parámetro `--handle-extended-json-format` a `deployment create` para admitir varias líneas y comentarios en la plantilla JSON.

### <a name="compute"></a>Proceso

* Se ha agregado el parámetro `--enable-agent` a `vm create`
* Se ha cambiado `vm create` para que use SKU de IP pública estándar automáticamente al usar zonas.
* Se ha cambiado `vm create` para que cree automáticamente un nombre de equipo válido para una máquina virtual si no se proporciona ninguno.
* Se ha agregado el parámetro `--computer-name-prefix` a `vmss create` para admitir el prefijo de nombre de equipo personalizado de las máquinas virtuales en el VMSS.
* Agregue el parámetro `--workspace` a `vm create` para habilitar automáticamente el área de trabajo de Log Analytics.
* Se ha actualizado la versión de API de galerías a 2019-07-01.

### <a name="core"></a>Core

* Se ha agregado la comprobación de la sintaxis del parámetro `--set` en el comando de actualización genérico.

### <a name="iot"></a>IoT

* Se ha corregido un problema por el que `iot hub show` producía un error con el mensaje "recurso no encontrado".

### <a name="monitor"></a>Supervisión

* Se ha agregado compatibilidad para CRUD a `monitor log-analytics workspace`.

### <a name="network"></a>Red

* Se ha agregado compatibilidad para la vinculación virtual entre inquilinos a `network private-dns link vnet [create|update]`.
* [CAMBIO IMPORTANTE] Se ha cambiado `network vnet subnet list` para requerir los parámetros `--resource-group` y `--vnet-name`.

### <a name="sql"></a>SQL

* Se han agregado comandos a `sql mi ad-admin` que admiten la configuración de un administrador de AAD en instancias administradas.

### <a name="storage"></a>Storage

* Se ha agregado el parámetro `--preserve-s2s-access-tier` a `storage copy` para conservar el nivel de acceso durante la copia de servicio a servicio.
* Se ha agregado el parámetro `--enable-large-file-share` a `storage account [create|update]` para admitir recursos compartidos de archivos grandes para la cuenta de almacenamiento.

## <a name="september-24-2019"></a>24 de septiembre de 2019

Versión 2.0.74

### <a name="acr"></a>ACR

* Se ha agregado un parámetro `--type` obligatorio a `acr config retention update`.
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre del parámetro `--name -n` a `--registry -r ` para el grupo de comandos `acr config`.

### <a name="aks"></a>AKS

* Se ha agregado el parámetro `--load-balancer-sku` al comando `aks create`, lo que permite crear un clúster de AKS con SLB.
* Se han agregado los parámetros `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` y `--load-balancer-outbound-ip-prefixes` a los comandos `aks [create|update]`, lo que permite actualizar el perfil del equilibrador de carga de un clúster de AKS con SLB.
* Se ha agregado el parámetro `--vm-set-type` al comando `aks create`, lo que permite especificar los tipos de máquina virtual de un clúster de AKS (vmas o vmss).

### <a name="arm"></a>ARM

* Se ha agregado el parámetro `--handle-extended-json-format` al comando `group deployment create` para admitir varias líneas y comentarios en la plantilla JSON.

### <a name="compute"></a>Proceso

* Se ha agregado el parámetro `--terminate-notification-time` a los comandos `vmss [create|update]` para poder finalizar la capacidad de configurar eventos programados.
* Se ha agregado el parámetro `--enable-terminate-notification` al comando `vmss update` para poder finalizar la capacidad de configurar eventos programados.
* Se han agregado los parámetros `--priority,` `--eviction-policy,` `--max-billing` a los comandos `[vm|vmss] create`.
* Se ha cambiado `disk create` para permitir especificar el tamaño exacto de la carga del disco.
* Se ha agregado compatibilidad para instantáneas incrementales de discos administrados a `snapshot create`.

### <a name="cosmos-db"></a>Cosmos DB

* Se ha agregado el parámetro `--type <key-type>` al comando `cosmosdb keys list` para mostrar la clave, las claves de solo lectura o las cadenas de conexión.
* Se agregó el comando `cosmosdb keys regenerate`.
* [EN DESUSO] Se han dejado de usar los comandos `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` y `cosmosdb list-read-only-keys`.

### <a name="eventgrid"></a>EventGrid

* Se ha corregido el texto de ayuda del punto de conexión para que haga referencia al parámetro correcto.

### <a name="key-vault"></a>Key Vault

* Se ha corregido un problema por el que un inquilino (`login -t`) podía producir un error en `keyvault create`.

### <a name="monitor"></a>Supervisión

* Se ha corregido un problema por el que no se permitía el carácter `:` en el argumento `--condition` de `monitor metrics alert create`.

### <a name="policy"></a>Directiva

* Se ha agregado compatibilidad con la versión 2019-06-01 de Policy API.
* Se ha agregado el parámetro `--enforcement-mode` al comando `policy assignment create`.

### <a name="storage"></a>Storage

* Se ha agregado el parámetro `--blob-type` al comando `az storage copy`.

## <a name="september-10-2019"></a>10 de septiembre de 2019

### <a name="acr"></a>ACR

* Se ha agregado el grupo de comandos `acr config retention` para configurar la directiva de retención.

### <a name="aks"></a>AKS

* Se ha agregado compatibilidad para la integración de ACR con los siguientes comandos:
  * Se ha agregado el parámetro `--attach-acr` a `aks [create|update]` para asociar un ACR a un clúster de AKS.
  * Se ha agregado el parámetro `--detach-acr` a `aks update` para desasociar un ACR de un clúster de AKS.

### <a name="arm"></a>ARM

* Se ha actualizado para usar la versión 2019-05-10 de la API.

### <a name="batch"></a>Batch

* Se han agregado nuevas opciones de configuración de JSON a `--json-file` para `batch pool create`:
  * Se ha agregado `MountConfigurations` para montajes del sistema de archivos (consulte https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obtener más información).
  * Se ha agregado la propiedad `publicIPs` opcional en `NetworkConfiguration` para las direcciones IP públicas en grupos (consulte https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body para obtener más información).
* Se ha agregado compatibilidad para la galería de imágenes compartidas a `--image`.
* [CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--start-task-wait-for-success` en `batch pool create` a `true`.
* [CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `Scope` en `AutoUserSpecification` para que siempre sea Pool (era `Task` en los nodos Windows, `Pool` en los nodos Linux).
  * Este argumento solo se puede establecer desde una configuración de JSON con `--json-file`.

### <a name="hdinsight"></a>HDInsight

* Versión de disponibilidad general
* [CAMBIO IMPORTANTE] Se ha cambiado el parámetro `--workernode-count/-c` de `az hdinsight resize` para que sea obligatorio.

### <a name="key-vault"></a>Key Vault

* Se ha corregido un problema por el que no se podían eliminar las subredes de las reglas de red.
* Se ha corregido un problema por el que se podían agregar subredes y direcciones IP duplicadas a las reglas de red.

### <a name="network"></a>Red

* Se ha agregado el parámetro `--interval` a `network watcher flow-log` para establecer el valor del intervalo de análisis del tráfico.
* Se ha agregado `network application-gateway identity` para administrar la identidad de puerta de enlace.
* Se ha agregado compatibilidad para establecer el identificador del almacén de claves en `network application-gateway ssl-cert`.
* Se agregó `network express-route peering peer-connection [show|list]`.

### <a name="policy"></a>Directiva

* Se ha actualizado para usar la versión 2019-01-01 de la API.

## <a name="august-27-2019"></a>27 de agosto de 2019

Versión 2.0.72

### <a name="acr"></a>ACR

* [CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para la SKU `classic`.

### <a name="api-management"></a>API Management

* [VERSIÓN PRELIMINAR] Se ha agregado el grupo de comandos `apim`

### <a name="appservice"></a>AppService

* Se ha corregido un problema con el comando `webapp webjob continuous start` al especificar una ranura
* Se ha cambiado `webapp up` para detectar la carpeta `env` y quitarla del archivo usado para la implementación

### <a name="keyvault"></a>Keyvault

* Se ha corregido un error en `keyvault secret set` que hacía que se ignorara el argumento `--expires`

### <a name="network"></a>Red

* Se ha agregado compatibilidad para las direcciones IPv6 con argumentos `--private-ip-address-version`
* Se han agregado nuevos comandos `network private-endpoint [create|update|list-types]` para la administración de un punto de conexión privado
* Se ha agregado el grupo de comandos `network private-link-service`
* Se agregaron los argumentos `--private-endpoint-network-policies` y `--private-link-service-network-policies` a `network vnet subnet update`

### <a name="rbac"></a>RBAC

* Se ha corregido el problema con `ad app update --homepage` por el cual la página principal no se actualizaba

### <a name="servicefabric"></a>ServiceFabric

* Se ha agregado compatibilidad con los nombres de Key Vault que combinan mayúsculas y minúsculas
* Se ha solucionado el problema que se producía al usar certificados en Key Vault
* Se ha solucionado el problema con el uso de archivos de certificado de PFX
* Se ha solucionado el problema con `sf cluster certificate add` que se producía cuando no se especificaba el grupo de recursos de Key Vault
* Se ha corregido el problema con `sf cluster set` que no funcionaba

### <a name="signalr"></a>SignalR

* Se han agregado nuevos comandos:
  * `signalr cors`: Administración de SignalR CORS
  * `signalr restart`: Reinicio de una instancia de SignalR Service
  * `signalr update`: Actualización de una instancia de SignalR Service
* Se agregó el argumento `--service-mode` a `signalr create`

### <a name="storage"></a>Storage

* Se agregó el comando `storage account revoke-delegation-keys`.

## <a name="august-13-2019"></a>13 de agosto de 2019

Versión 2.0.71

### <a name="appservice"></a>AppService

* Se ha corregido un problema por el que se producían errores con los comandos `webapp webjob continuous` en los espacios

### <a name="botservice"></a>BotService

* [CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para crear bots con el SDK v3.

### <a name="cognitiveservices"></a>CognitiveServices

* Se agregaron los comandos `cognitiveservices account network-rule`.

### <a name="cosmos-db"></a>Cosmos DB

* Se ha quitado la advertencia al actualizar varias ubicaciones de escritura.
* Se han agregado comandos CRUD para recursos de CosmosDB SQL, MongoDB, Cassandra, Gremlin y Table, así como capacidad de proceso para los recursos.

### <a name="hdinsight"></a>HDInsight

Esta versión contiene un gran número de cambios importantes.

* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `hdinsight create`:
  * Cambio de nombre de `--storage-default-container` a `--storage-container`
  * Cambio de nombre de `--storage-default-filesystem` a `--storage-filesystem`
* [CAMBIO IMPORTANTE] Se ha cambiado el argumento `--name` de `application create` para que represente el nombre de la aplicación en lugar del nombre del clúster.
* Se ha agregado el argumento `--cluster-name` a `application create` para reemplazar la funcionalidad de `--name` antigua.
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de los parámetros de `application create`:
  * Cambio de nombre de `--application-type` a `--type`
  * Cambio de nombre de `--marketplace-identifier` a `--marketplace-id`
  * Cambio de nombre de `--https-endpoint-access-mode` a `--access-mode`
  * Se cambió el nombre de `--https-endpoint-destination-port` a `--destination-port`.
* [CAMBIO IMPORTANTE] Se han quitado los parámetros de `application create`:
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--target-instance-count` a `--workernode-count` para `hdinsight resize`.
* [CAMBIO IMPORTANTE] Se han cambiado todos los comandos del grupo `hdinsight script-action` para que usen el parámetro `--name` como nombre de la acción de script.
* Se ha agregado el argumento `--cluster-name` a todos los comandos `hdinsight script-action` para reemplazar la funcionalidad de `--name` antigua.
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `--script-execution-id` a `--execution-id` para todos los comandos `hdinsight script-action`.
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `hdinsight script-action show` a `hdinsight script-action show-execution-details`
* [CAMBIO IMPORTANTE] Se han cambiado los parámetros a `hdinsight script-action execute --roles` para que estén separados por espacios en lugar de por comas.
* [CAMBIO IMPORTANTE] Se ha eliminado el parámetro `--persisted` de `hdinsight script-action list`.
* Se ha cambiado el parámetro `hdinsight create --cluster-configurations` para aceptar una ruta a un archivo JSON local o una cadena JSON.
* Se ha agregado el comando `hdinsight script-action list-execution-history`
* Se ha cambiado `hdinsight monitor enable --workspace` para aceptar un identificador o un nombre de área de trabajo de Log Analytics.
* Se ha agregado el argumento `hdinsight monitor enable --primary-key`, que es necesario si se proporciona un identificador de área de trabajo como parámetro.
* Se han agregado más ejemplos y se han actualizado las descripciones para los mensajes de ayuda.

### <a name="interactive"></a>Interactive

* Se ha corregido un error de carga.

### <a name="kubernetes"></a>Kubernetes

* Se ha cambiado para usar `https` si el puerto del contenedor del panel usa `https`.

### <a name="network"></a>Red

* Se ha agregado el argumento `network dns record-set cname delete` a `--yes`.

### <a name="profile"></a>Perfil

* Se ha agregado el argumento `--resource-type` a `account get-access-token` para obtener los tokens de acceso a recursos.

### <a name="servicefabric"></a>ServiceFabric

* Se han agregado todas las versiones del sistema operativo compatible para la creación de clústeres SF.
* Se ha corregido el error de validación de certificado principal.

### <a name="storage"></a>Storage

* Se ha agregado el comando `storage copy`

## <a name="july-30-2019"></a>30 de julio de 2019

Versión 2.0.70

### <a name="acr"></a>ACR

* Se ha corregido el problema 9952 (una regresión en el comando `acr pack build`).
* Se ha quitado el nombre predeterminado de la imagen del generador en `acr pack build`.

### <a name="appservice"></a>Appservice

* Se ha cambiado `webapp config ssl` para que muestre un mensaje si no se encuentra un recurso
* Se ha corregido un problema por el que `functionapp create` no acepta el tipo de cuenta de almacenamiento `Standard_RAGRS`.
* Se ha corregido un problema por el que `webapp up` producía un error si se ejecutaba con versiones anteriores de Python.

### <a name="network"></a>Red

* Se ha quitado un parámetro no válido `--ids` de `network nic ip-config add` (corrige el problema 9861).
* Corrige el problema 9604. Se ha agregado el parámetro `--root-certs` a `network application-gateway http-settings [create|update]` para admitir los certificados raíz de confianza de los usuarios asociados.
* Se ha corregido el argumento `--subscription` para `network dns record-set ns create` (9965).

### <a name="rbac"></a>RBAC

* Se agregó el comando `user update`.
* [EN DESUSO] Se ha dejado de usar `--upn-or-object-id` en los comandos relacionados con el usuario.
    * Use el nuevo argumento `--id`.
* Se ha agregado el argumento `--id` a los comandos relacionados con el usuario.

### <a name="sql"></a>SQL

* Se han agregado comandos de administración para claves de instancia administrada y protector de TDE.

### <a name="storage"></a>Storage

* Se agregó el comando `storage remove`.
* Se ha corregido un error con `storage blob update`.

### <a name="vm"></a>máquina virtual

* Se ha cambiado `list-skus` para que use la versión más reciente de la API para generar los detalles de la zona.
* Se ha cambiado el valor predeterminado de `--single-placement-group` a `false` para `vmss create`.
* Se ha agregado la posibilidad de seleccionar SKU de almacenamiento ZRS para `[snapshot|disk] create`.
* Se ha agregado un nuevo grupo de comandos `vm host` para admitir hosts dedicados.
* Se han agregado los parámetros `--host` y `--host-group` en `vm create` para establecer un host dedicado de máquina virtual.

## <a name="july-16-2019"></a>16 de julio de 2019

Versión 2.0.69

### <a name="appservice"></a>Appservice

* Se han cambiado los comandos de `webapp identity` para devolver un mensaje de error adecuado si el nombre del grupo de recursos o la aplicación no es válido.
* Se ha corregido `webapp list` para devolver el valor correcto de numberOfSites si no se ha proporcionado ningún grupo de recursos.
* Se han corregido los efectos secundarios de `appservice plan create` y `webapp create`.

### <a name="core"></a>Core

* Se ha corregido el problema por el que `--subscription` aparecía a pesar de no ser aplicable.

### <a name="batch"></a>Batch

* [CAMBIO IMPORTANTE] Se ha reemplazado `batch pool node-agent-skus list` por `batch pool supported-images list`.
* Se ha agregado compatibilidad con las reglas de seguridad que bloquea el acceso de red a un grupo basado en el puerto de origen del tráfico cuando se usa la opción `--json-file` de `batch pool create network`.
* Agrega compatibilidad para ejecutar la tarea en el directorio de trabajo del contenedor o en el directorio de trabajo de la tarea por lotes cuando se usa la opción `--json-file` de `batch task create`.
* Se ha corregido el error en la opción `--application-package-references` de `batch pool create` por el que solo funcionaba con los valores predeterminados.

### <a name="eventhubs"></a>Event Hubs

* Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.

### <a name="rdbms"></a>RDBMS

* Se ha agregado un parámetro opcional para especificar la SKU de réplica para crear comandos de réplica.
* Se ha corregido el problema con el error de prueba de CI al crear la réplica de MySQL.

### <a name="relay"></a>Retransmisión

* Se ha corregido el problema con la conexión híbrida cuando la autorización del cliente está deshabilitada [n.º 8775](https://github.com/azure/azure-cli/issues/8775)
* Se ha agregado el parámetro `--requires-transport-security` a `relay wcfrelay create`.

### <a name="servicebus"></a>Servicebus

* Se ha agregado validación para el parámetro `--rights` de los comandos de `authorizationrule`.

### <a name="storage"></a>Storage

* Habilitar archivos AADDS para la actualización de la cuenta de almacenamiento
* Se ha corregido el problema `storage blob service-properties update --set`

## <a name="july-2-2019"></a>2 de julio de 2019

Versión 2.0.68

### <a name="core"></a>Core

* Los módulos de comandos ahora se consolidan en un único paquete distribuible de Python. Esto reemplaza el uso directo de muchos paquetes `azure-cli-` en PyPI.
  Esto reducirá el tamaño de la instalación y solo afecta a los usuarios que hayan instalado directamente mediante `pip`.

### <a name="acr"></a>ACR

* Se ha agregado compatibilidad para los desencadenadores de temporizador para las tareas.

### <a name="appservice"></a>Appservice

* Se ha cambiado `functionapp create` para habilitar Application Insights de manera predeterminada.
* [CAMBIO IMPORTANTE] Se ha dejado de utilizar el comando `functionapp devops-build`.
  *  Use el nuevo comando `az functionapp devops-pipeline` en su lugar.
* Se ha agregado compatibilidad con el plan de aplicación de funciones Consumo para Linux a `functionapp deployment config-zip`.

### <a name="cosmos-db"></a>Cosmos DB

* Se ha agregado compatibilidad para deshabilitar TTL.

### <a name="dls"></a>DLS

* Se ha actualizado la versión de ADLS (0.0.45).

### <a name="feedback"></a>Comentarios

* Al informar de un error de comando de extensión, `az feedback` ahora intenta abrir el explorador en la dirección URL del repositorio del proyecto de la extensión desde el índice.

### <a name="hdinsight"></a>HDInsight

* [CAMBIO IMPORTANTE] Se ha cambiado el nombre del grupo de comandos `oms` por `monitor`.
* [CAMBIO IMPORTANTE] Ahora `--http-password/-p` es un parámetro necesario. 
* Se han agregado completadores para los parámetros `--cluster-admin-account` y `cluster-users-group-dns`. 
* Se ha cambiado el parámetro `cluster-users-group-dns` para que sea necesario cuando `—esp` está presente.
* Se ha agregado un tiempo de espera para todos los autocompletadores de argumentos existentes.
* Se ha agregado un tiempo de espera para transformar el nombre de recurso en un identificador de recurso.
* Se han cambiado los autocompletadores para seleccionar recursos de cualquier grupo de recursos. Puede ser un grupo de recursos diferente a que se especifica con `-g`.
* Se ha agregado compatibilidad con los parámetros `--sub-domain-suffix` y `--disable_gateway_auth` en el comando `hdinsight application create`.

### <a name="managed-services"></a>Servicios administrados

* Se ha introducido un módulo de comandos de servicios administrados en versión preliminar.

### <a name="profile"></a>Perfil
* Se ha suprimido el argumento `--subscription` del comando de cierre de sesión.

### <a name="rbac"></a>RBAC

* [CAMBIO IMPORTANTE] Se ha quitado el argumento `--password` de `create-for-rbac`.
* Se ha agregado el parámetro `--assignee-principal-type` al comando `create` para evitar errores intermitentes causados por la latencia de replicación del servidor de grafos de AAD.
* Se ha corregido un bloqueo en `ad signed-in-user` al enumerar los objetos que posee.
* Se ha corregido el problema por el que `ad sp` no encontraba la aplicación correcta en una entidad de servicio.

### <a name="rdbms"></a>RDBMS

* Se ha agregado compatibilidad para la replicación a MariaDB.

### <a name="sql"></a>SQL

* Se han documentado los valores permitidos para `sql db create --sample-name`.

### <a name="storage"></a>Storage

* Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage blob generate-sas`. 
* Se ha agregado compatibilidad de los token de SAS para la delegación de usuarios con `--as-user` a `storage container generate-sas`. 

### <a name="vm"></a>máquina virtual

* Se ha corregido un error por el que `vmss create` devuelve un mensaje de error cuando se ejecuta con `--no-wait`.
* Se ha quitado la validación del lado cliente para `vmss create --single-placement-group`. No genera ningún error si `--single-placement-group` está establecido en `true` y `--instance-count` es mayor que 100 o se especifican zonas de disponibilidad, y deja esta validación al servicio de proceso.
* Se ha corregido el error por el que `[vm|vmss] extension image list` produce un error cuando se usa con `--latest`.


## <a name="june-18-2019"></a>18 de junio de 2019

Versión 2.0.67

### <a name="core"></a>Core

Esta versión introduce una nueva etiqueta [Preview] para indicar con mayor claridad a los clientes si un grupo de comandos, un comando o un argumento está en versión preliminar. Antes esto se comunicaba en el texto de ayuda o se indicaba explícitamente en el número de versión del módulo de comandos.
La CLI eliminará los números de versión de los paquetes individuales en el futuro. Si un comando está en versión preliminar, todos sus argumentos también lo están. Si un grupo de comandos está etiquetado como versión preliminar, se consideran que todos los comandos y argumentos también están en versión preliminar.

Como resultado de este cambio, pueden parecer que varios grupos de comandos están "repentinamente" en versión preliminar con esta versión. Lo que realmente ha sucede es que la mayoría de los paquetes estaban en versión preliminar, pero se considera que están disponibles con carácter general con esta versión.

### <a name="acr"></a>ACR
* Se ha agregado el comando "acr check-health".
* Mejor control de los errores para los tokens AAD y para recuperar los comandos externos.

### <a name="acs"></a>ACS
* Los comandos en desuso de ACS ya no se muestran en la vista de la ayuda.

### <a name="ams"></a>AMS
* [CAMBIO IMPORTANTE] Las cadenas de hora ISO 8601 se han cambiado para volver a archive-window-length y key-frame-interval-duration.

### <a name="appservice"></a>AppService
* Se ha agregado el enrutamiento basado en la ubicación para `webapp deleted list` y `webapp deleted restore`.
* Se ha corregido el problema por el que no se podía hacer clic la dirección URL de destino registrada de la aplicación web ("Puede iniciar la aplicación en...") en Azure Cloud Shell.
* Se ha corregido el problema por el que, al crear aplicaciones con algunas SKU, se producía un error de AlwaysOn.
* Se ha agregado validación previa a `[appservice|webapp] create`.
* Se ha corregido `[webapp|functionapp] traffic-routing` para usar el valor correcto de actionHostName.
* Se ha agregado compatibilidad con ranuras a los comandos `functionapp`.

### <a name="batch"></a>Batch
* Se ha corregido la regresión de autenticación de AAD causada por una notificación demasiado agresiva de errores de autenticación de clave compartida.

### <a name="batchai"></a>BatchAI
* Los comandos de BatchAI han dejado de usarse y están ocultos.

### <a name="botservice"></a>BotService
* Se ha agregado un aviso de advertencia "compatibilidad descontinuada" o "modo de mantenimiento" a los comandos que admiten el SDK v3.

### <a name="cosmosdb"></a>CosmosDB
* [EN DESUSO] Se ha dejado de usar el comando `cosmosdb list-keys`.
* Se ha agregado el comando `cosmosdb keys list`, que reemplaza a `cosmosdb list-keys`.
* `cosmsodb create/update`: Se ha agregado el nuevo formato a --location para poder establecer la propiedad "isZoneRedundant". Formato antiguo en desuso.

### <a name="eventgrid"></a>EventGrid
* Se han agregado comandos `eventgrid domain` para las operaciones CRUD de dominios.
* Se han agregado comandos `eventgrid domain topic` para las operaciones CRUD de temas de dominio.
* Se ha agregado el argumento `--odata-query` a `eventgrid [topic|event-subscription] list` para filtrar los resultados mediante la sintaxis de OData.
* `event-subscription create/update`: Se ha agregado servicebusqueue como nuevos valores para el parámetro `--endpoint-type`.
* [CAMBIO IMPORTANTE] Se ha quitado la compatibilidad para `--included-event-types All` con `eventgrid event-subscription [create|update]`.

### <a name="hdinsight"></a>HDInsight
* Se ha agregado compatibilidad con el parámetro `--ssh-public-key` al comando `hdinsight create`.

### <a name="iot"></a>IoT
* Se ha agregado compatibilidad para volver a generar las claves de directiva de autorización.
* Se ha agregado un SDK y compatibilidad con el servicio de aprovisionamiento de repositorio de DigitalTwin.

### <a name="network"></a>Red
* Se ha agregado compatibilidad de las zonas con puertas de enlace NAT.
* Se ha agregado el comando `network list-service-tags`
* Se ha corregido el problema con `dns zone import` por el que los usuarios no podían importar registros A con caracteres comodín.
* Se ha corregido el problema con `watcher flow-log configure` por el que no se podía habilitar el registro de flujos en determinadas regiones.

### <a name="resource"></a>Resource
* Se ha agregado el comando `az rest` para hacer llamadas de REST.
* Se ha corregido el error al usar `policy assignment list` con un grupo de recursos o un nivel de suscripción `--scope`.

### <a name="servicebus"></a>ServiceBus
* Se ha corregido el error con `servicebus topic create --max-size` [9319](https://github.com/azure/azure-cli/issues/9319).

### <a name="sql"></a>SQL
* Se ha cambiado `--location` para que sea opcionalpara `sql [server|mi] create`; usa la ubicación del grupo de recursos si no se especifica.
* Se ha corregido el error "No se puede iterar en el objeto NoneType" para `sql db list-editions --available`.

### <a name="sqlvm"></a>SQLVm
* [CAMBIO IMPORTANTE] Se ha cambiado `sql vm create` para requerir el parámetro `--license-type`.
* Se ha cambiado para poder establecer el SKU de la imagen de SQL al crear o actualizar una máquina virtual de SQL.

### <a name="storage"></a>Storage
* Se ha corregido un problema con una clave de cuenta que falta para `storage container generate-sas`.
* Se ha corregido un problema con `storage blob sync` en Linux.

### <a name="vm"></a>máquina virtual
* [VERSIÓN PRELIMINAR] Se han agregado los comandos `vm image template` para compilar imágenes de máquina virtual.

## <a name="june-4-2019"></a>4 de junio de 2019

Versión 2.0.66

### <a name="core"></a>Core
* Se ha corregido el problema por el que los comandos generan un error si `--output yaml` se usa con `--query`.

### <a name="acr"></a>ACR
* Se ha agregado el grupo de comandos "acr pack" para crear tareas de compilación rápida mediante Buildpacks.

### <a name="acs"></a>ACS
* Se permite habilitar o deshabilitar el complemento kube-dashboard de AKS.
* Se imprime un mensaje descriptivo cuando la suscripción no está en la lista de permitidos para usar Azure Red Hat OpenShift.

### <a name="batch"></a>Batch
* Se ha mejorado el control de errores cuando no se ha iniciado sesión en una cuenta \[[9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[8978](https://github.com/Azure/azure-cli/issues/8978)\].

### <a name="iot"></a>IoT
* Se ha agregado compatibilidad para la conmutación por error manual.

### <a name="network"></a>Red
* Se han agregado comandos `network application-gateway waf-policy` para admitir reglas personalizadas de WAF.
* Se agregaron los argumentos `--waf-policy` y `--max-capacity` a `network application-gateway [create|update]` 

### <a name="resource"></a>Resource
* Se ha mejorado el mensaje de error de `deployment create` cuando TTY no está disponible.

### <a name="role"></a>Role
* Texto de ayuda actualizado.

### <a name="compute"></a>Proceso
* Se ha agregado compatibilidad a `vm create` para máquinas virtuales desde una imagen administrada con LUN de discos de datos que no comienzan en 0 o que omiten los números.

## <a name="may-21-2019"></a>21 de mayo de 2019

Versión 2.0.65

### <a name="core"></a>Core
* Se han agregado mejores comentarios para los errores de autenticación.
* Se ha corregido un problema por el que la CLI cargaba extensiones que no eran compatibles con su versión principal.
* Se ha corregido un problema con el inicio cuando `clouds.config` estaba dañado.

### <a name="acr"></a>ACR
* Se ha agregado compatibilidad para identidades administradas a Tareas.

### <a name="acs"></a>ACS
* Se ha corregido el comando `openshift create` cuando se usa con el cliente AAD.

### <a name="appservice"></a>AppService
* [EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`; se quitará en la próxima versión.
* Se ha cambiado `functionapp devops-pipeline` para recopilar el registro de compilación de Azure DevOps en modo detallado.
* [CAMBIO IMPORTANTE] Se ha eliminado la marca `--use_local_settings` del comando `functionapp devops-pipeline`; no era operativa.
* Se ha cambiado `webapp up` para que devuelva la salida JSON si no se usa `--logs`.
* Se ha agregado compatibilidad para escribir los recursos predeterminados en la configuración local para `webapp up`.
* Se ha agregado compatibilidad para `webapp up` para volver a implementar una aplicación sin usar el argumento `--location`.
* Se ha corregido un problema por el que, al crear un ASP en la SKU gratuita de Linux, el valor de SKU "Fee" no funcionaba.

### <a name="botservice"></a>BotService
* Se ha cambiado para permitir las mayúsculas y minúsculas para los parámetros `--lang` de los comandos.
* Se ha actualizado la descripción para el módulo de comandos.

### <a name="consumption"></a>Consumo
* Se ha agregado un parámetro obligatorio que faltaba al ejecutar `consumption usage list --billing-period-name`.

### <a name="iot"></a>IoT
* Se ha agregado compatibilidad para enumerar todas las claves.

### <a name="network"></a>Red
* [CAMBIO IMPORTANTE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* Se ha agregado el argumento `--nat-gateway` a `network vnet subnet [create|update]` para adjuntar a una puerta de enlace NAT.
* Se ha corregido el problema con `dns zone import` por el que los nombres de registro no encontraban un tipo de registro.

### <a name="rdbms"></a>RDBMS
* Se ha agregado compatibilidad con replicación geográfica a mysql y postgres.

### <a name="rbac"></a>RBAC
* Se ha agregado compatibilidad para el ámbito de grupos de administración a `role assignment`.

### <a name="storage"></a>Storage
* `storage blob sync`: se ha agregado el comando sync a Blob Storage.

### <a name="compute"></a>Proceso
* Se ha agregado `--computer-name` a `vm create` para establecer el nombre de equipo de una máquina virtual.
* Se ha cambiado el nombre de `--ssh-key-value` a `--ssh-key-values` para `[vm|vmss] create`; ahora pueden aceptar varios valores ssh de clave pública o rutas de acceso.
  * __Nota__: Este **no** es un cambio importante. `--ssh-key-value` se analizará correctamente porque solo coincide con `--ssh-key-values`.
* Se ha cambiado el argumento `--type` de `ppg create` para que sea opcional.

## <a name="may-6-2019"></a>6 de mayo de 2019

Versión 2.0.64

### <a name="acs"></a>ACS
* [CAMBIO IMPORTANTE] Se ha eliminado la marca `--fqdn` de los comandos `openshift`.
* Se ha cambiado para usar la versión GA de la API Openshift de Azure Red Hat.
* Se ha agregado la marca `customer-admin-group-id` a `openshift create`.
* [GA] Se ha quitado `(PREVIEW)` de la opción `--network-policy` de `aks create`.

### <a name="appservice"></a>Appservice
* [EN DESUSO] Se ha dejado de usar el comando `functionapp devops-build`.
  * Se ha cambiado el nombre a `functionapp devops-pipeline`.
* Se ha corregido un error por el que no se podía obtener el nombre de usuario correcto para cloudshell, lo que provocaba un error de `webapp up`.
* Se ha actualziado la documentación de `appservice plan --sku` para incluir la compatibilidad con appserviceplans.
* Se han agregado argumentos opcionales para el grupo de recursos y el plan a `webapp up`.
* Se ha agregado compatibilidad a `webapp ssh` para respetar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.
* Se ha agregado compatibilidad a `appserviceplan create` con la SKU gratuita de Linux.
* Se ha cambiado `webapp up` para que haya una suspensión de 30 segundos después de configurar la opción `SCM_DO_BUILD_DURING_DEPLOYMENT=true` para controlar el inicio en frío de kudu.
* Se ha agregado compatibilidad con el entorno de ejecución `powershell` a `functionapp create` en Windows.
* Se agregó el comando `create-remote-connection`.

### <a name="batch"></a>Batch
* Se ha corregido un error en el validador para las opciones de `--application-package-references`.

### <a name="botservice"></a>Botservice
* [CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para crear un bot de Web App vacío de forma predeterminada (es decir, el bot no se implementa en App Service).
* Se ha agregado la marca `--echo` a `bot create` para usar el comportamiento anterior con `-v v4`.
* [CAMBIO IMPORTANTE] Se ha cambiado el valor predeterminado de `--version` a `v4`.
  * __NOTA:__ `bot prepare-publish` sigue usando el valor predeterminado anterior.
* [CAMBIO IMPORTANTE] Se ha cambiado `--lang` para que su valor predeterminado ya no sea `Csharp`. Si el comando requiere `--lang` y no se proporciona, ahora producirá un error.
* [CAMBIO IMPORTANTE] Se han cambiado los argumentos `--appid` y `--password` de `bot create` para que sean necesarios y ahora se pueden crear mediante `ad app create`.
* Se ha agregado la validación de `--appid` y `--password`.
* [CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4` para que no cree ni use una cuenta de almacenamiento ni Application Insights.
* [CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v3` para que requiera una región donde esté disponible Application Insights.
* [CAMBIO IMPORTANTE] Se ha cambiado `bot update` para que ahora afecte solo a determinadas propiedades de un bot.
* [CAMBIO IMPORTANTE] Se han cambiado las marcas `--lang` para que acepten `Javascript` en lugar de `Node`.
* [CAMBIO IMPORTANTE] Se ha quitado `Node` como valor de `--lang` permitido.
* [CAMBIO IMPORTANTE] Se ha cambiado `bot create -v v4 -k webapp` para que no establezca `SCM_DO_BUILD_DURING_DEPLOYMENT` en true. Todas las implementaciones a través de Kudu actuarán según su comportamiento predeterminado.
* Se ha cambiado `bot download` para los bots sin archivos `.bot` para crear el archivo de configuración específico del idioma con los valores de Application Insights para el bot.
* Se ha agregado compatibilidad de `Typescript` con `bot prepare-deploy`
* Se ha agregado un mensaje de advertencia a `bot prepare-deploy` para los bots `Javascript` y `Typescript` cuando `--code-dir` no contiene `package.json`.
* Se ha cambiado `bot prepare-deploy` para que devuelva `true` si es correcto.
* Se ha agregado el registro detallado a `bot prepare-deploy`.
* Se han agregado regiones más disponibles de Application Insights a `az bot create -v v3`.

### <a name="configure"></a>Configuración
* Se ha agregado compatibilidad para configuraciones de valores predeterminados de argumentos basadas en carpetas.

### <a name="eventhubs"></a>Event Hubs
* Se agregaron los comandos `namespace network-rule`.
* Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.

### <a name="network"></a>Red
* [CAMBIO IMPORTANTE] Se ha reemplazado el argumento `--cache` con `--defer` para `vnet [create|update]`. 

### <a name="policy-insights"></a>Información de directiva
* Se ha agregado compatibilidad a `--expand PolicyEvaluationDetails` para consultar detalles de evaluación de directivas en el recurso.

### <a name="role"></a>Role
* [EN DESUSO] Se ha cambiado el argumento `create-for-rbac` hide '--password' y se dejará de dar soporte en mayo de 2019.

### <a name="service-bus"></a>Azure Service Bus
* Se agregaron los comandos `namespace network-rule`.
* Se ha agregado el argumento `--default-action` para reglas de red a `namespace [create|update]`.
* Se ha corregido `topic [create|update]` para que `--max-size` permita valores de 10, 20, 40 y 80 GB con SKU Premium.

### <a name="sql"></a>SQL
* Se agregaron los comandos `sql virtual-cluster [list|show|delete]`.

### <a name="vm"></a>máquina virtual
* Se ha agregado `--protect-from-scale-in` y `--protect-from-scale-set-actions` a `vmss update` para habilitar las actualizaciones a la directiva de protección de instancias de máquina virtual de VMSS.
* Se ha agregado `--instance-id` a `vmss update` para habilitar la actualización genérica de instancias de máquina virtual de VMSS.
* Se ha agregado `--instance-id` a `vmss wait`
* Se ha agregado un nuevo grupo de comandos `ppg` para administrar grupos de ubicación de proximidad.
* Se ha agregado `--ppg` a `[vm|vmss] create` y `vm availability-set create` para administrar grupos de ubicación de proximidad.
* Se ha agregado el parámetro `--hyper-v-generation` a `image create`

## <a name="april-23-2019"></a>23 de abril de 2019

Versión 2.0.63

### <a name="acs"></a>ACS
* Se ha cambiado `aks get-credentials` para que pregunte si se desean sobrescribir los valores duplicados.
* Se ha quitado `(PREVIEW)` de los comandos de DevSpaces "aks use-dev-spaces" y "aks remove-dev-spaces".

### <a name="ams"></a>AMS
* Se ha corregido un error con la actualización de los filtros de cuenta y recursos.

### <a name="appservice"></a>AppService
* Se ha agregado compatibilidad para ASE y un tiempo de espera a `webapp ssh`.
* Se ha agregado compatibilidad para establecer la integración e implementación continuas a una canalización de Azure DevOps desde un repositorio de Github para aplicaciones de función.
* Se ha agregado el argumento `--github-pat` a `functionapp devops-build create` para aceptar el token de acceso personal de Github.
* Se ha agregado el argumento `--github-repository` a `functionapp devops-build create` para aceptar el repositorio de Github que contiene un código de origen de aplicación de función.
* Se ha corregido el problema por el que `az webapp up --logs` producía un error y actualizaba .NETCORE a la versión 2.1 de forma predeterminada.
* Se han quitado las opciones de configuración de aplicaciones de función innecesarias a la hora de crear una aplicación de función con un plan de consumo.
* Se ha cambiado `webapp up` para que la cadena asp predeterminada ahora anexe el número al final para crear un nuevo ASP según las opciones de SKU.
* Se ha agregado `-b` como opción a `webapp up` para iniciar la aplicación en el explorador.
* Se ha cambiado `webapp deployment source config zip` para controlar la variable de entorno `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.

### <a name="deployment-manager"></a>Administrador de implementaciones
* [VERSIÓN PRELIMINAR] Creación y administración de artefactos que admiten lanzamientos.

### <a name="lab"></a>Laboratorio
* Se ha corregido el error que provocaba una salida prematura.

### <a name="network"></a>Red
* Se ha agregado la delegación de servidor nombre automática a `dns zone create` en la zona primaria durante la creación de una zona secundaria.

### <a name="resource"></a>Resource
* [EN DESUSO] Se han dejado de usar los argumentos `--link-id`, `--target-id` y `--filter-string` de `resource link`.
  * En su lugar, use los argumentos `--link`, `--target` y `--filter`.
* Se ha corregido el problema por el que los comandos `resource link [create|update]` no funcionaban.
* Se ha corregido un problema por el que se podía producir un problema al eliminar utilizando un identificador de recurso.

### <a name="sql"></a>SQL
* Se ha agregado compatibilidad para zonas horarias personalizadas en instancias administradas.
* Se ha cambiado para poder usar un nombre de grupo elástico con `sql db update`.
* Se ha agregado compatibilidad de `--no-wait` con `sql server [create|update]`
* Se ha agregado el comando `sql server wait`

### <a name="storage"></a>Storage
* Se ha corregido un problema con los tokens de SAS de codificación doble en `storage blob generate-sas`.

### <a name="vm"></a>máquina virtual
* Se ha agregado la marca `--skip-shutdown` a `vm|vmss stop` para apagar las máquinas virtuales sin cerrarlas.
* Se ha agregado el argumento `--storage-account-type` a `sig image-version create` para establecer el tipo de cuenta del perfil de publicación.
* Se ha agregado el argumento `--target-regions` a `sig image-version create` para permitir tipos de cuenta de almacenamiento específicos de la región.

## <a name="april-9-2019"></a>9 de abril de 2019

### <a name="core"></a>Core
* Se ha corregido el problema por el que algunas extensiones mostraban una versión `Unknown` y no se podían actualizar.

### <a name="acr"></a>ACR
* Se ha agregado compatibilidad con la ejecución de una imagen sin contexto.

### <a name="ams"></a>AMS
* [EN DESUSO]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [CAMBIO IMPORTANTE]: Renamed the `--bitrate` parameter to `--first-quality`
* Se ha agregado compatibilidad con nuevos parámetros de cifrado a `ams streaming-policy create`.
* Se ha agregado un nuevo parámetro `--filters` a `ams streaming-locator create`.

### <a name="appservice"></a>AppService
* Se ha agregado compatibilidad de `--logs` con `webapp up`
* En el comando `functionapp devops-build create`, se han corregido los problemas de generación de `azure-pipelines.yml`
* Se ha mejorado el control de errores y los indicadores de `unctionapp devops-build create`
* [CAMBIO IMPORTANTE] Se ha quitado la marca `--local-git` del comando `devops-build`; la detección y administración del repositorio git local son obligatorias para crear canalizaciones de Azure DevOps
* Se ha agregado compatibilidad para crear planes de funciones Linux
* Se ha agregado la posibilidad de cambiar el plan de una aplicación de función mediante `functionapp update --plan`.
* Se ha agregado compatibilidad para las opciones de escalado horizontal del plan Premium de Azure Functions

### <a name="cdn"></a>CDN
* Se ha agregado compatibilidad para `Microsoft_Standard` y `Standard_ChinaCdn`.

### <a name="feedback"></a>Comentarios
* Se ha cambiado `feedback` para mostrar los metadatos de los comandos ejecutados recientemente
* Se ha cambiado `feedback` para pedir al usuario que abra un explorador y use una plantilla de incidencia para ayudar en el proceso de creación de la incidencia
* Se ha cambiado `feedback` para imprimir el cuerpo de la incidencia cuando se ejecuta con "--verbose"

### <a name="monitor"></a>Supervisión
* Se ha corregido un problema por "count" no era un valor permitido en `metrics alert [create|update]`. 

### <a name="network"></a>Red
* Se ha corregido el formato de tabla que no se mostraba con `vnet-gateway list-bgp-peer-status`.
* Se han agregado los comandos `list-request-headers` y `list-response-headers` a `application-gateway rewrite-rule`.
* Se ha agregado el comando `list-server-variables` a `application-gateway rewrite-rule condition`.
* Se ha corregido un problema por el que actualización del estado de un vínculo en un puerto de express-route generaba una excepción de atributo desconocido `express-route port update`.

### <a name="privatedns"></a>PrivateDNS
* Se ha agregado `network private-dns` para zonas DNS privadas

### <a name="resource"></a>Resource
* Se ha corregido el problema con `deployment create` y `group deployment create` por el que no funcionaba un archivo de parámetros con un conjunto de parámetros vacío

### <a name="role"></a>Role
* Se ha corregido `create-for-rbac` para que trate `--years` correctamente
* [CAMBIO IMPORTANTE] Se ha cambiado `role assignment delete` para preguntar cuando se eliminan todas las asignaciones de la suscripción de forma incondicional

### <a name="sql"></a>SQL
* Se ha actualizado `sql mi [create|update]` con las propiedades proxyOverride y publicDataEndpointEnabled

### <a name="storage"></a>Storage
* [CAMBIO IMPORTANTE] Se ha quitado el resultado de `storage blob delete`.
* Se ha agregado `--full-uri` a `storage blob generate-sas` para crear el URI completo para el blob con SAS
* Se ha agregado `--file-snapshot` a `storage file copy start` para copiar el archivo desde la instantánea
* Se ha cambiado `storage blob copy cancel` para mostrar solo el error en lugar de la excepción para NoPendingCopyOperation

## <a name="march-26-2019"></a>26 de marzo de 2019


### <a name="core"></a>Core
* Se han corregido problemas con la incompatibilidad de la extensión de desarrollo.
* El control de errores ahora dirige a los clientes a la página de problemas.

### <a name="cloud"></a>Nube
* Se ha corregido un error de "suscripción no encontrada" en `cloud set`.

### <a name="acr"></a>ACR
* Se han corregido orígenes redundantes en la importación de imágenes.
* Se ha agregado `--auth-mode` a los comandos `acr build`, `acr run`, `acr task create` y `acr task update`.
* Se ha agregado el grupo de comandos "acr task credential" para administrar las credenciales de una tarea.
* Se ha agregado "--no-wait" al comando `acr build`.

### <a name="appservice"></a>AppService
* Se ha corregido el error por el que `webapp up` no controlaba correctamente los escenarios de ejecución desde un directorio o de código desconocido.
* Se ha corregido el error por el que los espacios no funcionaban para `[webapp|functionapp] config ssl bind`.

### <a name="bot-service"></a>Servicio BOT
* Se ha agregado `bot prepare-deploy` para preparar la implementación de bots mediante `webapp`.
* Se ha cambiado `bot create --kind registration` para que muestre la contraseña si no se proporciona una.
* [CAMBIO IMPORTANTE] Se ha cambiado `--endpoint` en `bot create --kind registration` a que sea una cadena vacía de forma predeterminada en lugar de que sea obligatorio.
* Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.

### <a name="cdn"></a>CDN
* Se agregó compatibilidad para `--no-wait` a `cdn endpoint [create|update|start|stop|delete|load|purge]`.  
* [CAMBIO IMPORTANTE] Se ha cambiado el comportamiento de almacenamiento de cadenas de consulta en caché predeterminado de `cdn endpoint create`. El valor predeterminado ya no es "IgnoreQueryString". Ahora lo establece el servicio

### <a name="cosmosdb"></a>Cosmosdb
* Se ha agregado compatibilidad con `--enable-multiple-write-locations` al actualizar la cuenta.
* Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.

### <a name="interactive"></a>Interactive
* Se ha corregido la incompatibilidad con la extensión interactiva instalada mediante azdev.

### <a name="monitor"></a>Supervisión
* Se ha cambiado para permitir el valor de dimensión `*` para `monitor metrics alert [create|update]`.

### <a name="network"></a>Red
* Se ha agregado el grupo de comandos `rewrite-rule` a `application-gateway`.

### <a name="profile"></a>Perfil
* Se ha agregado a `login` compatibilidad de la cuenta en el nivel de inquilino para la identidad de servicio administrada.

### <a name="postgres"></a>Postgres 
* Se han agregado los comandos postgresql `replica` y el comando `restart server`.
* Se ha cambiado para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.

### <a name="resource"></a>Resource
* Se ha mejorado la salida de tabla de `deployment [create|list|show]`.
* Se ha corregido el problema con `deployment [create|validate]` por el que no reconocía el tipo secureObject.

### <a name="graph"></a>Grafo
* Se agregó compatibilidad para `--end-date` a `ad [app|sp] credential reset`.
* Se ha agregado compatibilidad para agregar permisos con `ad app permission add`.
* Se ha corregido un error con `ad app permission list` cuando no había ningún permiso.
* Se ha cambiado `ad sp delete` para omitir la eliminación de la asignación de roles si la cuenta actual no tiene ninguna suscripción.
* Se ha cambiado `ad app create` para que `--identifier-uris` sea una lista vacía de forma predeterminada si no se proporciona.

### <a name="storage"></a>storage
* Se ha agregado `--snapshot` a `storage file download-batch` para descargar desde una instantánea de recurso compartido.
* Se ha cambiado la barra de progreso `storage blob [download-batch|upload-batch]` para que sea menos detallada y que indique el blob actual.
* Se ha corregido el problema con `storage account update` al actualizar los parámetros de cifrado.
* Se ha corregido el problema por el que `storage blob show` producía un error al usar oauth (`--auth-mode=login`).

### <a name="vm"></a>máquina virtual
* Se agregó el comando `image update`.

## <a name="march-12-2019"></a>12 de marzo de 2019

Versión 2.0.60

### <a name="core"></a>Core

* Se ha corregido un error incorrecto en `cloud set` sobre la suscripción no encontrada.

### <a name="acr"></a>ACR

* Se han corregido orígenes redundantes en la importación de imágenes.

### <a name="acs"></a>ACS

* Ahora, se omite el parámetro `--listen-address` de `aks browse` si kubectl no lo admite 

### <a name="appservice"></a>AppService

* Se ha agregado `[webapp|functionapp] deployment list-publishing-credentials` para obtener la dirección URL y sus credenciales de publicación de Kudu.
* Se ha quitado la instrucción de impresión errónea para `webapp auth update`.
* Se ha corregido `functionapp` para establecer la imagen correcta en el entorno de ejecución en los planes de App Service de Linux
* Se ha quitado la etiqueta de versión preliminar para `webapp up` y se han agregado mejoras al comando.

### <a name="botservice"></a>Botservice

* Se ha agregado `SCM_DO_BUILD_DURING_DEPLOYMENT` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web.
* Se han agregado `Microsoft-BotFramework-AppId` y `Microsoft-BotFramework-AppPassword` a la configuración de la aplicación de la plantilla de ARM para la versión 4 de bots de aplicación web
* Se han quitado las comillas simples de la salida del comando `bot publish` al final de `bot create`.
* Se ha cambiado `bot publish` para que sea asincrónico.

### <a name="container"></a>Contenedor

* Se agregó el argumento `--no-wait` a `container [start|restart]`

### <a name="eventhub"></a>EventHub

* Se ha agregado la marca `--skip-empty-archives` a `eventhub create|update` para admitir archivos vacíos en la captura.

### <a name="find"></a>Buscar

* Actualización de la funcionalidad principal

### <a name="hdinsight"></a>HDInsight

* Se ha agregado el parámetro `--storage-account-managed-identity` a `hdinsight create` para admitir MSI de ADLS Gen2.

### <a name="network"></a>Red

* Se ha corregido un problema con `vpn-connection update` por el que no se podía actualizar una conexión VPN entre pasarelas de diferentes suscripciones.

### <a name="rdbms"></a>Rdbms

* Correcciones menores para obtener la ubicación predeterminada del grupo de recursos cuando no se proporciona para la creación de servidores y agregar validación para los días de retención.

### <a name="role"></a>Role

* Se ha corregido `role definition update` para usar el identificador para resolver la definición correctamente.
* Se ha cambiado `ad app credential reset` para eliminar la suposición de que la entidad de servicio de la aplicación siempre existe.

### <a name="service-fabric"></a>Service Fabric

* Se ha corregido un problema con `sf cluster list` que no se podía iterar.

## <a name="february-26-2019"></a>26 de febrero de 2019

Versión 2.0.59

### <a name="core"></a>Core

* Se ha corregido un problema por el que en algunos casos el uso de `--subscription NAME` generaba una excepción.

### <a name="acr"></a>ACR

* Se ha agregado el parámetro `--target` a los comandos `acr build`, `acr task create` y `acr task update`.
* Se ha mejorado el control de errores para los comandos del entorno de ejecución cuando no se ha iniciado sesión en Azure.

### <a name="acs"></a>ACS

* Se agregó la opción `--listen-address` a `aks port-forward`

### <a name="appservice"></a>AppService

* Se agregó el comando `functionapp devops-build`.

### <a name="batch"></a>Batch
* [CAMBIO IMPORTANTE] Se ha eliminado el comando `batch pool upgrade os`.
* [CAMBIO IMPORTANTE] Se ha quitado la propiedad `Pacakges` desde las respuestas `Application`.
* Se ha agregado el comando `batch application package list` a la lista de paquetes de una aplicación.
* [CAMBIO IMPORTANTE] Se ha cambiado `--application-id` a `--application-name` en todos los comandos `batch application`. 
* Se ha agregado el argumento `--json-file` a los comandos para solicitar la respuesta de la API sin formato.
* Se ha actualizado la validación para incluir automáticamente `https://` en todos los puntos de conexión si falta.

### <a name="cosmosdb"></a>CosmosDB

* Se ha agregado el subgrupo `network-rule` con los comandos `add`, `remove` y `list` para administrar las reglas de la red virtual de una cuenta de Cosmos DB.

### <a name="kusto"></a>Kusto

* [CAMBIO IMPORTANTE] Se han cambiado los tipos `hot_cache_period` y `soft_delete_period` para la base de datos al formato de duración ISO8601.

### <a name="network"></a>Red

* Se agregó el argumento `--express-route-gateway-bypass` a `vpn-connection [create|update]`
* Se han agregado grupos de comandos desde extensiones `express-route`.
* Se han agregado los grupos de comandos `express-route gateway` y `express-route port`.
* Se agregó el argumento `--legacy-mode` a `express-route peering [create|update]` 
* Se han agregado los argumentos `--allow-classic-operations`, `--express-route-port` a `express-route [create|update]`.
* Se agregó el argumento `--gateway-default-site` a `vnet-gateway [create|update]`
* Se han agregado comandos `ipsec-policy` a `vnet-gateway`.

### <a name="resource"></a>Resource

* Se ha corregido el problema con `deployment create` en el que el campo de tipo distinguía entre mayúsculas y minúsculas.
* Se ha agregado compatibilidad para el archivo de parámetros basado en URI a `policy assignment create`.
* Se ha agregado compatibilidad para definiciones y parámetros basados en URI para `policy set-definition update`.
* Se ha corregido el control de parámetros y reglas para `policy definition update`.
* Se ha corregido un problema con `resource show/update/delete/tag/invoke-action` por el que los identificadores entre suscripciones no respectaban correctamente con el identificador de suscripción.

### <a name="role"></a>Role

* Se ha agregado compatibilidad con roles de aplicación a `ad app [create|update]`

### <a name="vm"></a>máquina virtual

* Se ha corregido un problema con `vm create where `--acelerated-networking` que no estaba habilitado de forma predeterminada para Ubuntu 18.0.

## <a name="february-12-2019"></a>12 de febrero de 2019

Versión 2.0.58

### <a name="core"></a>Core

* `az --version` ahora muestra una notificación si tiene paquetes que se pueden actualizar.
* Se ha corregido la regresión por la que `--ids` no podía usarse con la salida JSON.

### <a name="acr"></a>ACR
* [CAMBIO IMPORTANTE] Se ha eliminado el grupo de comandos `acr build-task`.
* [CAMBIO IMPORTANTE] Se han quitado las opciones `--tag` y `--manifest` de `acr repository delete`.

### <a name="acs"></a>ACS
* Se ha agregado compatibilidad a `aks [enable-addons|disable-addons]` para que no distinga mayúsculas y minúsculas en los nombres.
* Se ha agregado compatibilidad para la operación de actualización de Azure Active Directory mediante `aks update-credentials --reset-aad`.
* Se ha incluido una aclaración de que `--output` se omite para `aks get-credentials`.

### <a name="ams"></a>AMS
* Se agregaron los comandos `ams streaming-endpoint [start | stop | create | update] wait`.
* Se agregaron los comandos `ams live-event [create | start | stop | reset] wait`.

### <a name="appservice"></a>Appservice
* Se ha agregado la posibilidad de crear y configurar funciones mediante contenedores de ACR.
* Se ha agregado compatibilidad para actualizar las configuraciones de las aplicaciones web mediante JSON.
* Se ha mejorado la ayuda de `appservice-plan-update`.
* Se ha agregado compatibilidad para App Insights al crear una aplicación de función.
* Se han corregido los problemas de SSH con las aplicaciones web.

### <a name="botservice"></a>Botservice
* Se ha mejorado la experiencia de usuario de `bot publish`.
* Se ha agregado una advertencia de tiempo de espera agotado cuando se ejecuta `npm install` durante `az bot publish`.
* Se han quitado caracteres no válidos `.` de `--name` en `az bot create`.
* Se ha dejado de generar nombres de recursos aleatorios al crear almacenamiento de Azure Storage, planes de App Service, funciones o aplicaciones web y recursos de Application Insights.
* [EN DESUSO] Se ha dejado de utilizar el argumento `--proj-name` en favor de `--proj-file-path`.
* Se ha cambiado `az bot publish` para quitar los archivos de implementación IIS de Node.js capturados si ya no existen.
* Se ha agregado el argumento `--keep-node-modules` a `az bot publish` para no eliminar la carpeta `node_modules` en App Service.
* Se ha agregado el par clave-valor `"publishCommand"` a la salida de `az bot create` al crear una función o un bot de aplicación web de Azure.
  * El valor de `"publishCommand"` es un comando `az bot publish` rellenado previamente con los parámetros necesarios para publicar el bot recién creado.
* Se ha actualizado `"WEBSITE_NODE_DEFAULT_VERSION"` en la plantilla ARM para que los bots del SDK v4 usen la versión 10.14.1 en lugar de la versión 8.9.4.

### <a name="key-vault"></a>Key Vault
* Se ha corregido el problema con `keyvault secret backup` por el que algunos usuarios recibían un error `unexpected_keyword` cuando usaban `--id`.

### <a name="monitor"></a>Supervisión
* Se ha cambiado `monitor metrics alert [create|update]` para permitir el valor de dimensión `*`.

### <a name="network"></a>Red
* Se ha cambiado `dns zone export` para asegurarse de que los valores de CNAME exportados sean nombres de dominio completos.
* Se ha agregado el parámetro `--gateway-name` a `nic ip-config address-pool [add|remove]` para admitir grupos de direcciones de back-end de puerta de enlace de aplicaciones.
* Se han agregado los argumentos `--traffic-analytics` y `--workspace` a `network watcher flow-log configure` para admitir el análisis de tráfico mediante un área de trabajo de Log Analytics.
* Se ha agregado `--idle-timeout` y `--floating-ip` a `lb inbound-nat-pool [create|update]`.

### <a name="policy-insights"></a>Información de directiva
* Se han agregado los comandos `policy remediation` para admitir las características de corrección de directivas de recursos.

### <a name="rdbms"></a>RDBMS
* Se han mejorado los parámetros de mensajes y comandos de ayuda.

### <a name="redis"></a>Redis
* Se han agregado comandos para administrar reglas de firewall (crear, actualizar, eliminar, mostrar y enumerar).
* Se han agregado comandos para administrar vínculos de servidor (crear, eliminar, mostrar y enumerar).
* Se han agregado comandos para administrar programaciones de revisiones (crear, actualizar, eliminar y mostrar).
* Se ha agregado compatibilidad con zonas de disponibilidad y versión de TLS mínima a "redis create".
* [CAMBIO IMPORTANTE] Se han eliminado los comandos `redis update-settings` y `redis list-all`.
* [CAMBIO IMPORTANTE] El parámetro "tenant settings" de `redis create` no se acepta en con el formato clave[=valor].
* [EN DESUSO] Se ha agregado el mensaje de advertencia de desuso del comando `redis import-method`.

### <a name="role"></a>Role
* [CAMBIO IMPORTANTE] Se ha movido el comando `az identity` aquí desde los comandos `vm`.

### <a name="sql-vm"></a>VM con SQL
* [EN DESUSO] Se ha dejado de usar el argumento `--boostrap-acc-pwd` debido a un error de escritura.

### <a name="vm"></a>máquina virtual
* Se ha cambiado `vm list-skus` para poder usar `--all` en lugar de `--all true`.
* Se agregó `vmss run-command [invoke | list | show]`.
* Se ha corregido el error por el que `vmss encryption enable` producía un error si se ejecutaba previamente.
* [CAMBIO IMPORTANTE] Se ha movido el comandos `az identity` a los comandos `role`.

## <a name="january-31-2019"></a>31 de enero de 2019

Versión 2.0.57

### <a name="core"></a>Core

* Corrección para el [problema 8399](https://github.com/Azure/azure-cli/issues/8399).

## <a name="january-28-2019"></a>28 de enero de 2019

Versión 2.0.56

### <a name="acr"></a>ACR
* Se ha agregado compatibilidad con las reglas de red virtual o dirección IP.

### <a name="acs"></a>ACS
* Se ha agregado la versión preliminar de nodos virtuales.
* Se han agregado comandos OpenShift administrados.
* Se ha agregado compatibilidad para la operación de actualización de la entidad de servicio con `aks update-credentials -reset-service-principal`.

### <a name="ams"></a>AMS
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams asset get-streaming-locators` a `ams asset list-streaming-locators`
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `ams streaming-locator get-content-keys` a `ams streaming-locator list-content-keys`

### <a name="appservice"></a>Appservice
* Se ha agregado compatibilidad para App Insights en `functionapp create`.
* Se ha agregado a las aplicaciones de función compatibilidad para la creación de planes de App Service (includo el plan Premium Elástico).
* Se han corregido los problemas de configuración de aplicaciones con los planes Premium Elástico.

### <a name="container"></a>Contenedor
* Se agregó el comando `container start`.
* Se ha cambiado para poder usar valores decimales de la CPU durante la creación de contenedores.

### <a name="eventgrid"></a>EventGrid
* Se ha agregado el parámetro `--deadletter-endpoint` a `event-subscription [create|update]`
* Se han agregado storagequeue y hybridconnection como nuevos valores para "event-subscription [create|update] --endpoint-type".
* Se han agregado los parámetros `--max-delivery-attempts` y `--event-ttl` a `event-subscription create` para especificar la directiva de reintentos para los eventos.
* Se ha agregado un mensaje de advertencia a `event-subscription [create|update]` cuando se usa un webhook como destino para una suscripción de eventos.
* Se ha agregado el parámetro source-resource-id para todos los comandos relativos a suscripciones de eventos, y se han marcado en desuso todos los demás parámetros relativos al recurso de origen.

### <a name="hdinsight"></a>HDInsight
* [CAMBIO IMPORTANTE] Se han eliminado los parámetros `--virtual-network` y `--subnet-name` en `hdinsight [application] create`.
* [CAMBIO IMPORTANTE] Se ha cambiado `hdinsight create --storage-account` para aceptar el nombre o el identificador de una cuenta de almacenamiento en lugar de los puntos de conexión de un blob.
* Se han agregado los parámetros `--vnet-name` y `--subnet-name` a `hdinsight create`.
* Se ha agregado compatibilidad con Enterprise Security Package y el cifrado de discos a `hdinsight create`. 
* Se agregó el comando `hdinsight rotate-disk-encryption-key`.
* Se agregó el comando `hdinsight update`.

### <a name="iot"></a>IoT
* Se ha agregado un formato de codificación al comando routing-endpoint.

### <a name="kusto"></a>Kusto
* Versión preliminar

### <a name="monitor"></a>Supervisión
* Se ha cambiado la comparación de identificadores para que no distinga entre mayúsculas y minúsculas.

### <a name="profile"></a>Perfil
* Se ha habilitado la cuenta de nivel de inquilino para la identidad de servicio administrada de `login`.

### <a name="network"></a>Red
* Se ha corregido el problema con `express-route update` por el que se pasaba por el alto el argumento `--bandwidth`.
* Se ha corregido el problema con `ddos-protection update` por el que la comprensión de conjuntos provocaba el seguimiento de la pila.

### <a name="resource"></a>Resource
* Se ha agregado compatibilidad para el archivo de parámetros URI a `group deployment create`.
* Se ha agregado compatibilidad para identidades administradas a `policy assignment [create|list|show]`.

### <a name="sql-virtual-machine"></a>Máquina virtual SQL
* Versión preliminar

### <a name="storage"></a>Storage
* Se ha modificado una corrección para actualizar solo las propiedades que se cambian en el mismo objeto.
* Se ha corregido el problema 8021: los datos binarios se codifican en base 64 cuando se devuelven.

### <a name="vm"></a>máquina virtual
* Se ha cambiado `vm encryption enable` para validar el almacén de claves de cifrado de disco y ese almacén de claves de cifrado existe.
* Se ha agregado la marca `--force` a `vm encryption enable`.

## <a name="january-15-2019"></a>15 de enero de 2019

Versión 2.0.55

### <a name="acr"></a>ACR
* Se ha cambiado para poder forzar la inserción de un gráfico de Helm que no existe.
* Se ha cambiado para permitir las operaciones en tiempo de ejecución sin solicitudes ARM.
* [EN DESUSO] Se ha dejado de usar el parámetro `--resource-group` en los comandos:
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a>ACS
* Se ha agregado compatibilidad para nuevas regiones de ACI.

### <a name="appservice"></a>Appservice
* Se ha corregido un problema con la carga de certificados para aplicaciones hospedadas en un entorno ASE, donde los grupos de recursos del entorno ASE y de la aplicación son diferentes.
* Se ha cambiado `webapp up` para que use la SKU P1V1 como predeterminada para Linux.
* Se ha corregido `[webapp|functionapp] deployment source config-zip` para mostrar el mensaje de error correcto cuando se produce un error en una implementación. 
* Se agregó el comando `webapp ssh`.

### <a name="botservice"></a>Botservice
* Se han agregado actualizaciones al estado de implementación a `bot create`.

### <a name="configure"></a>Configuración
* Se ha agregado `none` como formato de salida configurable.

### <a name="cosmosdb"></a>CosmosDB
* Se ha agregado compatibilidad para la creación de bases de datos con una capacidad de proceso compartida.

### <a name="hdinsight"></a>HDInsight
* Se han agregado comandos para administrar aplicaciones.
* Se han agregado comandos para administrar acciones de script.
* Se han agregado comandos para administrar Operations Management Suite (OMS).
* Se ha agregado compatibilidad para enumerar el uso regional a `hdinsight list-usage`.
* [CAMBIO IMPORTANTE] Se ha quitado el tipo de clúster predeterminado de `hdinsight create`.

### <a name="network"></a>Red
* Se agregaron los argumentos `--custom-headers` y `--status-code-ranges` a `traffic-manager profile [create|update]`
* Se han agregado nuevos tipos enrutamientos: subred y multivalor.
* Se agregaron los argumentos `--custom-headers` y `--subnets` a `traffic-manager endpoint [create|update]`  
* Se ha corregido el problema por el que se producía un error al suministrar `--vnets ""` a `ddos-protection update`.

### <a name="role"></a>Role
* [EN DESUSO] Se ha dejado de usar el argumento `--password` para `create-for-rbac`. En su lugar, use contraseñas seguras generadas por la CLI.

### <a name="security"></a>Seguridad
* Versión inicial

### <a name="storage"></a>Storage
* [CAMBIO IMPORTANTE] Se ha cambiado el número predeterminado de resultados de `storage [blob|file|container|share] list` a 5000. Use `--num-results *` para el comportamiento original de devolver todos los resultados.
* Se ha agregado el parámetro `--marker` a `storage [blob|file|container|share] list`
* Se ha agregado un marcador de registro para página siguiente en STDERR para `storage [blob|file|container|share] list`. 
* Se ha agregado el comando `storage blob service-properties update` con compatibilidad para sitios web estáticos.

### <a name="vm"></a>máquina virtual
* Se ha cambiado `vm [disk|unmanaged-disk]` y `vmss disk` para que tengan parámetros más coherentes.
* Se ha agregado compatibilidad para hacer referencia a imágenes entre inquilinos a `[vm|vmss] create`.
* Se ha corregido el error con la configuración predeterminada de `vm diagnostics get-default-config --windows-os`.
* Se ha agregado el argumento `--provision-after-extensions` a `vmss extension set` para definir qué extensiones se deben aprovisionar antes de establecer la extensión.
* Se ha agregado el argumento `--replica-count` a `sig image-version update` para establecer el número predeterminado de replicaciones.
* Se ha corregido el error con `image create --source` por el que se confundía el disco de sistema operativo de origen para una máquina virtual con el mismo nombre, aunque se proporcionara el identificador de recurso completo.

## <a name="december-20-2018"></a>20 de diciembre de 2018

Versión 2.0.54
### <a name="appservice"></a>Appservice
* Se ha corregido el problema por el que `webapp up` producía un error al volver a implementarse.
* Se ha agregado compatibilidad para enumerar y restaurar instantáneas de aplicaciones web.
* Se ha agregado compatibilidad con la marca `--runtime` para aplicaciones de función de Windows.

### <a name="iotcentral"></a>IoTCentral
* Se ha corregido la actualización de la llamada API del comando

### <a name="role"></a>Role
* [CAMBIO IMPORTANTE] Se ha cambiado `ad [app|sp] list` para que solo enumere los 100 primeros objetos de forma predeterminada.

### <a name="sql"></a>SQL
* Se ha agregado compatibilidad para la intercalación personalizada en instancias administradas.

### <a name="vm"></a>máquina virtual
* Se ha agregado el parámetro `---os-type` a `disk create`

## <a name="december-18-2018"></a>18 de diciembre de 2018

Versión 2.0.53
### <a name="acr"></a>ACR
* Se ha agregado compatibilidad para la importación de imágenes desde registros de contenedor externo.
* Se ha comprimido el diseño de tabla para la lista de tareas.
* Se ha agregado compatibilidad para las direcciones URL de Azure DevOps.

### <a name="acs"></a>ACS
* Se ha agregado la versión preliminar de nodos virtuales.
* Se ha quitado "(VERSIÓN PRELIMINAR)" de los argumentos de AAD a `aks create`.
* [EN DESUSO] Se han dejado de usar los comandos `az acs`. El servicio de ACS se retirará el 31 de enero de 2020.
* Se ha agregado compatibilidad de directiva de red al crear nuevos clústeres de AKS.
* Se ha eliminado el requisito del argumento `--nodepool-name` para `aks scale` si hay un único nodepool.

### <a name="appservice"></a>Appservice
* Se ha corregido un problema donde `webapp config container` no aplicaba el parámetro `--slot`.

### <a name="botservice"></a>Botservice
* Se ha agregado compatibilidad con el análisis de archivo `.bot` al llamar a `bot show`.
* Se ha corregido el error de aprovisionamiento de AppInsights.
* Se ha corregido un error de espacios en blanco al trabajar con rutas de acceso de archivo.
* Se han reducido las llamadas de red de Kudu.
* Se ha mejorado la experiencia de usuario de comandos generales.

### <a name="consumption"></a>Consumo
* Se han corregido errores para que la API de presupuesto muestre notificaciones.

### <a name="cosmosdb"></a>CosmosDB
* Se ha agregado compatibilidad para actualizar la cuenta de la arquitectura multimaestro a de un único maestro.

### <a name="maps"></a>Mapas
* Se agregó compatibilidad para S1 SKU a `maps account [create|update]`.

### <a name="network"></a>Red
* Se ha agregado compatibilidad para `--format` y `--log-version` a `watcher flow-log configure`
* Se ha corregido un problema con `dns zone update` donde no funcionaba el uso de "" para borrar las redes virtuales de registro y resolución.

### <a name="resource"></a>Resource
* Se ha corregido el control del parámetro de ámbito para los grupos de administración en `policy assignment [create|list|delete|show|update]`. 
* Se ha agregado un nuevo comando `resource wait`.

### <a name="storage"></a>Storage
*  Se ha agregado la posibilidad de actualizar la versión del esquema de registro para servicios de almacenamiento en `storage logging update`.

### <a name="vm"></a>máquina virtual
* Se ha corregido el bloqueo en `vm identity remove` cuando la máquina virtual especificada no tenía ninguna identidad de servicio administrada asignada.

## <a name="december-4-2018"></a>4 de diciembre de 2018

Versión 2.0.52
### <a name="core"></a>Core
* Se ha agregado compatibilidad para el aprovisionamiento de recursos entre inquilinos para entidades de servicio multiinquilino
* Se ha corregido el error por el que los comandos con salida tsv no se analizaban correctamente

### <a name="appservice"></a>Appservice
* [VERSIÓN PRELIMINAR] Se han agregado comandos `webapp up` que ayudan a crear e implementar contenido a la aplicación
* Se ha corregido un error en la aplicación Windows basada en contenedor debido a un cambio de back-end

### <a name="network"></a>Red
* Se ha agregado el argumento `--exclusion` a `application-gateway waf-config set` para admitir las exclusiones de WAF

### <a name="role"></a>Role
* Se ha agregado compatibilidad para identificadores personalizados para las credenciales de contraseña 

### <a name="vm"></a>máquina virtual
* [EN DESUSO] Se ha dejado de usar el parámetro `vm extension [show|wait] --expand`
* Se ha agregado el parámetro `--force` a `vm restart` para volver a implementar máquinas virtuales que no responden
* Se ha cambiado `[vm|vmss] create --authentication-type` para que acepte el valor "all" para crear una máquina virtual con autenticación mediante contraseña y SSH
* Se ha agregado el parámetro `image create --os-disk-caching` para establecer el almacenamiento en caché del disco de sistema operativo de una imagen

## <a name="november-20-2018"></a>20 de noviembre de 2018

Versión 2.0.51
### <a name="core"></a>Core
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

### <a name="core"></a>Core
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

### <a name="resource"></a>Resource
* Ha agregado compatibilidad con grupos de administración y suscripciones a los comandos `policy definition|set-definition`

### <a name="role"></a>Role
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

### <a name="core"></a>Core
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

### <a name="core"></a>Core
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
* Versión inicial

### <a name="iot"></a>IoT
* Se ha agregado un comando de instalación de extensiones al banner de primera ejecución

### <a name="keyvault"></a>KeyVault
* Se ha modificado para restringir los comandos de almacenamiento del almacén de claves al perfil de API más reciente

### <a name="network"></a>Red
* Se ha corregido `network dns zone create`: el comando se ejecuta correctamente incluso si el usuario ha configurado una ubicación predeterminada. Consulte el número 6052
* `--remote-vnet-id` en desuso para `network vnet peering create`
* Se ha agregado `--remote-vnet` a `network vnet peering create`, el cual acepta un nombre o identificador
* Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet create` con `--subnet-prefixes`
* Se ha agregado compatibilidad con varios prefijos de dirección a `network vnet subnet [create|update]` con `--address-prefixes`
* Se ha corregido el problema con `network application-gateway create` que impedía la creación de puertas de enlace con las SKU `WAF_v2` o `Standard_v2`
* Se ha agregado el argumento de comodidad `--service-endpoint-policy` a `network vnet subnet update`

### <a name="role"></a>Role
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
* `network express-route create/update`: Se ha agregado la marca `--allow-global-reach`
* `network vnet subnet create/update`: se ha agregado compatibilidad para `--delegation`
* Se agregó el comando `network vnet subnet list-available-delegations`.
* `network traffic-manager profile create/update`: Se ha agregado compatibilidad para `--interval`, `--timeout` y `--max-failures` para la configuración de Monitor. Las opciones `--monitor-path`, `--monitor-port` y `--monitor-protocol` han dejado de usarse en favor de `--path`, `--port`, `--protocol`
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

### <a name="role"></a>Role
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

### <a name="core"></a>Core

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

### <a name="resource"></a>Resource

* Se ha cambiado `provider operation show` para salir con código 3 cuando falta un recurso

### <a name="storage"></a>Storage

* Se ha cambiado `storage share policy show` para salir con código 3 cuando falta un recurso

### <a name="vm"></a>máquina virtual

* Se ha cambiado `vm/vmss identity show` para salir con código 3 cuando falta un recurso 
* `--storage-caching` en desuso para `vm create`

## <a name="auguest-14-2018"></a>14 de agosto de 2018

Versión 2.0.44

### <a name="core"></a>Core

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

* Versión inicial

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

### <a name="resource"></a>Resource

* Se ha agregado `--rollback-on-error` a `group deployment create` para ejecutar una implementación correcta conocida en caso de error.
* Se ha corregido el problema por el que `--parameters {}` con `group deployment create` generaba un error.

### <a name="role"></a>Role

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

### <a name="core"></a>Core

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

### <a name="resource"></a>Resource

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

### <a name="core"></a>Core

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

### <a name="resource"></a>Resource

* Se ha agregado un nuevo grupo de operaciones `deployment`

### <a name="vm"></a>máquina virtual

* Se ha agregado compatibilidad para quitar la identidad asignada por el sistema

## <a name="june-25-2018"></a>25 de junio de 2018

Versión 2.0.39

### <a name="cli"></a>CLI

* Se ha actualizado el recorte de archivo en el instalador MSI para corregir el problema de instalación de extensión

## <a name="june-19-2018"></a>19 de junio de 2018

Versión 2.0.38

### <a name="core"></a>Core

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

* Se ha agregado compatibilidad para `https` a `network lb probe create` [6571](https://github.com/Azure/azure-cli/issues/6571).
* Se ha corregido un problema por el que `--endpoint-status` distinguía entre mayúsculas y minúsculas. [n.º 6502](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a>Reservations

* [CAMBIO IMPORTANTE] Se ha agregado el parámetro necesario `ReservedResourceType` a `reservations catalog show`.
* Se ha agregado el parámetro `Location` a `reservations catalog show`.
* [CAMBIO IMPORTANTE] Se ha eliminado `kind` de `ReservationProperties`.
* [CAMBIO IMPORTANTE] Se ha cambiado el nombre de `capabilities` a `sku_properties` en `Catalog`.
* [CAMBIO IMPORTANTE] Se han quitado las propiedades `size` y `tier` de `Catalog`.
* Se ha agregado el parámetro `InstanceFlexibility` a `reservations reservation update`.

### <a name="role"></a>Role

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

### <a name="core"></a>Core

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

### <a name="core"></a>Core

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

### <a name="core"></a>Core

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

### <a name="core"></a>Core

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

* Se ha corregido el error de escritura en el ejemplo de `cognitiveservices account create` [5603](https://github.com/Azure/azure-cli/issues/5603).

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

### <a name="role"></a>Role

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

* Se han agregado los parámetros de montaje de volúmenes del repositorio de git `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` y `--gitrepo-mount-path`.
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

### <a name="resource"></a>Resource

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

### <a name="core"></a>Core

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

* Se ha agregado compatibilidad para `--top`, `--orderby` y `--namespace` a `metrics list` [5785](https://github.com/Azure/azure-cli/issues/5785).
* Se ha corregido el problema [4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` acepta una lista separada por espacios de las métricas que se van a recuperar
* Se ha agregado compatibilidad para `--namespace` a `metrics list-definitions` [5785](https://github.com/Azure/azure-cli/issues/5785).

### <a name="network"></a>Red

* Se ha agregado compatibilidad para zonas DNS privadas

### <a name="profile"></a>Perfil

* Se ha agregado una advertencia para `--identity-port` y `--msi-port` a `login`

### <a name="rdbms"></a>RDBMS

* Se ha agregado el modelo de negocio GA API versión 2017-12-01

### <a name="resource"></a>Resource

* [CAMBIO IMPORTANTE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a>Role

* Se ha agregado compatibilidad para configuraciones de acceso necesarias y clientes nativos a `az ad app create`
* Se han cambiado los comandos `rbac` para que devuelvan menos de 1000 identificadores de resolución de objeto
* Se agregaron comandos de administración de credenciales `ad sp credential [reset|list|delete]`
* [CAMBIO IMPORTANTE] Se quitó "properties" de la salida de `az role assignment [list|show]`
* Se ha agregado compatibilidad para los permisos `dataActions` y `notDataActions` a `role definition`

### <a name="storage"></a>Storage

* Se ha corregido un problema al cargar archivos con un tamaño de entre 195 GB y 200 GB
* Se ha corregido el problema [4049](https://github.com/Azure/azure-cli/issues/4049): los problemas con las cargas de blobs de anexión ignoraban los parámetros de condición

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

* Versión inicial

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

* Versión inicial

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

### <a name="core"></a>Core

* Se ha corregido el problema [5184](https://github.com/Azure/azure-cli/issues/5184): problema de instalación de Homebrew
* Se ha agregado compatibilidad para la telemetría de la extensión con claves personalizadas
* Se ha agregado el registro de HTTP a `--debug`

### <a name="acs"></a>ACS

* Se ha modificado para usar el gráfico de Helm `virtual-kubelet-for-aks` para `aks install-connector` de forma predeterminada
* Se ha corregido el problema: problema de permisos insuficientes para que las entidades de servicio creen el grupo de contenedores ACI
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

* Se ha corregido el problema [5559](https://github.com/Azure/azure-cli/issues/5559): falta el cliente en `network vnet-gateway vpn-client generate`

### <a name="resource"></a>Resource

* Se ha modificado `group deployment export` para mostrar una plantilla parcial y mensajes en caso de error

### <a name="role"></a>Role

* Se ha agregado `role assignment list-changelogs` para permitir la auditoría de los roles de la entidad de servicio

### <a name="sql"></a>SQL

* Se ha agregado compatibilidad para redundancia de zona para las bases de datos y los grupos elásticos tanto en creación como en actualización

### <a name="storage"></a>Storage

* Se ha habilitado al especificación de destino y ruta de acceso o prefijo para `storage blob [upload-batch|download-batch]`

### <a name="vm"></a>máquina virtual

* Se ha agregado compatibilidad con la conexión y desconexión de discos en una única instancia de VMSS


## <a name="february-13-2018"></a>13 de febrero de 2018

Versión 2.0.27

### <a name="core"></a>Core

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

### <a name="resource"></a>Resource

* Se ha agregado de nuevo `feature show`

### <a name="role"></a>Role

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

### <a name="core"></a>Core

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

### <a name="resource"></a>Resource

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

### <a name="role"></a>Role

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

### <a name="core"></a>Core
* Se modificó el punto de conexión de autoridad de AAD `AZURE_US_GOV_CLOUD` de login.microsoftonline.com a login.microsoftonline.us
* Se corrigió el problema por el que se podía enviar datos de telemetría continuamente

### <a name="acs"></a>ACS

* Se agregaron los comandos `aks install-connector` y `aks remove-connector`
* Se mejoraron los informes de errores de `acs create`
* Se corrigió el uso de `aks get-credentials -f` sin ruta de acceso completa

### <a name="advisor"></a>Advisor

* Versión inicial

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

### <a name="resource"></a>Resource

* Se agregó el argumento `--include-response-body` a `resource show`

### <a name="role"></a>Role

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

### <a name="resource"></a>Resource

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
* Cambio de nombre de `vm format-secret` a `vm secret format`
* Se agregó el argumento `--encrypt format` a `vm encryption enable`

## <a name="october-24-2017"></a>24 de octubre de 2017

Versión 2.0.20

### <a name="core"></a>Core

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

### <a name="resource"></a>Resource

* Se corrigió la incompatibilidad con la versión más reciente de la dependencia msrest en `group export`
* Se corrigió `policy assignment create` para trabajar con definiciones de directivas integradas y definiciones de conjuntos de directivas

### <a name="vm"></a>máquina virtual

* Se agregó el argumento `--accelerated-networking` a `vmss create`


## <a name="october-9-2017"></a>9 de octubre de 2017

Versión 2.0.19

### <a name="core"></a>Core

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

### <a name="resource"></a>Resource

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

### <a name="resource"></a>Resource

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

### <a name="core"></a>Core

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

* Cambio de nombre de `vnet list-private-access-services` a `vnet list-endpoint-services`
* Se cambió el nombre del argumento `--private-access-services` a `--service-endpoints` para `vnet subnet create/update`.
* Se agregó compatibilidad para varios intervalos de direcciones IP y puertos a `nsg rule create/update`.
* Se agregó compatibilidad para SKU a `lb create`.
* Se agregó compatibilidad para SKU a `public-ip create`.

### <a name="resource"></a>Resource

* Se permite pasar las definiciones de parámetro de directiva de recursos en `policy definition create` y `policy definition update`.
* Se permite pasar valores de parámetro para `policy assignment create`.
* Se permite pasar código JSON o archivo para todos los parámetros.
* Versión de API incrementada

### <a name="sql"></a>SQL

* Se agregaron los comandos `sql server vnet-rule`.

### <a name="vm"></a>máquina virtual

* Solucionado: no asignar acceso a menos que se proporcione `--scope`.
* Solucionado: usar para las extensiones la misma nomenclatura que el portal.
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
* Solucionado: la configuración de los espacios se detecta correctamente.

### <a name="iot"></a>IoT

* Se ha corregido el problema 3934: la creación de directivas ya no borra las directivas existentes.

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

* `create`: se ha corregido un problema por el que no se permitía el signo igual en una variable de entorno.


### <a name="data-lake-store"></a>Data Lake Store

* Control de progreso habilitado.

### <a name="event-grid"></a>Event Grid

* Versión inicial

### <a name="network"></a>Red

* `lb`: se ha corregido un problema por el que determinados nombres de recursos secundarios no se resolvían correctamente cuando se omitían.
* `application-gateway {subresource} delete`: se ha corregido un problema por el que no se aplicaba `--no-wait`.
* `application-gateway http-settings update`: se ha corregido un problema por el que `--connection-draining-timeout` no podía desactivarse.
* Se corrigió un error de argumento de palabra clave `sa_data_size_kilobyes` inesperado con `az network vpn-connection ipsec-policy add`.

### <a name="profile"></a>Perfil

* `account list`: se ha agregado `--refresh` para sincronizar las suscripciones más recientes del servidor.

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

### <a name="core"></a>Core

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
  * Subcomandos de `keyvault``purge`, `recover`, `keyvault list-deleted`
  * Subcomandos de `keyvault secret``backup`, `restore`, `purge`, `recover`, `list-deleted`
  * Subcomandos de `keyvault certificate``purge`, `recover`, `list-deleted`
  * Subcomandos de `keyvault key``purge`, `recover`, `list-deleted`
* Se agregó integración para almacén de claves de entidad de servicio (n.º 3133).
* Se actualizó el plano de datos del almacén de claves a 0.3.2 (n.º 3307).

### <a name="lab"></a>Laboratorio

* Se agregó compatibilidad para reclamar todas las máquinas virtuales del laboratorio mediante `az lab vm claim`.
* Se agregó un formateador de tablas de salida para `az lab vm list` y `az lab vm show`.

### <a name="monitor"></a>Supervisión

* Se corrigió el archivo de plantilla con el comando `monitor autoscale-settings get-parameters-template` (n.º 3349).
* Cambio de nombre de `monitor alert-rule-incidents list` a `monitor alert list-incidents`
* Cambio de nombre de `monitor alert-rule-incidents show` a `monitor alert show-incident`
* Cambio de nombre de `monitor metric-defintions list` a `monitor metrics list-definitions`
* Cambio de nombre de `monitor alert-rules` a `monitor alert`
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
* Se ha agregado compatibilidad para `--dns-servers` a `nic update` y `nic create`. Se ha agregado compatibilidad para servidores --dns.
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

### <a name="resource"></a>Resource

* Se mejoraron los mensajes de parámetros que faltan para `group deployment create`.
* Se mejoró el análisis de la sintaxis `--parameters KEY=VALUE`.
* Se corrigieron los problemas por los que los archivos de parámetros de `group deployment create` ya no se reconocen con la sintaxis `@<file>`.
* Compatibilidad con el argumento `--ids` para los comandos `resource` y `managedapp`.
* Se corrigieron algunos mensajes de error y de análisis (n.º 3584).
* Se corrigió el análisis de `--resource-type` para el comando `lock` para aceptar `<resource-namespace>` y `<resource-type>`.
* Se agregó comprobación de los parámetros para las plantillas de vínculo de plantilla (n.º 3629).
* Se agregó compatibilidad para especificar los parámetros de implementación mediante la sintaxis `KEY=VALUE`.

### <a name="role"></a>Role

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

* Se eliminó el parámetro `sql server create` `--identity` roto.
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

### <a name="core"></a>Core

* core: capturar excepciones producidas por un proveedor no registrado y registrarlo automáticamente
* perf: persistir caché de tokens Adal en memoria hasta que se realice el procesamiento ([#2603](https://github.com/Azure/azure-cli/issues/2603))
* Corregir bytes devueltos de la huella digital hexadecimal -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))
* Mejora de la descarga de certificados de Key Vault y de la integración de entidades de servicio de AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003))
* Agregar ubicación de Python a "az —version" ([#2986](https://github.com/Azure/azure-cli/issues/2986))
* login: admitir inicios de sesión cuando no hay suscripciones ([#2929](https://github.com/Azure/azure-cli/issues/2929))
* core: corregir un error al iniciar sesión dos veces con una entidad de servicio ([#2800](https://github.com/Azure/azure-cli/issues/2800))
* core: permitir que la ruta de acceso al archivo accessTokens.json se pueda configurar con env-var ([n.º 2605](https://github.com/Azure/azure-cli/issues/2605))
* core: permitir que los valores predeterminados configurados se apliquen a argumentos opcionales ([n.º 2703](https://github.com/Azure/azure-cli/issues/2703))
* core: rendimiento mejorado.
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
* BC: quitar --expires y --not-before de `keyvault certificate create` porque el servicio no admite estos parámetros
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

* Corrección de errores: modelado de `--actions` de `az alert-rules create` para consumir cadenas JSON ([n.º 3009](https://github.com/Azure/azure-cli/issues/3009))
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

### <a name="resource"></a>Resource

* Agregar comandos de definición managedapp y managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985))
* Compatibilidad de comandos de "operación de proveedores" ([#2908](https://github.com/Azure/azure-cli/issues/2908))
* Compatibilidad para creación de recursos genéricos ([#2606](https://github.com/Azure/azure-cli/issues/2606))
* Corregir análisis de recursos y búsqueda de versiones de API ([#2781](https://github.com/Azure/azure-cli/issues/2781))
* Agregar documentos para actualización de az lock ([#2702](https://github.com/Azure/azure-cli/issues/2702))
* Error generado si trata de enumerar recursos de un grupo que no existe ([#2769](https://github.com/Azure/azure-cli/issues/2769))
* [Compute] Corregir errores con la actualización de conjuntos de disponibilidad de VMSS y VM ([#2773](https://github.com/Azure/azure-cli/issues/2773))
* Corregir la creación y eliminación de bloqueos si parent-resource-path es None ([#2742](https://github.com/Azure/azure-cli/issues/2742))

### <a name="role"></a>Role

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

  nota: comandos de máquina virtual en nubes soberanas. Evitar características relacionadas con discos administrados, incluidas las siguientes:
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

### <a name="core"></a>Core

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

* DocumentDB: compatibilidad agregada para enumerar las cadenas de conexión ([n.º 2580](https://github.com/Azure/azure-cli/pull/2580))

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

