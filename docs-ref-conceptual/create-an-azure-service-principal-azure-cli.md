---
title: "Creación de una entidad de servicio de Azure con la CLI de Azure 2.0"
description: "Aprenda a crear a una entidad de servicio para cualquier aplicación o servicio con la CLI de Azure 2.0."
keywords: CLI de Azure 2.0, Azure Active Directory, Azure Active directory, AD, RBAC
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: fab89cb8-dac1-4e21-9d34-5eadd5213c05
ms.openlocfilehash: 10a168ae0c33207905d58b7b57ac9ad76d8d9bf4
ms.sourcegitcommit: 73a73c8a17d95b116d33eee3287d938addc5c0ac
ms.translationtype: HT
ms.contentlocale: es-ES
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Creación de una entidad de servicio de Azure con la CLI de Azure 2.0

Si planea administrar una aplicación o servicio con la CLI de Azure 2.0, debe ejecutarla en una entidad de servicio de Azure Active Directory (AAD), en lugar de con sus propias credenciales.
En este tema le ayudará a crear a una entidad de seguridad con la CLI de Azure 2.0.

> [!NOTE]
> Las entidades de servicio también se pueden crear desde Azure Portal.
> Para más información, lea [Uso del portal para crear una aplicación de Azure Active Directory y una entidad de servicio con acceso a los recursos](/azure/azure-resource-manager/resource-group-create-service-principal-portal).

## <a name="what-is-a-service-principal"></a>¿Qué es una "entidad de servicio"?

Una entidad de servicio de Azure es una identidad de seguridad que usan las aplicaciones, los servicios y las herramientas de automatización creadas por el usuario para acceder a recursos específicos de Azure. Se puede considerar una "identidad de usuario" (inicio de sesión y una contraseña o certificado) con un rol específico y permisos estrechamente controlados para acceder a los recursos. A diferencia de una identidad de usuario general, solo necesita poder realizar acciones específicas. Mejora la seguridad si solo se le concede el nivel de permiso mínimo necesario para realizan sus tareas de administración. 

En la actualidad, la CLI de Azure 2.0 solo admite la creación de credenciales de autenticación basados en contraseña. En este tema, se explica cómo crear una entidad de servicio con una contraseña concreta y cómo asignarle roles concretos.

## <a name="verify-your-own-permission-level"></a>Comprobación del nivel de permiso

En primer lugar, debe tener permisos suficientes tanto en su suscripción de Azure como en Azure Active Directory. En concreto, debe poder crear una aplicación en Active Directory y asignar un rol a la entidad de servicio. 

El portal representa la forma más sencilla de comprobar si su cuenta tiene los permisos adecuados. Consulte [Comprobación de los permisos necesarios en el portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).

## <a name="create-a-service-principal-for-your-application"></a>Creación de una entidad de servicio para una aplicación

Debe tener uno de los elementos siguientes para identificar la aplicación para la que desea crear una entidad de servicio:

  * El nombre único o el identificador URI de la aplicación implementada (como "MyDemoWebApp" en los ejemplos), o bien
  * el identificador de la aplicación, el GUID único asociado a la aplicación, el servicio o el objeto implementados

Estos valores identifican la aplicación al crear a una entidad de servicio.

### <a name="get-information-about-your-application"></a>Obtención de información acerca de una aplicación

Con `az ad app list` puede obtener información de la identidad.

```azurecli
az ad app list --display-name MyDemoWebApp
```

```json
{
    "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "appPermissions": null,
    "availableToOtherTenants": false,
    "displayName": "MyDemoWebApp",
    "homepage": "http://MyDemoWebApp.azurewebsites.net",
    "identifierUris": [
      "http://MyDemoWebApp"
    ],
    "objectId": "bd07205b-629f-4a2e-945e-1ee5dadf610b9",
    "objectType": "Application",
    "replyUrls": []
  }
```

La opción `--display-name` filtra la lista de aplicaciones devuelta para mostrar las que tengan `displayName`, a partir de MyDemoWebApp.

### <a name="create-the-service-principal"></a>Creación de la entidad de servicio

Use [az ad sp crear-de-rbac](/cli/azure/ad/sp#create-for-rbac) para crear la entidad de servicio. 

```azurecli
az ad sp create-for-rbac --name {appId} --password "{strong password}" 
``` 

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "name": "http://MyDemoWebApp",
  "password": {strong password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

 > [!WARNING] 
 > No cree una contraseña que no sea segura.  Siga la guía de las [restricciones y reglas de contraseña de Azure AD](/azure/active-directory/active-directory-passwords-policy).

### <a name="get-information-about-the-service-principal"></a>Obtención de información acerca de la entidad de servicio

```azurecli
az ad sp show --id a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "displayName": "MyDemoWebApp",
  "objectId": "0ceae62e-1a1a-446f-aa56-2300d176659bde",
  "objectType": "ServicePrincipal",
  "servicePrincipalNames": [
    "http://MyDemoWebApp",
    "a487e0c1-82af-47d9-9a0b-af184eb87646d"
  ]
}
```

### <a name="sign-in-using-the-service-principal"></a>Inicio de sesión mediante la entidad de servicio

Ya puede iniciar sesión como nuevo servidor principal de servicio en la aplicación mediante *appId* y *password* desde `az ad sp show`.  Especifique el valor *tenant* de los resultados de `az ad sp create-for-rbac`.

```azurecli
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password} --tenant {tenant}
``` 

Si ha iniciado sesión correctamente, verá este resultado:

```json
[
  {
    "cloudName": "AzureCloud",
    "id": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
    "isDefault": true,
    "state": "Enabled",
    "tenantId": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX",
    "user": {
      "name": "https://MyDemoWebApp",
      "type": "servicePrincipal"
    }
  }
]
```

Use los valores `id`, `password`, y `tenant` valores como credenciales para ejecutar la aplicación. 

## <a name="managing-roles"></a>Administración de roles 

> [!NOTE]
> El control de acceso basado en roles (RBAC) de Azure es un modelo para definir y administrar roles tanto para usuario como para las entidades de servicio.
> Los roles conjuntos de permisos asociados a ellos, que son los que determinan los recursos que una entidad puede administrar o leer, a los que puede acceder o en los que puede escribir.
> Para más información acerca RBAC y roles, consulte [Roles integrados para el control de acceso basado en roles de Azure](/azure/active-directory/role-based-access-built-in-roles).

La CLI de Azure 2.0 proporciona los siguientes comandos para administrar las asignaciones de roles:

* [az role assignment list](/cli/azure/role/assignment#list)
* [az role assignment create](/cli/azure/role/assignment#create)
* [az role assignment delete](/cli/azure/role/assignment#delete)

El rol predeterminado de una entidad de servicio es **colaborador**. Dado su gran cantidad de permisos, es posible que sea la mejor opción para las interacciones de una aplicación con los servicios de Azure. El rol **Lector** es más restrictivo y es una buena elección para el acceso de solo lectura. En Azure Portal encontrará más información acerca de los permisos específicos de los roles o podrá crear permisos personalizados.

En este ejemplo, agregue el rol de **lector** al ejemplo anterior y elimine el de **colaborador**:

```azurecli
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

Para comprobar los cambios, enumere los roles asignados actualmente:

```azurecli
az role assignment list --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d
```

```json
{
    "id": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleAssignments/c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "name": "c27f78a7-9d3b-404b-ab59-47818f9af9ac",
    "properties": {
      "principalId": "790525226-46f9-4051-b439-7079e41dfa31",
      "principalName": "http://MyDemoWebApp",
      "roleDefinitionId": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac/providers/Microsoft.Authorization/roleDefinitions/acdd72a7-3385-48ef-bd42-f606fba81ae7",
      "roleDefinitionName": "Reader",
      "scope": "/subscriptions/34345f33-0398-4a99-a42b-f6613d1664ac"
    },
    "type": "Microsoft.Authorization/roleAssignments"
}
```

> [!NOTE] 
> Si su cuenta no tiene permisos suficientes para asignar un rol, verá un mensaje de error.
> El mensaje indica que la cuenta no tiene autorización para realizar la acción "Microsoft.Authorization/roleAssignments/write' en el ámbito '/subscriptions/{guid}".
   
## <a name="change-the-credentials-of-a-security-principal"></a>Cambio de las credenciales de una entidad de seguridad

A nivel de seguridad se recomienda revisar los permisos y actualizar las contraseñas periódicamente. Si lo desea, también puede administrar y modificar las credenciales de seguridad cuando la aplicación cambie.

### <a name="reset-a-service-principal-password"></a>Restablecimiento de la contraseña de una entidad de servicio

Use `az ad sp reset-credentials` para restablecer la contraseña actual de la entidad de servicio.

```azurecli
az ad sp reset-credentials --name 20bce7de-3cd7-49f4-ab64-bb5b443838c3 --password {new-password}
```

```json
{
  "appId": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "name": "a487e0c1-82af-47d9-9a0b-af184eb87646d",
  "password": {new-password},
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

La CLI genera una contraseña segura, si deja fuera la opción `--password`.