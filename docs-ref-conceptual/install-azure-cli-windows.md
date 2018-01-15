---
title: "Instalación de la CLI de Azure para Windows"
description: "Instalación de la CLI de Azure 2.0 en Windows"
keywords: CLI de Azure, instalar la CLI de Azure, instalar azure windows, azure cli windows, azure windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 11/01/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ROBOTS: NOINDEX,NOFOLLOW
ms.openlocfilehash: 247ae43813ca9ca7b7b98ebd8e933e02989c6649
ms.sourcegitcommit: 3eef136ae752eb90c67af604d4ddd298d70b1c9d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/06/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Instalación de la CLI de Azure 2.0 en Windows

En Windows, puede instalar un archivo binario nativo desde un archivo MSI, que se puede usar mediante el símbolo del sistema de Windows o PowerShell. Si está ejecutando el subsistema de Windows para Linux (WSL), hay paquetes disponibles para la distribución que se está ejecutando. Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.

## <a name="install-or-update-with-msi"></a>Instalación o actualización con MSI

El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows. También puede [descargar el instalador MSI](https://aka.ms/InstallAzureCliWindows) y, a continuación, ejecutarlo para instalar o actualizar.

Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".

Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell.

## <a name="uninstall-with-msi"></a>Desinstalación con MSI

Si alguna vez decide desinstalar la CLI, sentimos que se marche. Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella. Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos. También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).

Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar". También puede [descargar el instalador MSI](https://aka.ms/InstallAzureCliWindows) si no lo tiene disponible.
