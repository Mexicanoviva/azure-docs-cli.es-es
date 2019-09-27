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
ms.openlocfilehash: 270be4c41bdb3c913e41ef1b2bb0c7c0b393aa20
ms.sourcegitcommit: 5a29ce9c0a3d7b831f22b1a13b1ae2e239e5549f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/19/2019
ms.locfileid: "71144035"
---
# <a name="install-azure-cli-with-yum"></a>Instalación de la CLI de Azure con yum

Para distribuciones Linux con `yum`, como RHEL, Fedora o CentOS, hay un paquete de la CLI de Azure. Este paquete se ha probado con RHEL 7, Fedora 19 y versiones posteriores y CentOS 7.

[!INCLUDE [current-version](includes/current-version.md)]

[!INCLUDE [rpm-warning](includes/rpm-warning.md)]

## <a name="install"></a>Instalación

1. Importe la clave del repositorio de Microsoft.

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Cree la información del repositorio `azure-cli` local.

   ```bash
   sudo sh -c 'echo -e "[azure-cli]
   name=Azure CLI
   baseurl=https://packages.microsoft.com/yumrepos/azure-cli
   enabled=1
   gpgcheck=1
   gpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Realice la instalación con el comando `yum install`.

   ```bash
   sudo yum install azure-cli
   ```

Ejecute la CLI de Azure con el comando `az`. Para iniciar sesión, use el comando [az login](/cli/azure/reference-index#az-login).

[!INCLUDE [interactive-login](includes/interactive-login.md)]

Para más información acerca de los diferentes métodos de autenticación, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="troubleshooting"></a>solución de problemas

Estos son algunos problemas comunes que se han observado cuando se instala con `yum`. Si tiene algún problema que no se trata aquí, [abra una incidencia en GitHub](https://github.com/Azure/azure-cli/issues).

### <a name="proxy-blocks-connection"></a>Conexión de bloques proxy

[!INCLUDE[configure-proxy](includes/configure-proxy.md)]

También puede configurar explícitamente `yum` para usar este servidor proxy en todo momento. Asegúrese de que las líneas siguientes aparecen en la sección `[main]` de `/etc/yum.conf`:

```yum.conf
[main]
# ...
proxy=http://[proxy]:[port] # If your proxy requires https, change http->https
proxy_username=[username] # Only required for basic auth
proxy_password=[password] # Only required for basic auth
```

Para obtener la clave de firma de Microsoft y obtener el paquete de nuestro repositorio, el servidor proxy debe permitir las conexiones HTTPS a la siguiente dirección:

* `https://packages.microsoft.com`

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

3. Si no usa otros paquetes de Microsoft, quite la clave de firma.

   ```bash
   MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
   sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
   ```

## <a name="next-steps"></a>Pasos siguientes

Ahora que ha instalado la CLI de Azure, dé un breve paseo por sus características y comandos más comunes.

> [!div class="nextstepaction"]
> [Introducción a la CLI de Azure](get-started-with-azure-cli.md)
