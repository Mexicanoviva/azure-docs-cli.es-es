---
title: Uso de entidades de servicio de Azure con la CLI de Azure 2.0
description: Aprenda a crear y utilizar una entidad de servicio con la CLI de Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.service: role-based-access-control
ms.openlocfilehash: 956a1c10c3e4321651df58f86f6f2c21ede5061f
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967918"
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a>Creación de una entidad de servicio de Azure con la CLI de Azure 2.0

Si desea crear un inicio de sesión independiente con restricciones de acceso, puede hacerlo a través de una entidad de servicio. Las entidades de servicio son identidades independientes que se pueden asociar con una cuenta. Las entidades de servicio son útiles para trabajar con aplicaciones y tareas que se deben automatizar. Este artículo le guía por los pasos de creación de una entidad de servicio.

## <a name="create-the-service-principal"></a>Creación de la entidad de servicio

Use el comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) para crear una entidad de servicio. El nombre de la entidad de servicio no está vinculado a ninguna aplicación o nombre de usuario existentes. Puede crear una entidad de servicio con el tipo de autenticación de su elección.

* `--password` se utiliza para la autenticación basada en contraseña. Asegúrese de que se crea una contraseña segura siguiendo las [reglas y restricciones de contraseñas de Azure Active Directory](/azure/active-directory/active-directory-passwords-policy). Si no especifica una contraseña, se crea una automáticamente.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* `--cert` se utiliza para la autenticación basada en certificados para un certificado existente, ya sea como una cadena pública PEM o DER o mediante `@{file}` para cargar un archivo.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  Se puede agregar el argumento `--keyvault` para indicar que el certificado se almacena en Azure Key Vault. En este caso, el valor `--cert` hace referencia al nombre del certificado en el almacén de claves.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* `--create-cert` crea un certificado _autofirmado_ para la autenticación. Si no se proporciona el argumento `--cert`, se genera un nombre de certificado aleatorio.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  Se puede agregar el argumento `--keyvault` para almacenar el certificado en Azure Key Vault. Cuando se usa `--keyvault`, el argumento `--cert` también es necesario.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

Si no se incluye un argumento para indicar el tipo de autenticación, se utiliza `--password` de forma predeterminada.

La salida del comando `create-for-rbac` tiene el formato siguiente:

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

Los valores `appId`, `tenant` y `password` se utilizan para la autenticación. El valor `displayName` se utiliza cuando se busca una entidad de servicio existente.

> [!NOTE]
> Si su cuenta no tiene permisos suficientes para crear una entidad de servicio, verá un mensaje de error que contiene el texto "Privilegios suficientes para completar la operación". Póngase en contacto con el administrador de Azure Active Directory para crear a una entidad de servicio.

## <a name="manage-service-principal-roles"></a>Administración de roles de la entidad de servicio

La CLI de Azure 2.0 proporciona los siguientes comandos para administrar las asignaciones de roles.

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)

El rol predeterminado de una entidad de servicio es **colaborador**. Este rol tiene permiso total para leer y escribir en una cuenta de Azure y normalmente no es adecuado para aplicaciones. El rol **Lector** es más restrictivo y proporciona acceso de solo lectura.  Para más información sobre el control de acceso basado en roles (RBAC) y los roles, consulte [RBAC: roles integrados](/azure/active-directory/role-based-access-built-in-roles).

En este ejemplo se agrega el rol **Lector** y se elimina el rol **Colaborador**.

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

La adición de un rol _no_ cambia los permisos asignados previamente. Al restringir los permisos de una entidad de servicio, el rol __Colaborador__ siempre se debe eliminar.

Los cambios se pueden comprobar obteniendo una lista de los roles asignados.

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> Si su cuenta no tiene permisos para asignar un rol, verá un mensaje de error indicando que su cuenta "no tiene autorización para realizar la acción "Microsoft.Authorization/roleAssignments/write" sobre el ámbito "/subscriptions/{guid}". Póngase en contacto con el administrador de Azure Active Directory para administrar los roles.

## <a name="sign-in-using-the-service-principal"></a>Inicio de sesión mediante la entidad de servicio

Puede probar las credenciales y los permisos de la nueva entidad de servicio, iniciando sesión en la CLI de Azure. Inicie sesión como la nueva entidad de servicio utilizando `appId`, `tenant` y los valores de las credenciales. La información de autenticación que debe proporcionar cambia en función de si eligió crear la entidad de servicio con una contraseña o con un certificado.

Para iniciar sesión con una contraseña, debe proporcionarla como un parámetro de argumento.

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Para iniciar sesión con un certificado, debe estar disponible localmente en un archivo PEM o DER.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a>Restablecimiento de las credenciales

En caso de que olvide las credenciales de una entidad de servicio, se pueden restablecer mediante el comando [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp#az-ad-sp-reset-credentials). Las mismas restricciones y opciones para crear una entidad de servicio nueva también se aplican aquí.

```azurecli-interactive
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```
