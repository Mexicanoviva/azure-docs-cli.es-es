---
title: "Instalación de la CLI de Azure 2.0 con yum"
description: "Instalación de la CLI de Azure 2.0 con yum"
keywords: CLI de Azure, instalar la CLI de Azure, azure yum, azure rhel, azure fedora, azure centos
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
ms.openlocfilehash: f0d5effcd8315094b30050a35119e41eddf89961
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2017
---
# <a name="install-azure-cli-20-with-yum"></a>Instalación de la CLI de Azure 2.0 con yum

Si está ejecutando una distribución que viene con `yum`, como RHEL, Fedora o CentOS, hay un paquete disponible para la CLI de Azure que se puede instalar en el sistema.

[!INCLUDE [linux-install-requirements.md](includes/linux-install-requirements.md)]

## <a name="install"></a>Instalación

1. Importe la clave del repositorio de Microsoft:

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. Cree la información del repositorio `azure-cli` local:

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. Actualice el índice del paquete `yum` e instálelo:

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

Ejecute la CLI de Azure con el comando `az`.

## <a name="update"></a>Actualizar

Actualice la CLI de Azure con el comando `yum update`.

```bash
yum check-update
sudo yum update azure-cli
```

## <a name="uninstall"></a>Desinstalación

Si alguna vez decide desinstalar la CLI, sentimos que se marche. Antes de desinstalar, use el comando `az feedback` para enviarnos algunos de los motivos por los que eligió desinstalar la CLI y cómo podemos mejorar su experiencia con ella. Queremos asegurarnos de que la CLI de Azure sea fácil de usar y tan libre de errores como podamos. También puede [notificar un problema en github](https://github.com/Azure/azure-cli/issues).

1. Elimine el paquete de su equipo.

   ```bash
   sudo yum remove azure-cli
   ```

2. Si no piensa volver a instalar la CLI, elimine la información del repositorio.

   ```bash
   sudo rm /etc/yum.repos.d/azure-cli.repo
   ```

3. Si ha eliminado la información del repositorio, elimine también la clave de la firma GPG de Microsoft.

  ```bash
  MSFT_KEY=`rpm -qa gpg-pubkey /* --qf "%{version}-%{release} %{summary}\n" | grep Microsoft | awk '{print $1}'`
  sudo rpm -e --allmatches gpg-pubkey-$MSFT_KEY
  ```
