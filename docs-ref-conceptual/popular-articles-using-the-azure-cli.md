---
title: Vínculos de varios servicios sobre el trabajo con la CLI de Azure
description: Vínculos a tutoriales populares, inicios rápidos, ejemplos, conceptos y guías de procedimientos, la CLI de Azure, máquinas virtuales, Azure Kubernetes Service (AKS), Batch, CLI de Azure (Core), Azure Resource Manager, Key Vault, Azure Stack Hub, Functions, Database, Event Hubs, App Configuración, configuración de la aplicación, Alemania, seguridad, gobernanza, información, IoT, Internet de las cosas, DevOps, Virtual Network, Compute, Networking, Herramientas de desarrollo, bases de datos, Analytics, administración y gobernanza, híbrido, almacenamiento, seguridad, IA, IA y Machine Learning, Linux, Windows, Ubuntu, automatización, aplicación, aplicación web, script
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 03/01/2020
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 3a0b2e315e0eaf6c352aa2737f33da043b5feb7d
ms.sourcegitcommit: 93d8137f37e974f7d314a0b1deb65ac563c2e2c5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/21/2020
ms.locfileid: "80075940"
---
# <a name="popular-articles-using-the-azure-cli"></a>Artículos populares en los que se usa la CLI de Azure

La CLI de Azure se usa en muchos servicios de Azure, lo que da lugar a la diversificación de artículos entre los repositorios de documentos.  Esta página proporciona vínculos para seleccionar los artículos más populares.  

## <a name="compute"></a>Proceso

| | | | |
|-|-|-|-|
|Virtual Machines | Tutorial: Linux | [Creación de una máquina virtual Linux con la CLI de Azure](azure-cli-vm-tutorial.yml) | Cree una máquina virtual.  Obtenga información sobre las consultas de salida y el establecimiento de las variables de entorno.
|Virtual Machines | Inicio rápido: Linux | [Creación de una máquina virtual Linux mediante la CLI de Azure](/azure/virtual-machines/linux/quick-create-cli) | Cree e implemente una máquina virtual Linux.  Abra un puerto para el tráfico web e instale un servidor web.
|Virtual Machines | Guía paso a paso: Linux |[Creación de una imagen Linux de una máquina virtual o un disco duro virtual](/azure/virtual-machines/linux/capture-image) | Desaprovisione una máquina virtual existente, cree una imagen y cree una nueva máquina virtual a partir de la imagen capturada.
|Virtual Machines | Guía paso a paso: Linux | [Carga de un disco duro virtual en Azure mediante la CLI de Azure](/azure/virtual-machines/linux/disks-upload-vhd-to-managed-disk-cli) | Cree un disco administrado vacío, cargue el archivo VHD local y copie un disco administrado.
|Virtual Machines | Guía paso a paso: Linux | [Creación de una galería de imágenes compartidas mediante la CLI de Azure](/azure/virtual-machines/linux/shared-images) | Cree Shared Image Gallery, una galería con imágenes de máquina virtual personalizadas compartidas con otras personas de la organización, dentro de una región, entre regiones o dentro de un inquilino de Azure Active Directory.
|Virtual Machines | Guía paso a paso: Linux | [Implementación de máquinas virtuales de Spot con la CLI de Azure (versión preliminar)](/azure/virtual-machines/linux/spot-cli) | Implemente una máquina virtual Linux de Spot que no se expulse en función del precio.
|Virtual Machines | Inicio rápido: Windows | [Creación de una máquina virtual Windows con la CLI de Azure](/azure/virtual-machines/windows/quick-create-cli) | Implemente una máquina virtual en Azure que ejecute Windows Server 2016.
|Virtual Machines | Módulo de aprendizaje | [Administración de máquinas virtuales con la CLI de Azure](https://docs.microsoft.com/learn/modules/manage-virtual-machines-with-azure-cli/) | Cree, inicie, detenga y realice tareas de administración adicionales relacionadas con máquinas virtuales.
|Azure Kubernetes Service (AKS)| Guía de inicio rápido | [Implementación de un clúster de Azure Kubernetes Service (AKS) mediante la CLI de Azure](/azure/aks/kubernetes-walkthrough) | Implemente y administre clústeres de AKS.  Consulte cómo supervisar el mantenimiento del clúster y los pods que ejecutan la aplicación.
|Azure Batch|Muestra | [Ejecución de un trabajo y de tareas con Azure Batch mediante la CLI de Azure](/azure/batch/scripts/batch-cli-sample-run-job) | Cree un trabajo de Batch y agregue una serie de tareas al trabajo. Supervise un trabajo y sus tareas.
|Azure Batch|Muestra | [Creación y administración de un grupo de Windows en Azure Batch con la CLI de Azure](/azure/batch/scripts/batch-cli-sample-manage-windows-pool) | Cree y administre un grupo de nodos de proceso Windows con una configuración de Cloud Services.
|Azure Container Instances|Guía de inicio rápido | [Implementación de una instancia de contenedor mediante la CLI de Azure](/azure/container-instances/container-instances-quickstart) | Implemente un contenedor de Docker aislado y haga que la aplicación esté disponible con un nombre de dominio completo (FQDN). Ejecute un solo comando de implementación y, a continuación, vaya a la aplicación que se ejecuta en el contenedor.
|Función de Azure|Guía de inicio rápido |  [Creación de una función en Azure que responda a solicitudes HTTP con la CLI de Azure](/azure/azure-functions/functions-create-first-azure-function-azure-cli) | Utilice herramientas de la línea de comandos para crear una función que responda a solicitudes HTTP. Después de probar el código localmente, implemente la función en el entorno sin servidor de Azure Functions.

## <a name="networking"></a>Redes

| | | | |
|-|-|-|-|
|Virtual Network|Guía de inicio rápido | [Creación de una red virtual mediante la CLI de Azure](/azure/virtual-network/quick-create-cli) | Cree una red virtual, implemente dos máquinas virtuales en la red virtual y conéctese a las máquinas virtuales desde Internet.
|Virtual Network|Guía paso a paso | [Habilitación de redes aceleradas en una máquina virtual Linux con la CLI de Azure](/azure/virtual-network/create-vm-accelerated-networking-cli) | Cree una máquina virtual Linux, controle el enlace dinámico y la revocación de la función virtual, y habilite las redes aceleradas.

## <a name="internet-of-things"></a>Internet de las cosas

| | | | |
|-|-|-|-|
|IoT Hub|Tutorial | [Configuración del enrutamiento de mensajes de IoT Hub mediante la CLI de Azure](/azure/iot-hub/tutorial-routing) | Configure y use consultas de enrutamiento personalizadas con IoT Hub.

## <a name="developer-tools"></a>Herramientas para desarrolladores

| | | | |
|-|-|-|-|
|Azure App Configuration|Ejemplos |[Ejemplos de la CLI de Azure para Azure App Configuration](/azure/azure-app-configuration/cli-samples) | Obtenga vínculos a scripts de bash que usan la CLI de Azure para Azure App Configuration.
|Azure DevOps| Introducción: Canalización de DevOps |[Creación de su primera canalización de Azure mediante la CLI de Azure](/azure/devops/pipelines/create-first-pipeline-cli) | Cree una nueva canalización en un directorio de GitHub clonado, administre y ejecute las canalizaciones.
|Azure DevOps| Guía paso a paso: Canalización de DevOps |[Tareas de implementación de una canalización de Azure mediante la CLI de Azure](/azure/devops/pipelines/tasks/deploy/azure-cli?view=azure-devops) | En una canalización de compilación o de versión, ejecute un script del shell o de Batch que contenga la CLI de Azure.  Los comandos se ejecutan en agentes multiplataforma que se ejecutan en sistemas operativos Linux, macOS o Windows.
|Azure DevOps| Tutorial: Canalización de Jenkins |[Implementación en Azure App Service con Jenkins mediante la CLI de Azure](/azure/jenkins/execute-cli-jenkins-pipeline) | Cree y configure una máquina virtual de Jenkins, cree una aplicación web en Azure y prepare un repositorio de GitHub.  Cree y ejecute la canalización de Jenkins.

## <a name="databases"></a>Bases de datos

| | | | |
|-|-|-|-|
|SQL Database| Muestra |[Configuración de Azure SQL Database con la CLI de Azure](/azure/sql-database/sql-database-cli-samples?tabs=single-database) | Ejemplos de la CLI de Azure para Azure SQL Database.
|MySQL|Guía de inicio rápido |[Creación de un servidor de Azure Database for MySQL mediante la CLI de Azure](/azure/mysql/quickstart-create-mysql-server-database-using-azure-cli) | Cree de un servidor de Azure Database for MySQL.  Configure una regla de firewall y la configuración de SSL.  Obtenga y utilice la información de conexión.
|Cosmos DB |Guía paso a paso |[Administración de recursos de Azure Cosmos mediante la CLI de Azure](/azure/cosmos-db/manage-with-cli) | Utilice comandos comunes para automatizar la administración de las cuentas, las bases de datos y los contenedores de Azure Cosmos DB.
|Cosmos DB |Muestra |[Ejemplos de la CLI de Azure para SQL API (Core) de Azure Cosmos DB](/azure/cosmos-db/cli-samples) | Obtenga vínculos a scripts de ejemplo de la CLI de Azure para SQL API (Core) de Azure Cosmos DB.

## <a name="analytics"></a>Análisis

| | | | |
|-|-|-|-|
Centro de eventos de Azure |Guía de inicio rápido |[Creación de un centro de eventos mediante la CLI de Azure](/azure/event-hubs/event-hubs-quickstart-cli) | Cree un espacio de nombres de Event Hubs y un centro de eventos.
HDInsight |Guía de procedimientos |[Creación de clústeres de HDInsight mediante la CLI de Azure](/azure/hdinsight/hdinsight-hadoop-create-linux-clusters-azure-cli) | Cree un clúster de HDInsight 3.6.
HDInsight |Tutorial |[Administración de clústeres de Azure HDInsight mediante la CLI de Azure](/azure/hdinsight/hdinsight-administer-use-command-line) | Enumere, muestre, elimine y escale clústeres de HDInsight.

## <a name="management-and-governance"></a>Administración y gobernanza

| | | | |
|-|-|-|-|
Plantillas de Resource Manager |Guía paso a paso |[Implementación de recursos con plantillas de Resource Manager y la CLI de Azure](/azure/azure-resource-manager/templates/deploy-cli) | Implemente los recursos en Azure mediante plantillas.
Grupos de Resource Manager |Guía paso a paso |[Administración de grupos de recursos de Azure Resource Manager mediante la CLI de Azure](/azure/azure-resource-manager/management/manage-resource-groups-cli) | Use Azure Resource Manager para administrar los grupos de recursos de Azure.
Gráfico de recursos |Guía de inicio rápido |[Ejecución de su primera consulta de Resource Graph con la CLI de Azure](/azure/governance/resource-graph/first-query-azurecli) | Agregue Azure Resource Graph a la instalación de la CLI de Azure y ejecute su primera consulta de Resource Graph.
Asignación de directiva |Guía de inicio rápido |[Creación de una asignación de directiva para identificar recursos no compatibles mediante la CLI de Azure](/azure/governance/policy/assign-policy-azurecli) | Cree una asignación de directiva para identificar máquinas virtuales que no usan discos administrados.

## <a name="hybrid"></a>Híbrido

| | | | |
|-|-|-|-|
Azure Stack Hub| Inicio rápido: Máquina virtual de Linux |[Creación de una máquina virtual con un servidor Linux en Azure Stack Hub mediante la CLI de Azure](/azure-stack/user/azure-stack-quick-create-vm-linux-cli) | Cree una máquina virtual con Ubuntu Server 16.04 LTS, conéctese a la máquina virtual con un cliente remoto e instale un servidor web NGINX.
Azure Stack Hub| Inicio rápido: Máquina virtual de Windows |[Creación de una máquina virtual con Windows Server en Azure Stack Hub mediante la CLI de Azure](/azure-stack/user/azure-stack-quick-create-vm-windows-cli) |Cree una máquina virtual con Windows Server 2016, conéctese a la máquina virtual con un cliente remoto e instale el servidor web IIS.
Azure Stack Hub| Guía paso a paso: Recursos de ASDK |[Administración e implementación de recursos en Azure Stack Hub con la CLI de Azure](/azure-stack/user/azure-stack-version-profiles-azurecli2) | Configure la CLI de Azure para administrar los recursos del Kit de desarrollo de Azure Stack (ASDK) desde las plataformas de cliente de Linux, Mac y Windows.

## <a name="storage"></a>Storage

| | | | |
|-|-|-|-|
Almacenamiento de blobs |Guía de inicio rápido |  [Creación, descarga y enumeración de blobs mediante la CLI de Azure](/azure/storage/blobs/storage-quickstart-blobs-cli) | Cargue y descargue datos hacia y desde Azure Blob Storage.
Almacenamiento de blobs |Guía paso a paso |[Autorización del acceso a los datos de blobs o colas con la CLI de Azure](/azure/storage/common/authorize-data-operations-cli) | Especifique cómo se autorizan las operaciones de datos y establezca las variables de entorno para los parámetros.
Almacenamiento de blobs |Guía paso a paso |[Uso de la CLI de Azure para administrar directorios, archivos y listas de control de acceso en Azure Data Lake Storage Gen2 (versión preliminar)](/azure/storage/blobs/data-lake-storage-directory-file-acl-cli) | Cree y administre directorios, archivos y permisos en cuentas de almacenamiento que tengan un espacio de nombres jerárquico.
File Storage |Guía de inicio rápido |[Creación y administración de recursos compartidos de archivos de Azure mediante la CLI de Azure](/azure/storage/files/storage-how-to-use-files-cli) | Cree y utilice recursos compartidos de archivos de Azure.  Cree y administre instantáneas de recursos compartidos.

## <a name="security"></a>Seguridad

| | | | |
|-|-|-|-|
Entidad de servicio |Guía paso a paso |[Creación de una entidad de servicio de Azure con la CLI de Azure](/cli/azure/create-an-azure-service-principal-azure-cli) | Cree, obtenga información sobre ella y restablezca una entidad de servicio con la CLI de Azure.
RBAC |Guía paso a paso |[Incorporación o eliminación de asignaciones de roles con RBAC de Azure y la CLI de Azure](/azure/role-based-access-control/role-assignments-cli) | Asigne roles al control de acceso basado en roles de Azure.
Key Vault |Guía paso a paso |[Administración de Key Vault mediante la CLI de Azure](/azure/key-vault/key-vault-manage-with-cli2) | Cree y administre Azure Key Vault.  Registre y autorice una aplicación, establezca directivas de acceso avanzadas y obtenga información sobre los comandos de la interfaz de la línea de comandos multiplataforma.
Key Vault |Tutorial |[Administración de claves de cuenta de almacenamiento con Key Vault y la CLI de Azure](/azure/key-vault/key-vault-ovw-storage-keys) | Administre claves de cuenta de almacenamiento y genere tokens de firma de acceso compartido.

## <a name="ai--machine-learning"></a>AI + Aprendizaje automático

| | | | |
|-|-|-|-|
Machine Learning |Referencia |[Uso de la extensión de la CLI de Azure para Azure Machine Learning](/azure/machine-learning/reference-azure-machine-learning-cli) | Ejecute experimentos para crear modelos de aprendizaje automático y registre modelos de aprendizaje automático para su uso por parte del cliente.  Empaquete, implemente y realice un seguimiento del ciclo de vida de los modelos de aprendizaje automático.
Cognitive Services |Guía de procedimientos |[Creación de un recurso de Cognitive Services con la CLI de Azure](/azure/cognitive-services/cognitive-services-apis-create-account-cli) | Suscríbase a Azure Cognitive Services y cree una cuenta con una suscripción a un solo servicio o a varios servicios.  Use las claves y el punto de conexión generados para autenticar las aplicaciones.
Azure Monitor |Guía paso a paso |[Creación de un área de trabajo de Log Analytics con la CLI de Azure](/azure/azure-monitor/learn/quick-create-workspace-cli) | Cree e implemente un área de trabajo de Log Analytics.

## <a name="geographies"></a>Zonas geográficas

| | | | |
|-|-|-|-|
Azure Alemania |Introducción |[Conexión a Azure Alemania mediante la CLI de Azure](/azure/germany/germany-get-started-connect-with-cli) | Con Azure Alemania, administre una suscripción de gran tamaño mediante scripts y acceda a características que no están disponibles actualmente en Azure Portal global.
Azure Government|Introducción |[Conexión a Azure Government con la CLI de Azure](/azure/azure-government/documentation-government-get-started-connect-with-cli)|Obtenga acceso a los recursos y comience a administrarlos en Azure Government.

## <a name="see-also"></a>Consulte también

* [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
* [Lista de referencia de comandos completa para la CLI de Azure](/cli/azure/reference-index)
* [Servicios que se pueden administrar con la CLI de Azure](azure-services-the-azure-cli-can-manage.md)
