---
title: "Inicio de sesión con la CLI de Azure 2.0"
description: "Inicie sesión con la CLI de Azure 2.0 en Linux, Mac o Windows."
keywords: "CLI de Azure 2.0, inicio de sesión, CLI de Azure, autenticación, autorizar, iniciar sesión"
author: sptramer
ms.author: stttramer
manager: routlaw
ms.date: 11/13/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: dd05868f7378673836f47e743ed4088f2efd3dca
ms.sourcegitcommit: 5db22de971cf3983785cb209d92cbed1bbd69ecf
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/14/2017
---
# <a name="log-in-with-azure-cli-20"></a>Inicio de sesión con la CLI de Azure 2.0

Hay varias maneras de iniciar sesión y autenticarse con la CLI de Azure. La manera más sencilla de empezar es iniciar sesión de forma interactiva mediante el explorador o en la línea de comandos. El enfoque recomendado consiste en usar entidades de servicio que proporcionan una manera de crear cuentas no interactivas que puede usar para manipular recursos. Mediante la concesión de los permisos adecuados necesarios a una entidad de servicio, puede asegurarse de que sus scripts de automatización son aún más seguros. 

Ninguna información de credenciales privada se almacena localmente. En su lugar, Azure genera un token de autenticación que se almacena. Después de iniciar sesión, el token de inicio de sesión local es válido hasta que transcurren 14 días sin ser usado. En ese momento, debe volver a autenticarse.

Después de iniciar sesión, los comandos de la CLI se ejecutan con su suscripción predeterminada. Si tiene más de una suscripción, quizás desee [cambiar la suscripción predeterminada](manage-azure-subscriptions-azure-cli.md).

## <a name="interactive-log-in"></a>Inicio de sesión interactivo

Inicie sesión de forma interactiva desde el explorador web.

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a>Línea de comandos

Proporcione sus credenciales en la línea de comandos.

> [!Note]
> Este enfoque no es compatible con cuentas de Microsoft o cuentas que tienen habilitada la autenticación en dos fases.

```azurecli-interactive
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a>Inicio de sesión con una entidad de servicio

Las entidades de servicio son parecidas a las cuentas de usuario a las que puede aplicar reglas con Azure Active Directory.
La autenticación con una entidad de servicio es la mejor manera de proteger el uso de los recursos de Azure de sus scripts o aplicaciones que manipulan recursos. Si aún no tiene una entidad de servicio disponible y le gustaría crear una, consulte [Creación de una entidad de servicio de Azure con la CLI de Azure](create-an-azure-service-principal-azure-cli.md).

Para iniciar sesión con una entidad de servicio, proporcione el nombre de usuario, la contraseña o el archivo de certificado PEM y el inquilino asociado a la entidad de servicio:

```azurecli-interactive
az login --service-principal -u <user> -p <password-or-cert> --tenant <tenant>
```

El valor del inquilino es el inquilino de Azure Active Directory asociado a la entidad de servicio. Puede ser un dominio .onmicrosoft.com o el identificador de objeto de Azure del inquilino.
Para obtener el identificador de objeto de inquilino del inicio de sesión actual, use este comando:

```azurecli
az account show --query 'tenanatId' -o tsv
```

