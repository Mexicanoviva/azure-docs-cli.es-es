---
title: "Instalación de la CLI de Azure 2.0 con zypper"
description: "Instalación de la CLI de Azure 2.0 con zypper"
keywords: "cli de azure, instalación de la cli de azure, azure cli zypper, azure cli opensuse, azure cli sle"
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
ms.openlocfilehash: c01679ccb77880f1f628f4e48683d8ff030a568b
ms.sourcegitcommit: 905939cc44764b4d1cc79a9b36c0793f7055a686
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2017
---
# <a name="install-azure-cli-20-with-zypper"></a>Instalación de la CLI de Azure 2.0 con zypper

Si está ejecutando una distribución que incluye `zypper`, como OpenSUSE o SLE, hay un paquete disponible para la CLI de Azure que se puede instalar en el sistema.

> [!NOTE]
> Debe tener Python 2.7.x o Python 3.x para poder usar la CLI. Si la distribución no tiene uno de los dos paquetes, [instale Python](https://www.python.org/downloads/).

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

Puede ejecutar la CLI con el comando `az`.

## <a name="update"></a>Actualizar

Puede actualizar el paquete con el comando `zypper update`.

```bash
sudo zypper refresh
sudo zypper update azure-cli
```

## <a name="uninstall"></a>Desinstalación

Si alguna vez decide desinstalar la CLI, sentimos que se marche. Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella. Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos. También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).

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
