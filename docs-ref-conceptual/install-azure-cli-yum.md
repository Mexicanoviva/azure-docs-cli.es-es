---
title: Instalación de la CLI de Azure en Linux con yum
description: Cómo instalar la CLI de Azure con yum
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: faa1855efe9651ee104880740338c30e7dd84810
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593241"
---
# <a name="install-azure-cli-with-yum"></a>Instalación de la CLI de Azure con yum

Para distribuciones Linux con `yum`, como RHEL, Fedora o CentOS, hay un paquete de la CLI de Azure. Este paquete se ha probado con RHEL 7, Fedora 19 y versiones posteriores y CentOS 7.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalación

1. Importe la clave del repositorio de Microsoft.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Cree la información del repositorio `azure-cli` local.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Realice la instalación con el comando `yum install`.

   ```bash
   sudo yum install azure-cli
   ```

Después, ejecute la CLI de Azure con el comando `az`. Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solución de problemas

Estos son algunos problemas comunes que se han observado cuando se instala con `yum`. Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).

[!INCLUDE[troubleshoot-wsl.md](includes/troubleshoot-wsl.md)]

## <a name="update"></a>Actualizar

Actualice la CLI de Azure con el comando `yum update`.

```bash
sudo yum update azure-cli
```

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Elimine el paquete de su equipo.

   ```bash
   sudo yum remove azure-cli
   ```

2. Si no tiene previsto volver a instalar la CLI, elimine la información del repositorio.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
