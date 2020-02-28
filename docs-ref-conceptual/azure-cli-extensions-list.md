---
title: Extensiones disponibles para la CLI de Azure
description: Lista completa de las extensiones oficialmente admitidas por la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/17/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: bac834704f4e965d44a8790f5a4fa59254357373
ms.sourcegitcommit: aff84ab984e2d129927888e6b854ed7a5ccaaf59
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/21/2020
ms.locfileid: "77520778"
---
# <a name="available-extensions-for-the-azure-cli"></a>Extensiones disponibles para la CLI de Azure

Este artículo es una lista completa de las extensiones disponibles para la CLI de Azure que mantiene Microsoft.

La lista de extensiones también está disponible en la CLI. Para obtenerla, ejecute [az extension list-available](/cli/azure/extension?view=azure-cli-latest#az-extension-list-available):

```azurecli-interactive
az extension list-available --output table
```

| Nombre | Versión | Resumen | Vista previa |
|------|---------|---------|---------|
| [aem](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Administración de las extensiones de supervisión mejorada de Azure para SAP. |  |
| [aks-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/aks-preview) | 0.4.29 | Proporciona una versión preliminar de las futuras características de AKS | Sí |
| [alias](https://github.com/Azure/azure-cli-extensions) | 0.5.2 | Compatibilidad con alias de comandos | Sí |
| [appconfig](https://github.com/Azure/azure-cli-extensions) | 0.5.0 | Proporciona una versión preliminar de las futuras características de configuración de aplicaciones. | Sí |
| [application-insights](https://github.com/Azure/azure-cli-extensions/tree/master/src/application-insights) | 0.1.3 | Compatibilidad para administrar componentes de Application Insights y consultar las métricas, los eventos y los registros de esos componentes. | Sí |
| [azure-batch-cli-extensions](https://github.com/Azure/azure-batch-cli-extensions) | 5.0.0 | Comandos adicionales para trabajar con el servicio Azure Batch |  |
| [azure-cli-iot-ext](https://github.com/azure/azure-iot-cli-extension) | 0.8.9 | Extensión de Azure IoT para la CLI de Azure. |  |
| [azure-cli-ml](https://docs.microsoft.com/azure/machine-learning/service/) | 1.0.85 | Módulo de comandos de AzureML de la herramienta de línea de comandos de Microsoft Azure |  |
| [azure-devops](https://github.com/Microsoft/azure-devops-cli-extension) | 0.17.0 | Herramientas para administrar Azure DevOps. |  |
| [azure-firewall](https://github.com/Azure/azure-cli-extensions/tree/master/src/azure-firewall) | 0.3.0 | Administración de los recursos de Azure Firewall. | Sí |
| [connectedmachine](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensión Connectedmachine de las herramienta de línea de comandos de Microsoft Azure | Sí |
| [connection-monitor-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/connection-monitor-preview) | 0.1.0 | Extensión de supervisión de la línea de comandos de Microsoft Azure Command-Line V2 | Sí |
| [db-up](https://github.com/Azure/azure-cli-extensions/tree/master/src/db-up) | 0.1.13 | Comandos adicionales para simplificar los flujos de trabajo de bases de datos de Azure. | Sí |
| [dev-spaces](https://github.com/Azure/azure-cli-extensions) | 1.0.4 | Dev Spaces proporciona a los equipos una experiencia de desarrollo en Kubernetes iterativa y rápida. |  |
| [dev-spaces-preview](https://github.com/Azure/azure-cli-extensions) | 0.1.6 | Dev Spaces proporciona a los equipos una experiencia de desarrollo en Kubernetes iterativa y rápida. | Sí |
| [dms-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/dms-preview) | 0.9.0 | Compatibilidad con nuevos escenarios de Database Migration Service. | Sí |
| [eventgrid](https://github.com/Azure/azure-cli-extensions) | 0.4.4 | Módulo de comandos de EventGrid para la herramienta de línea de comandos de Microsoft Azure. | Sí |
| [express-route](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route) | 0.1.3 | Administración de circuitos ExpressRoute con características en versión preliminar. | Sí |
| [express-route-cross-connection](https://github.com/Azure/azure-cli-extensions/tree/master/src/express-route-cross-connection) | 0.1.1 | Administre circuitos ExpressRoute del cliente mediante una conexión cruzada de ExpressRoute. |  |
| [find](https://github.com/Azure/azure-cli-extensions/tree/master/src/find) | 0.3.0 | Consultas inteligentes para obtener información de la CLI. | Sí |
| [front-door](https://github.com/Azure/azure-cli-extensions/tree/master/src/front-door) | 1.0.2 | Administración de redes de Front Door. |  |
| [hack](https://github.com/Azure/azure-cli-extensions) | 0.4.1 | Extensión Hack de la herramienta de línea de comandos de Microsoft Azure | Sí |
| [healthcareapis](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Extensión HealthCareApis de la herramienta de línea de comandos de Microsoft Azure |  |
| [image-copy-extension](https://github.com/Azure/azure-cli-extensions) | 0.2.3 | Compatibilidad para copiar imágenes de máquina virtual administradas entre regiones |  |
| [interactive](https://github.com/Azure/azure-cli) | 0.4.3 | Shell interactivo de la línea de comandos de Microsoft Azure | Sí |
| [internet-analyzer](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc4 | Extensión Internet Analyzer de las herramienta de línea de comandos de Microsoft Azure | Sí |
| [ip-group](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensión IpGroup de la herramienta de línea de comandos de Microsoft Azure |  |
| [keyvault-preview](https://github.com/Azure/azure-keyvault-cli-extension) | 0.1.3 | Comandos de Azure Key Vault en versión preliminar. | Sí |
| [log-analytics](https://github.com/Azure/azure-cli-extensions/tree/master/src/log-analytics) | 0.1.4 | Compatibilidad con las funcionalidades de consulta de Azure Log Analytics. | Sí |
| [maintenance](https://github.com/Azure/azure-cli-extensions) | 1.0.0 | Compatibilidad con la versión preliminar de Azure Maintenance Management. | Sí |
| [managementpartner](https://github.com/Azure/azure-cli-extensions) | 0.1.2 | Compatibilidad con la versión preliminar de administración de partners. |  |
| [mesh](https://github.com/Azure/azure-cli-extensions) | 0.10.6 | Compatibilidad con Microsoft Azure Service Fabric Mesh (versión preliminar pública). | Sí |
| [mixed-reality](https://github.com/Azure/azure-cli-extensions) | 0.0.1 | Extensión de la CLI de Azure de Mixed Reality. |  |
| [netappfiles-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/netappfiles-preview) | 0.3.2 | Proporciona una versión preliminar de las nuevas características de Azure NetApp Files (ANF). | Sí |
| [notification-hub](https://github.com/Azure/azure-cli-extensions) | 0.1.0 | Extensión de centro de notificaciones de la línea de comandos de Microsoft Azure | Sí |
| [peering](https://github.com/Azure/azure-cli-extensions) | 0.1.0rc1 | Extensión Peering de la herramienta de línea de comandos de Microsoft Azure | Sí |
| [privatedns](https://github.com/Azure/azure-cli-extensions) | 0.1.1 | Comandos para administrar zonas DNS privadas. | Sí |
| [resource-graph](https://github.com/Azure/azure-cli-extensions/tree/master/src/resource-graph) | 1.0.0 | Se admite la consulta de recursos de Azure con Resource Graph. |  |
| [sap-hana](https://github.com/Azure/azure-hanaonazure-cli-extension) | 0.5.5 | Comandos adicionales para trabajar con instancias de SAP Hana en Azure. |  |
| [spring-cloud](https://github.com/Azure/azure-cli-extensions) | 0.2.0 | Extensión spring-cloud de la herramienta de línea de comandos de Microsoft Azure | Sí |
| [storage-preview](https://github.com/Azure/azure-cli-extensions/tree/master/src/storage-preview) | 0.2.10 | Proporciona una versión preliminar de las características de almacenamiento futuras. | Sí |
| [suscripción](https://github.com/Azure/azure-cli-extensions) | 0.1.3 | Compatibilidad con la versión preliminar de la administración de suscripciones. |  |
| [support](https://github.com/azure/azure-cli-extensions/tree/master/src/support) | 0.1.0 | Extensión de soporte de las herramientas de línea de comandos de Microsoft Azure | Sí |
| [virtual-network-tap](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-network-tap) | 0.1.0 | Administración de TAP de red virtual (VTAP). | Sí |
| [virtual-wan](https://github.com/Azure/azure-cli-extensions/tree/master/src/virtual-wan) | 0.1.2 | Administración de redes WAN virtuales, concentradores, puertas de enlace de VPN y sitios de VPN. | Sí |
| [vm-repair](https://github.com/Azure/azure-cli-extensions/tree/master/src/vm-repair) | 0.2.5 | Comandos de reparación automática para corregir las máquinas virtuales. |  |
| [vmware-cs](https://github.com/Azure/az-vmware-cli) | 0.2.0 | Administrar la solución de VMware en Azure. | Sí |
| [webapp](https://github.com/Azure/azure-cli-extensions/tree/master/src/webapp) | 0.2.24 | Comandos adicionales para Azure App Service. | Sí |