---
title: "Inicio de sesión con la CLI de Azure 2.0"
description: "Inicie sesión con la CLI de Azure 2.0 en Linux, Mac o Windows."
keywords: CLI de Azure 2.0, Linux, Mac, Windows, OS X, Ubuntu, Debian, CentOS, RHEL, SUSE, CoreOS, Docker, Windows, Python, PIP
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 65becd3a-9d69-4415-8a30-777d13a0e7aa
ms.openlocfilehash: 4ab4f0de38614eff00f55bad96ea886bb007f3c0
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2017
---
# <a name="log-in-with-azure-cli-20"></a>Inicio de sesión con la CLI de Azure 2.0

Hay varias maneras de iniciar sesión y autenticarse con la CLI de Azure. La manera más sencilla de empezar es iniciar sesión de forma interactiva mediante el explorador o en la línea de comandos. El enfoque recomendado consiste en usar entidades de servicio que proporcionan una manera de crear cuentas no interactivas que puede usar para manipular recursos. Mediante la concesión de los permisos adecuados necesarios a una entidad de servicio, puede asegurarse de que sus scripts de automatización son aún más seguros.

Los comandos que se ejecutan con la CLI se ejecutan de manera predeterminada en su suscripción.  Si tiene más de una suscripción, puede que desee [confirmar la suscripción predeterminada](manage-azure-subscriptions-azure-cli.md) y cambiarla según resulte adecuado.

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
La autenticación con una entidad de servicio es la mejor manera de proteger el uso de los recursos de Azure de sus scripts o aplicaciones que manipulan recursos.
Defina los roles que desea que los usuarios tengan mediante el conjunto de comandos `az role`.
Puede obtener más información y ejemplos de roles de entidad de servicio en nuestros [artículos de referencia de roles az](https://docs.microsoft.com/cli/azure/role.md).

1. Si aún no tiene una entidad de servicio, [cree una](create-an-azure-service-principal-azure-cli.md).

1. Inicie sesión con la entidad de servicio.

   ```azurecli-interactive
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   Para obtener el inquilino, inicie sesión de forma interactiva y, a continuación, obtenga el valor de TenantId de su suscripción.

   ```azurecli
   az account show
   ```

   ```json
   {
       "environmentName": "AzureCloud",
       "id": "********-****-****-****-************",
       "isDefault": true,
       "name": "Pay-As-You-Go",
       "state": "Enabled",
       "tenantId": "********-****-****-****-************",
       "user": {
       "name": "********",
       "type": "user"
       }
   }
   ```