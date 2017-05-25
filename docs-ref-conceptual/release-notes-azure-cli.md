---
title: "Notas de la versión de la CLI de Azure 2.0"
description: "Obtenga información acerca de las actualizaciones más recientes de la CLI de Azure 2.0"
keywords: "CLI de Azure 2.0, notas de la versión"
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 3bd4b9c059da3b841fc0757a11bc7ce78ec64b08
ms.sourcegitcommit: 66d997a5afcf32143a4d4817ec1608cbdf58a59f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/11/2017
---
# <a name="azure-cli-20-release-notes"></a>Notas de la versión de la CLI de Azure 2.0

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
Puede formular preguntas sobre el [uso de StackOverflow mediante la etiqueta de cli de azure](http://stackoverflow.com/questions/tagged/azure-cli), o ponerse en contacto con el equipo del producto en [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).
Puede proporcionar comentarios desde la línea de comandos con el comando `az feedback`.

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

