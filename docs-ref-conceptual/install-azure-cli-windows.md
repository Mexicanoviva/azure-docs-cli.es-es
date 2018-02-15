---
title: "Instalación de la CLI de Azure para Windows"
description: "Instalación de la CLI de Azure 2.0 en Windows"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 3e732ea7fae118ddb1564bed28d54d15bab4f7f0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Instalación de la CLI de Azure 2.0 en Windows

En Windows, el archivo binario de la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.
Si está ejecutando el subsistema de Windows para Linux (WSL), hay paquetes disponibles para la distribución de Linux. Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.

## <a name="install-or-update"></a>Instalación o actualización

El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows.

> [!div class="nextstepaction"]
> [Descargue el instalador MSI](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)

Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".

Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell. PowerShell ofrece algunas características de la función de autocompletar que no están disponibles desde CMD.

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar".

> [!div class="nextstepaction"]
> [Descargue el instalador MSI](https://azurecliprod.blob.core.windows.net/msi/azure-cli-latest.msi)
