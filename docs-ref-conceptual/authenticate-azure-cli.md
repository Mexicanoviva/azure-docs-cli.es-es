---
title: Inicio de sesión con la CLI de Azure
description: Inicio de sesión con la CLI de Azure de forma interactiva o con credenciales locales
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/22/2019
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.component: authentication
ms.openlocfilehash: 234c53f27ba365550e6502b8410aced57eb9ff4e
ms.sourcegitcommit: 334a1da92a73e42e715e33470057f4194f10b2ea
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/18/2019
ms.locfileid: "59724581"
---
# <a name="sign-in-with-azure-cli"></a>Inicio de sesión con la CLI de Azure 

Hay varios tipos de autenticación para la CLI de Azure. La manera más fácil de empezar a trabajar es [Azure Cloud Shell](/azure/cloud-shell/overview), que inicia sesión automáticamente.
De forma local, puede iniciar sesión interactivamente en el explorador con el comando [az login](/cli/azure/reference-index#az-login). Al escribir scripts, el enfoque recomendado es usar entidades de servicio. Para proteger la automatización, conceda los permisos adecuados necesarios a una entidad de servicio.

La CLI no almacena ninguna de la información de inicio de sesión. En su lugar, Azure genera y almacena un [token de autenticación](https://docs.microsoft.com/en-us/azure/active-directory/develop/v1-id-and-access-tokens#refresh-tokens). A partir de agosto de 2018, este token se revoca después de 90 días de inactividad, pero este valor lo puede cambiar Microsoft o el administrador de inquilinos. Una vez revocado el token, recibirá un mensaje desde la CLI indicando que debe volver a iniciar sesión.

Después de iniciar sesión, los comandos de la CLI se ejecutan en su suscripción predeterminada. Si tiene varias suscripciones, puede [cambiar la suscripción predeterminada](manage-azure-subscriptions-azure-cli.md).

## <a name="sign-in-interactively"></a>Inicio sesión interactivo

El método de autenticación predeterminado de la CLI de Azure usa un explorador web y un token de acceso para iniciar sesión.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="sign-in-with-credentials-on-the-command-line"></a>Inicie sesión con sus credenciales en la línea de comandos.

Proporcione sus credenciales de usuario de Azure en la línea de comandos.

> [!Note]
> Este enfoque no es compatible con cuentas de Microsoft o cuentas que tienen habilitada la autenticación en dos fases.

```azurecli-interactive
az login -u <username> -p <password>
```

> [!IMPORTANT]
> Si desea evitar que se muestre la contraseña en la consola y está usando `az login` de forma interactiva, utilice el comando `read -s` en `bash`.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> En PowerShell, use el cmdlet `Get-Credential`.
>
> ```powershell
> $AzCred = Get-Credential -UserName <username>
> az login -u $AzCred.UserName -p $AzCred.GetNetworkCredential().Password
> ```

## <a name="sign-in-with-a-service-principal"></a>Inicio de sesión con una entidad de servicio

Las entidades de servicio son cuentas no asociadas a un usuario concreto, las cuales pueden tener permisos asignados mediante roles predefinidos. La autenticación con una entidad de servicio es la mejor manera de escribir scripts o programas seguros, lo que le permite aplicar las restricciones de permisos y la información de credenciales estáticas almacenadas de modo local. Para más información sobre las entidades de servicio, consulte [Creación de una entidad de servicio de Azure con la CLI de Azure](create-an-azure-service-principal-azure-cli.md).

Para iniciar sesión con una entidad de servicio, necesita:

* La dirección URL o el nombre asociado a la entidad de servicio.
* La contraseña de la entidad de servicio o el certificado X509 utilizado para crear la entidad de servicio con el formato PEM.
* El inquilino asociado con la entidad de servicio, como un dominio de `.onmicrosoft.com` o un identificador de objeto de Azure.

> [!IMPORTANT]
>
> Si la entidad de servicio utiliza un certificado que se almacena en Key Vault, la clave privada del certificado debe estar disponible sin iniciar sesión en Azure. Para recuperar una clave privada para su uso sin conexión, use [az keyvault secret show](/cli/azure/keyvault/secret).

```azurecli-interactive
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

> [!IMPORTANT]
> Si desea evitar que se muestre la contraseña en la consola y está usando `az login` de forma interactiva, utilice el comando `read -s` en `bash`.
>
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> En PowerShell, use el cmdlet `Get-Credential`.
>
> ```powershell
> $AzCred = Get-Credential -UserName <app-url>
> az login --service-principal -u $AzCred.UserName -p $AzCred.GetNetworkCredential().Password --tenant <tenant>
> ```

## <a name="sign-in-with-a-different-tenant"></a>Inicio de sesión con un inquilino diferente

Puede seleccionar un inquilino para iniciar sesión con el argumento `--tenant`. El valor de este argumento puede ser un dominio `.onmicrosoft.com` o el identificador de objeto de Azure del inquilino. Tanto el método de inicio de sesión interactivo como el de línea de comandos funcionan con `--tenant`.

```azurecli-interactive
az login --tenant <tenant>
```

## <a name="sign-in-with-a-managed-identity"></a>Inicio de sesión con una identidad administrada

En los recursos configurados para las identidades administradas para los recursos de Azure, puede iniciar sesión con la identidad administrada. El inicio de sesión con la identidad del recurso se realiza mediante la marca `--identity`.

```azurecli-interactive
az login --identity
```

Para más información acerca de las identidades administradas para los recursos de Azure, consulte [Configuración de identidades administradas para recursos de Azure](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/qs-configure-cli-windows-vm) y [Uso de identidades administradas para recursos de Azure para el inicio de sesión](https://docs.microsoft.com/en-us/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-sign-in).
