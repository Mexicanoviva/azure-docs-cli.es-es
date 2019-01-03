---
title: Instalación de la CLI de Azure para Windows
description: Cómo instalar la CLI de Azure en Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: ff4ed838351167410c75c046dc8f615faa0930f5
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593224"
---
# <a name="install-azure-cli-on-windows"></a>Instalación de la CLI de Azure en Windows

En Windows, la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.
Si se va a instalar el subsistema de Windows para Linux (WSL), hay paquetes disponibles para su distribución de Linux. Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.

## <a name="install-or-update"></a>Instalación o actualización

El archivo MSI distribuible se usa para instalar, actualizar y desinstalar el comando `az` en Windows.

> [!div class="nextstepaction"]
> [Descargue el instalador MSI](https://aka.ms/installazurecliwindows)

Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".

Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell. PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows. Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

Para desinstalar, puede volver a ejecutar el archivo MSI y elija la opción "Desinstalar".

> [!div class="nextstepaction"]
> [Descargue el instalador MSI](https://aka.ms/installazurecliwindows)

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
