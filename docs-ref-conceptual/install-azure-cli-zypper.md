---
title: Instalación de la CLI de Azure 2.0 en Linux con zypper
description: Instalación de la CLI de Azure 2.0 con zypper
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 01/29/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 3a1e82dc666cd034d0cc4320a8b99dd6a9a14b6d
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2018
---
# <a name="install-azure-cli-20-with-zypper"></a>Instalación de la CLI de Azure 2.0 con zypper

Si está ejecutando una distribución que viene con `zypper`, como openSUSE o SLES, hay un paquete disponible para la CLI de Azure. Este paquete se ha probado con openSUSE 42.2 y SLES 12 SP 2.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalación

1. Instale `curl`:

   ```bash
   sudo zypper refresh
   sudo zypper install -y curl
   ```

2. Importe la clave del repositorio de Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

3. Cree la información del repositorio `azure-cli` local:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

4. Actualice el índice del paquete `zypper` e instálelo:

   ```bash
   sudo zypper refresh
   sudo zypper install -y azure-cli
   ```

Después, ejecute la CLI de Azure con el comando `az`. Para iniciar sesión, ejecute el comando `az login`.

```azurecli
az login
```

Para más información acerca de los diferentes métodos de inicio de sesión, consulte [Inicio de sesión con la CLI de Azure 2.0](authenticate-azure-cli.md).

## <a name="update"></a>Actualizar

Puede actualizar el paquete con el comando `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Desinstalación

[!INCLUDE [uninstall-boilerplate.md](includes/uninstall-boilerplate.md)]

1. Elimine el paquete de su equipo.

    ```bash
    sudo zypper remove -y azure-cli
    ```

2. Si no piensa volver a instalar la CLI, elimine la información del repositorio.

  ```bash
  sudo rm /etc/zypp/repos.d/azure-cli.repo
  ```

3. Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```

