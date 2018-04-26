---
title: Instalación de la CLI de Azure para Windows
description: Instalación de la CLI de Azure 2.0 en Windows
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/29/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 30b9621c82af259e3de762127fd20b31eb249234
ms.sourcegitcommit: 0e9aafa07311526f43661c8bd3a7eba7cbc2caed
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/20/2018
---
# <a name="install-azure-cli-20-on-windows"></a>Instalación de la CLI de Azure 2.0 en Windows

En Windows, el archivo binario de la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.
Si está ejecutando el subsistema de Windows para Linux (WSL), hay paquetes disponibles para la distribución de Linux. Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.

## <a name="install-or-update"></a>Instalación o actualización

El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows.

> [!div class="nextstepaction"]
> [Descargue el instalador MSI](https://aka.ms/installazurecliwindows)

Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".

Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell. PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows. Para iniciar sesión, ejecute el comando `az login`.

```azurecli
az login
```

Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar".

> [!div class="nextstepaction"]
> [Descargue el instalador MSI](https://aka.ms/installazurecliwindows)
