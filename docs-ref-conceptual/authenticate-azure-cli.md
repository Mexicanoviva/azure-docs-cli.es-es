---
title: "Inicio de sesión con la CLI de Azure 2.0"
description: "Inicio de sesión con la CLI de Azure 2.0 de forma interactiva o con credenciales locales"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 02/13/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 92c96b7e969de686689ef02bf068392b9f565698
ms.sourcegitcommit: 29d7366a0902488f4f4d39c2cb0e89368d5186ea
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/08/2018
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

Proporcione sus credenciales en la línea de comandos.

> [!Note]
> Este enfoque no es compatible con cuentas de Microsoft o cuentas que tienen habilitada la autenticación en dos fases.

```azurecli
az login -u <username> -p <password>
```

## <a name="log-in-with-a-specific-tenant"></a>Inicie sesión con un inquilino específico

Si trabaja con varios inquilinos, puede usar el argumento `--tenant` para seleccionar el inquilino con el que iniciará sesión. El valor de este argumento puede ser un dominio `.onmicrosoft.com` o el identificador de objeto de Azure del inquilino. Puede iniciar sesión de forma interactiva o proporcionar las credenciales con los argumentos `--user` y `--password`. 

```
az login --tenant <tenant>
```

## <a name="logging-in-with-a-service-principal"></a>Inicio de sesión con una entidad de servicio

Las entidades de servicio son cuentas no asociadas a un usuario concreto, las cuales pueden tener permisos asignados mediante roles predefinidos. La autenticación con una entidad de servicio es la mejor manera de escribir scripts o programas seguros, lo que le permite aplicar las restricciones de permisos y la información de credenciales estáticas almacenadas de modo local. Para más información sobre las entidades de servicio, consulte [Creación de una entidad de servicio de Azure con la CLI de Azure](create-an-azure-service-principal-azure-cli.md).

Para iniciar sesión con una entidad de servicio, proporcione el nombre de usuario, la contraseña o el archivo de certificado PEM y el inquilino asociado a la entidad de servicio:

```azurecli
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

El valor del inquilino es el inquilino de Azure Active Directory asociado a la entidad de servicio. Puede ser un dominio `.onmicrosoft.com` o el identificador de objeto de Azure del inquilino.
Para obtener el identificador de objeto de inquilino del inicio de sesión actual, use este comando:

```azurecli
az account show --query 'tenantId' -o tsv
```
