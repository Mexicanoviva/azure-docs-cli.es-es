---
title: Extensiones disponibles para la CLI de Azure
description: Lista completa de las extensiones oficialmente admitidas por la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: a7eec3fc523b4c24b16802d831566fd272ae63fc
ms.sourcegitcommit: 943598f8bf05ee058593ca0d72aec507aa26c242
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/28/2019
ms.locfileid: "56963449"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensiones disponibles para la CLI de Azure

Este artículo es una lista completa de las extensiones disponibles para la CLI de Azure que mantiene Microsoft.

La lista de extensiones también está disponible en la CLI. Para obtenerla, ejecute [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| NOMBRE | Versión | Resumen | Vista previa |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Administración de las extensiones de supervisión mejorada de Azure para SAP. |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.2.3 | Proporciona una versión preliminar de las futuras características de AKS | Sí |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Compatibilidad con alias de comandos | Sí |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Proporciona una versión preliminar de las futuras características de configuración de aplicaciones. | Sí |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 3.0.1 | Comandos adicionales para trabajar con el servicio Azure Batch |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.6.1 | Proporciona una capa de comandos en el plano de datos para Azure IoT Hub, IoT Edge e IoT Device Provisioning Service. |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.3.0 | Herramientas para administrar Azure DevOps. | Sí |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.1.1 | Administración de los recursos de Azure Firewall. | Sí |
| [botservice](https://github.com/Azure/azure-cli-extensions) | 0.4.3 | Correcciones de errores para los problemas en el módulo nativo de comandos de la CLI botservice. | Sí |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.6 | Comandos adicionales para simplificar los flujos de trabajo de bases de datos de Azure. | Sí |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces proporciona a los equipos una experiencia de desarrollo en Kubernetes iterativa y rápida. | Sí |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.6.0 | Compatibilidad con nuevos escenarios de Database Migration Service. | Sí |
| [dns](https://github.com/Azure/azure-cli-extensions) | 0.0.2 | Extensión de la CLI de Azure para las zonas DNS |  |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.0 | Compatibilidad con las características de Azure EventGrid versión 2018-09-15-preview | Sí |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Administración de circuitos ExpressRoute con características en versión preliminar. | Sí |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.0 | Administre circuitos ExpressRoute del cliente mediante una conexión cruzada de ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Consultas inteligentes para obtener información de la CLI. | Sí |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 0.1.1 | Administración de redes de Front Door. | Sí |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.0.9 | Compatibilidad para copiar imágenes de máquina virtual administradas entre regiones |  |
| [interactive](https://github.com/Azure/azure-cli) | 0.4.1 | Shell interactivo de la línea de comandos de Microsoft Azure | Sí |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Comandos de Azure Key Vault en versión preliminar. | Sí |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.3 | Compatibilidad con las funcionalidades de consulta de Azure Log Analytics. | Sí |
| [managementgroups](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensión de la CLI de Azure para los grupos de administración |  |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Compatibilidad con la versión preliminar de administración de partners. |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.2 | Compatibilidad con Microsoft Azure Service Fabric Mesh (versión preliminar pública). | Sí |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Comandos para administrar zonas DNS privadas. | Sí |
| [rdbms-vnet](https://github.com/Azure/azure-cli-extensions) | 10.0.0 | Compatibilidad para reglas de red virtual en recursos de Azure MySQL y Azure PostgreSQL |  |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 0.1.8 | Se admite la consulta de recursos de Azure con Resource Graph. | Sí |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.3.4 | Comandos adicionales para trabajar con instancias de SAP Hana en Azure. |  |
| [signalr](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Compatibilidad con la versión preliminar de la administración de signalr. | Sí |
| [sqlvm-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/sqlvm-preview) | 0.1.0 | Herramientas para administrar máquinas virtuales SQL, grupos y agentes de escucha de grupo de disponibilidad. | Sí |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.2 | Proporciona una versión preliminar de las características de almacenamiento futuras. | Sí |
| [suscripción](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Compatibilidad con la versión preliminar de la administración de suscripciones. |  |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Administración de TAP de red virtual (VTAP). | Sí |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.0 | Administración de redes WAN virtuales, concentradores, puertas de enlace de VPN y sitios de VPN. | Sí |
| [webapp](https://github.com/Azure/azure-cli-extensions) | 0.2.16 | Comandos adicionales para Azure App Service. | Sí |