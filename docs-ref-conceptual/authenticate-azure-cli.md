---
title: Inicio de sesión con la CLI de Azure 2.0
description: Inicio de sesión con la CLI de Azure 2.0 de forma interactiva o con credenciales locales
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/13/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.service: active-directory
ms.component: authentication
ms.openlocfilehash: db676c7d81d1ea5628ebb52f3bcead763c5527f9
ms.sourcegitcommit: ae72b6c8916aeb372a92188090529037e63930ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2018
---
# <a name="log-in-with-azure-cli-20"></a>Inicio de sesión con la CLI de Azure 2.0

Hay varias maneras de iniciar sesión y autenticarse con la CLI de Azure. La manera más sencilla de empezar es iniciar sesión de forma interactiva mediante el explorador con Azure Cloud Shell o con el comando `az login`.
El método recomendado es el uso de entidades de servicio, que son cuentas con permisos restringidos. Mediante la concesión de los permisos adecuados necesarios a una entidad de servicio, puede asegurarse de que sus scripts de automatización son aún más seguros.

Ninguna información de credenciales privada se almacena localmente. En su lugar, Azure genera un token de autenticación que se almacena. Después de iniciar sesión, el token de inicio de sesión es válido hasta que transcurren 14 días sin ser usado. En ese momento, debe volver a autenticarse.

Después de iniciar sesión, los comandos de la CLI se ejecutan con su suscripción predeterminada. Si tiene más de una suscripción, puede [cambiar la suscripción predeterminada](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-log-in"></a>Inicio de sesión interactivo

Inicie sesión de forma interactiva desde el explorador web.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Línea de comandos

Proporcione sus credenciales de usuario de Azure en la línea de comandos.

> [!Note]
> Este enfoque no es compatible con cuentas de Microsoft o cuentas que tienen habilitada la autenticación en dos fases.

```azurecli
az login -u <username> -p <password>
```

> [!IMPORTANT]
> Si desea evitar que se muestre la contraseña en la consola y está usando `az login` de forma interactiva, utilice el comando `read -s` en `bash`.
> 
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login -u <username> -p $AZ_PASS
> ```
>
> En PowerShell, use el cmdlet `Read-Host -AsSecureString` y proteja la conversión de cadenas.
> 
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login -u <username> -p $AzPass;
> $AzPass = ""
> ```

## <a name="log-in-with-a-specific-tenant"></a>Inicie sesión con un inquilino específico

Si trabaja con varios inquilinos, puede usar el argumento `--tenant` para seleccionar el inquilino con el que iniciará sesión. El valor de este argumento puede ser un dominio `.onmicrosoft.com` o el identificador de objeto de Azure del inquilino. Puede iniciar sesión de forma interactiva o proporcionar las credenciales con los argumentos `--user` y `--password`. 

```
az login --tenant <tenant>
```

## <a name="log-in-with-a-service-principal"></a>Inicio de sesión con una entidad de servicio

Las entidades de servicio son cuentas no asociadas a un usuario concreto, las cuales pueden tener permisos asignados mediante roles predefinidos. La autenticación con una entidad de servicio es la mejor manera de escribir scripts o programas seguros, lo que le permite aplicar las restricciones de permisos y la información de credenciales estáticas almacenadas de modo local. Para más información sobre las entidades de servicio, consulte [Creación de una entidad de servicio de Azure con la CLI de Azure](create-an-azure-service-principal-azure-cli.md).

Para iniciar sesión con una entidad de servicio, proporcione el nombre de usuario, la contraseña o el archivo de certificado PEM y el inquilino asociado a la entidad de servicio:

```azurecli
az login --service-principal -u <app-url> -p <password-or-cert> --tenant <tenant>
```

El valor del inquilino es el inquilino de Azure Active Directory asociado a la entidad de servicio. Puede ser un dominio `.onmicrosoft.com` o el identificador de objeto de Azure del inquilino.
Para obtener el identificador de objeto de inquilino del inicio de sesión actual, use este comando:

```azurecli
az account show --query 'tenantId' -o tsv
```

> [!IMPORTANT]
> Si desea evitar que se muestre la contraseña en la consola y está usando `az login` de forma interactiva, utilice el comando `read -s` en `bash`.
> 
> ```bash
> read -sp "Azure password: " AZ_PASS && echo && az login --service-principal -u <app-url> -p $AZ_PASS --tenant <tenant>
> ```
>
> En PowerShell, use el cmdlet `Read-Host -AsSecureString` y proteja la conversión de cadenas.
> 
> ```powershell
> $securePass =  Read-Host "Azure password: " -AsSecureString;
> $AzPass = [Runtime.InteropServices.Marshal]::PtrToStringAuto([Runtime.InteropServices.Marshal]::SecureStringToBSTR($securePass));
> az login --service-principal -u <app-url> -p $AzPass --tenant <tenant>;
> $AzPass = ""
> ```
