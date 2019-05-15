---
title: Instalación de la CLI de Azure para Windows
description: Cómo instalar la CLI de Azure en Windows
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/01/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5c499800e49dcdc536337e7655ec1ee280d48f2
ms.sourcegitcommit: 65bf8561a6e047e4eab52186e066a2e8c21f1d40
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2019
ms.locfileid: "65240549"
---
# <a name="install-azure-cli-on-windows"></a>Instalación de la CLI de Azure en Windows

En Windows, la CLI de Azure se instala mediante un archivo MSI que proporciona acceso a la CLI a través del símbolo del sistema de Windows (CMD) o PowerShell.
Si se va a instalar el subsistema de Windows para Linux (WSL), hay paquetes disponibles para su distribución de Linux. Consulte la [página principal de instalación](install-azure-cli.md) para obtener la lista de administradores de paquetes admitidos o información para instalar manualmente en WSL.

[!INCLUDE [current-version](includes/current-version.md)]

## <a name="install-or-update"></a>Instalación o actualización

El archivo MSI distribuible se usa para instalar o actualizar la CLI de Azure en Windows. No es necesario desinstalar las versiones actuales antes de usar el instalador MSI.

> [!div class="nextstepaction"]
> [Descargue el instalador MSI](https://aka.ms/installazurecliwindows)

Cuando el instalador le pregunte si puede realizar cambios en el equipo, haga clic en la casilla "Sí".

Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell. PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows. Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

La CLI de Azure se desinstala desde la lista "Aplicaciones y características" de Windows. Para desinstalar:

| Plataforma | Instrucciones |
|---|---|
| Windows 10 | Inicio > Configuración > Aplicaciones |
| Windows 8<br/>Windows 7 | Inicio > Panel de Control > Programas > Desinstalar un programa |

En esta pantalla, escriba __CLI de Azure__ en la barra de búsqueda de programas. El programa para desinstalar aparece como __Microsoft CLI 2.0 para Azure__. Seleccione esta aplicación y haga clic en el botón `Uninstall`.

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
