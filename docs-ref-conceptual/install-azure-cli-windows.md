---
title: Instalación de la CLI de Azure para Windows
description: Cómo instalar la CLI de Azure en Windows
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 05/01/2019
ms.topic: conceptual
ms.service: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: c5e9118a04b0dc608309093866307fdc7083f591
ms.sourcegitcommit: b5ecfc168489cd0d96462d6decf83e8b26a10194
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/31/2020
ms.locfileid: "80417836"
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

También puede instalar la CLI de Azure mediante PowerShell. Abra PowerShell como administrador y ejecute el siguiente comando:

   ```PowerShell
   Invoke-WebRequest -Uri https://aka.ms/installazurecliwindows -OutFile .\AzureCLI.msi; Start-Process msiexec.exe -Wait -ArgumentList '/I AzureCLI.msi /quiet'; rm .\AzureCLI.msi
   ```
Esto descargará e instalará la versión más reciente de la CLI de Azure para Windows. Si ya tiene instalada una versión, se actualizará la versión existente. Una vez completada la instalación, tendrá que volver a abrir PowerShell para usar la CLI de Azure.

Ya puede ejecutar la CLI de Azure con el comando `az` desde el símbolo del sistema de Windows o PowerShell. PowerShell ofrece algunas características de finalización que no están disponibles en el símbolo del sistema de Windows. Para iniciar sesión, ejecute el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>Solución de problemas

Estos son algunos problemas comunes que se han observado cuando se instala con Windows. Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>El servidor proxy bloquea la conexión

Si no puede descargar al instalador MSI porque el proxy está bloqueando la conexión, asegúrese de que el servidor proxy esté configurado correctamente. En Windows 10, esta configuración se administra en el panel `Settings > Network & Internet > Proxy`. Póngase en contacto con el administrador del sistema para más información sobre la configuración necesaria, o si su máquina se puede administrar mediante configuración o si requiere configuración avanzada.

> [!IMPORTANT]
> Esta configuración también es necesaria para poder tener acceso a los servicios de Azure con la CLI, PowerShell o la línea de comandos. En PowerShell, se hace con el siguiente comando:
>
> ```powershell
> (New-Object System.Net.WebClient).Proxy.Credentials = `
>   [System.Net.CredentialCache]::DefaultNetworkCredentials
> ```

Para obtener el MSI, el servidor proxy debe permitir las conexiones HTTPS a las siguientes direcciones:

* `https://aka.ms/`
* `https://azurecliprod.blob.core.windows.net/`

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

La CLI de Azure se desinstala desde la lista "Aplicaciones y características" de Windows. Para desinstalar:

| Plataforma | Instructions |
|---|---|
| Windows 10 | Inicio > Configuración > Aplicaciones |
| Windows 8<br/>Windows 7 | Inicio > Panel de Control > Programas > Desinstalar un programa |

En esta pantalla, escriba __CLI de Azure__ en la barra de búsqueda de programas. El programa para desinstalar aparece como __Microsoft CLI 2.0 para Azure__. Seleccione esta aplicación y, después, haga clic en el botón `Uninstall`.

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
