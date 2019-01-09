---
title: Uso de entidades de servicio de Azure con la CLI de Azure
description: Aprenda a crear y utilizar una entidad de servicio con la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6cce8fb47dd2b57180487441055333343fff8330
ms.sourcegitcommit: 614811ea63ceb0e71bd99323846dc1b754e15255
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/28/2018
ms.locfileid: "53805880"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a>Creación de una entidad de servicio de Azure con la CLI de Azure

Si desea crear un inicio de sesión independiente con restricciones de acceso, puede hacerlo mediante una entidad de servicio. Las entidades de servicio son identidades independientes que se pueden asociar con una cuenta. Las entidades de servicio son útiles para trabajar con aplicaciones y tareas que se deben automatizar. Este artículo le guía por los pasos de creación de una entidad de servicio.

## <a name="create-the-service-principal"></a>Creación de la entidad de servicio

Use el comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) para crear una entidad de servicio. El nombre de la entidad de servicio no está vinculado a ninguna aplicación o nombre de usuario existentes. Puede crear una entidad de servicio con el tipo de autenticación de su elección.

* `--password` se utiliza para la autenticación basada en contraseña. Si no se incluye un argumento para indicar el tipo de autenticación, se utiliza la contraseña de forma predeterminada y la que haya creado el usuario. Si desea utilizar la autenticación basada en contraseña, le recomendamos que utilice este comando, de modo que la contraseña se cree para usted.  

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName 
  ```
  Si desea elegir la contraseña, en lugar de que se cree para usted (lo que no es recomendable, por razones de seguridad), puede utilizar este comando. Asegúrese de que se crea una contraseña segura siguiendo las [reglas y restricciones de contraseñas de Azure Active Directory](/azure/active-directory/active-directory-passwords-policy). La opción de elegir una contraseña deja la posibilidad de que se elija una contraseña débil o de que se vuelva a utilizar la contraseña. Esta opción está pensada para dejar de utilizarse en una futura versión de la CLI de Azure. 

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password <Choose a strong password>
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

La salida JSON del comando `create-for-rbac` tiene el formato siguiente:

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

La CLI de Azure proporciona los siguientes comandos para administrar las asignaciones de roles.

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)

El rol predeterminado de una entidad de servicio es **colaborador**. Este rol tiene permiso total para leer y escribir en una cuenta de Azure y no es adecuado para aplicaciones. El rol **Lector** es más restrictivo y proporciona acceso de solo lectura.  Para más información sobre el control de acceso basado en rol (RBAC), consulte [RBAC: roles integrados](/azure/active-directory/role-based-access-built-in-roles).

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

Puede probar las credenciales y los permisos de la nueva entidad de servicio, iniciando sesión en la CLI de Azure. Inicie sesión como la nueva entidad de servicio utilizando `appId`, `tenant` y los valores de las credenciales. Utilice el tipo de autenticación con el que se creó la entidad de servicio.

Para iniciar sesión con una contraseña, debe proporcionarla como un parámetro de argumento.

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Para iniciar sesión con un certificado, debe estar disponible localmente en un archivo PEM o DER.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a>Restablecimiento de las credenciales

Si olvida las credenciales de una entidad de servicio, se pueden restablecer mediante el comando [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset). Las mismas restricciones y opciones para crear una entidad de servicio nueva también se aplican aquí.

```azurecli-interactive
az ad sp credential reset --name APP_ID 
```
