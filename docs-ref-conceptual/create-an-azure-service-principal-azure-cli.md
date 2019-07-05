---
title: Uso de entidades de servicio de Azure con la CLI de Azure
description: Aprenda a crear y utilizar entidades de servicio con la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 6d88400b8d7070cf2f9dba2f3e124edfe2e3163d
ms.sourcegitcommit: e06d34682710e77840b0c51f4718184101bd8a03
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/02/2019
ms.locfileid: "67527324"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a>Creación de una entidad de servicio de Azure con la CLI de Azure

Las herramientas automatizadas que usan los servicios de Azure deberán tener siempre permisos restringidos. En lugar de que las aplicaciones inicien sesión como un usuario con privilegios totales, Azure ofrece las entidades de servicio.

Una entidad de servicio de Azure es una identidad creada para su uso con aplicaciones, servicios hospedados y herramientas automatizadas que acceden a los recursos de Azure. Este acceso está restringido por los roles asignados a la entidad de servicio, lo que permite controlar a qué recursos pueden tener acceso y en qué nivel. Por motivos de seguridad, se recomienda usar siempre entidades de servicio con las herramientas automatizadas, en lugar de permitirles iniciar sesión con una identidad de usuario.

En este artículo se muestra los pasos para crear una entidad de servicio, obtener información sobre ella y restablecerla con la CLI de Azure.

## <a name="create-a-service-principal"></a>Creación de una entidad de servicio

Cree una entidad de servicio con el comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac). Al crear una entidad de servicio, elija el tipo de autenticación de inicio de sesión que usa. 

> [!NOTE]
>
> Si su cuenta no tiene permisos suficientes para crear una entidad de servicio, `az ad sp create-for-rbac` devolverá un mensaje de error que contiene el texto "Privilegios insuficientes para completar la operación". Póngase en contacto con el administrador de Azure Active Directory para crear a una entidad de servicio.

Hay dos tipos de autenticación disponibles para las entidades de servicio: Autenticación basada en contraseña y autenticación basada en certificado.

### <a name="password-based-authentication"></a>Autenticación basada en contraseña

La autenticación basada en contraseña no tiene ningún parámetro de autenticación y se usa con una contraseña aleatoria que se crea automáticamente.

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

> [!IMPORTANT]
> A partir de la CLI de Azure 2.0.68, __ya no se admite__ el parámetro `--password` para crear una entidad de servicio con una contraseña definida por el usuario, para impedir el uso accidental de contraseñas no seguras.

La salida para una entidad de servicio con autenticación por contraseña incluye la clave `password`. __No olvide__ copiar este valor porque no se puede recuperar. Si olvida la contraseña, [restablezca las credenciales de la entidad de servicio](#reset-credentials).

Las claves `appId` y `tenant` se muestran en la salida de `az ad sp create-for-rbac` y se usan en la autenticación de la entidad de servicio.
Anote sus valores, aunque se pueden recuperar en cualquier momento con [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).

### <a name="certificate-based-authentication"></a>Autenticación basada en certificados

Para la autenticación basada en certificado, use el argumento `--cert`. Este argumento requiere que tenga un certificado. Asegúrese de que todas las herramientas que usan esta entidad de servicio tienen acceso a la clave privada del certificado. Los certificados deben estar en formato ASCII, como PEM, CER o DER. Pase el certificado como una cadena o use el formato `@path` para cargar el certificado desde un archivo.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

Se puede agregar el argumento `--keyvault` para usar un certificado de Azure Key Vault. En este caso, el valor `--cert` es el nombre del certificado.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

Para crear un certificado _autofirmado_ para la autenticación, use el argumento `--create-cert`:

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

Se puede agregar el argumento `--keyvault` para almacenar el certificado en Azure Key Vault. Cuando se usa `--keyvault`, el argumento `--cert` también es __necesario__.

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

A menos que almacene el certificado en Key Vault, la salida incluirá la clave `fileWithCertAndPrivateKey`. Este valor de clave indica donde está almacenado el certificado generado.
__No olvide__ copiar el certificado en una ubicación segura o no podrá iniciar sesión con esta entidad de servicio.

En el caso de los certificados almacenados en Key Vault, puede recuperar la clave privada del certificado con [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show). En Key Vault, el nombre del secreto del certificado es el mismo que el nombre del certificado. Si pierde el acceso a la clave privada de un certificado, [restablezca las credenciales de la entidad de servicio](#reset-credentials).

Las claves `appId` y `tenant` se muestran en la salida de `az ad sp create-for-rbac` y se usan en la autenticación de la entidad de servicio.
Anote sus valores, aunque se pueden recuperar en cualquier momento con [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).

## <a name="get-an-existing-service-principal"></a>Recuperación de una entidad de servicio existente

Para obtener una lista de las entidades de servicio de un inquilino, use [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list). De forma predeterminada, este comando devuelve las primeras 100 entidades de servicio del inquilino. Para obtener todas las entidades de servicio del inquilino, use el argumento `--all`. Generar esta lista puede tardar tiempo, por lo que se recomienda filtrarla con uno de los argumentos siguientes:

* `--display-name` solicita las entidades de servicio que tengan un _prefijo_ que coincida con el nombre proporcionado. El nombre para mostrar de una entidad de servicio es el valor que se establece con el parámetro `--name` durante la creación. Si no ha configurado `--name` durante la creación de la entidad de servicio, el prefijo del nombre es `azure-cli-`.
* `--spn` filtra por los nombres de entidad de servicio que coincidan exactamente. El nombre de la entidad de servicio siempre empieza con `https://`.
  Si el valor utilizado para `--name` no era un URI, este valor `https://`, seguido por el nombre para mostrar.
* `--show-mine` solicita solo las entidades de servicio creadas por el usuario que ha iniciado sesión.
* `--filter` toma un filtro OData y filtra _en el lado del servidor_. Se recomienda este método frente al filtrado en el lado del cliente con el argumento `--query` de la CLI. Para más información acerca de los filtros OData, consulte la [sintaxis de expresiones OData para filtros](/rest/api/searchservice/odata-expression-syntax-for-azure-search).

La información que se devuelve para los objetos de entidad de servicio es detallada. Para obtener solo la información necesaria para iniciar sesión, use la cadena de consulta `[].{"id":"appId", "tenant":"appOwnerTenantId"}`. Por ejemplo, para obtener la información de inicio de sesión de todas las entidades de servicio creadas por el usuario que haya iniciado la sesión actual:

```azurecli-interactive
az ad sp list --show-mine --query '[].{"id":"appId", "tenant":"appOwnerTenantId"}'
```

> [!IMPORTANT]
>
> `az ad sp list` o [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) obtienen el usuario y el inquilino, pero no los secretos de autenticación _ni_ el método de autenticación.
> Los secretos de los certificados de Key Vault se pueden recuperar con [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), pero no otros secretos que se almacenen de forma predeterminada.
> Si olvida un método de autenticación o un secreto, [restablezca las credenciales de la entidad de servicio](#reset-credentials).

## <a name="manage-service-principal-roles"></a>Administración de roles de la entidad de servicio

La CLI de Azure tiene los siguientes comandos para administrar las asignaciones de roles.

* [az role assignment list](/cli/azure/role/assignment#az-role-assignment-list)
* [az role assignment create](/cli/azure/role/assignment#az-role-assignment-create)
* [az role assignment delete](/cli/azure/role/assignment#az-role-assignment-delete)

El rol predeterminado de una entidad de servicio es **colaborador**. Este rol tiene permiso total para leer y escribir en una cuenta de Azure. El rol **Lector** es más restrictivo y proporciona acceso de solo lectura.  Para más información sobre el control de acceso basado en rol (RBAC), consulte [RBAC: roles integrados](/azure/active-directory/role-based-access-built-in-roles).

En este ejemplo se agrega el rol **Lector** y se elimina el rol **Colaborador**:

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> Si su cuenta no tiene permisos para asignar un rol, verá un mensaje de error indicando que su cuenta "no tiene autorización para realizar la acción Microsoft.Authorization/roleAssignments/write". Póngase en contacto con el administrador de Azure Active Directory para administrar los roles.

Agregar un rol _no_ restringe los permisos asignados previamente. Al restringir los permisos de una entidad de servicio, el rol __Colaborador__ se debe eliminar.

Para comprobar los cambios, puede obtener una lista de los roles asignados:

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a>Inicio de sesión mediante una entidad de servicio

Para probar las credenciales y los permisos de la nueva entidad de servicio, inicie sesión. Para iniciar sesión con una entidad de servicio, necesita `appId`, `tenant`y las credenciales.

Para iniciar sesión con una entidad de servicio con una contraseña:

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

Para iniciar sesión con un certificado, debe estar disponible localmente en un archivo PEM o DER, en formato ASCII.

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

Para más información acerca de inicio de sesión con una entidad de servicio, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).

## <a name="reset-credentials"></a>Restablecimiento de las credenciales

Si olvida las credenciales de una entidad de servicio, utilice [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset). El comando reset toma los mismos argumentos que `az ad sp create-for-rbac`.

```azurecli-interactive
az ad sp credential reset --name APP_ID
```
