---
title: Uso de entidades de servicio de Azure con la CLI de Azure
description: Aprenda a crear y utilizar una entidad de servicio con la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 40ff3b54cdd1f4908b59479e317092ee62b05bb0
ms.sourcegitcommit: f92d5b3ccd409be126f1e7c06b9f1adc98dad78b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2018
ms.locfileid: "52159378"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="035e8-103">Creación de una entidad de servicio de Azure con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="035e8-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="035e8-104">Si desea crear un inicio de sesión independiente con restricciones de acceso, puede hacerlo mediante una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="035e8-104">If you want to create a separate sign-in with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="035e8-105">Las entidades de servicio son identidades independientes que se pueden asociar con una cuenta.</span><span class="sxs-lookup"><span data-stu-id="035e8-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="035e8-106">Las entidades de servicio son útiles para trabajar con aplicaciones y tareas que se deben automatizar.</span><span class="sxs-lookup"><span data-stu-id="035e8-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="035e8-107">Este artículo le guía por los pasos de creación de una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="035e8-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="035e8-108">Creación de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="035e8-108">Create the service principal</span></span>

<span data-ttu-id="035e8-109">Use el comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) para crear una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="035e8-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="035e8-110">El nombre de la entidad de servicio no está vinculado a ninguna aplicación o nombre de usuario existentes.</span><span class="sxs-lookup"><span data-stu-id="035e8-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="035e8-111">Puede crear una entidad de servicio con el tipo de autenticación de su elección.</span><span class="sxs-lookup"><span data-stu-id="035e8-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="035e8-112">`--password` se utiliza para la autenticación basada en contraseña.</span><span class="sxs-lookup"><span data-stu-id="035e8-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="035e8-113">Asegúrese de que se crea una contraseña segura siguiendo las [reglas y restricciones de contraseñas de Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="035e8-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="035e8-114">Si no especifica una contraseña, se crea una automáticamente.</span><span class="sxs-lookup"><span data-stu-id="035e8-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="035e8-115">`--cert` se utiliza para la autenticación basada en certificados para un certificado existente, ya sea como una cadena pública PEM o DER o mediante `@{file}` para cargar un archivo.</span><span class="sxs-lookup"><span data-stu-id="035e8-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile}
  ```

  <span data-ttu-id="035e8-116">Se puede agregar el argumento `--keyvault` para indicar que el certificado se almacena en Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="035e8-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="035e8-117">En este caso, el valor `--cert` hace referencia al nombre del certificado en el almacén de claves.</span><span class="sxs-lookup"><span data-stu-id="035e8-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
  ```

* <span data-ttu-id="035e8-118">`--create-cert` crea un certificado _autofirmado_ para la autenticación.</span><span class="sxs-lookup"><span data-stu-id="035e8-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="035e8-119">Si no se proporciona el argumento `--cert`, se genera un nombre de certificado aleatorio.</span><span class="sxs-lookup"><span data-stu-id="035e8-119">If the `--cert` argument isn't provided, a random certificate name is generated.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

  <span data-ttu-id="035e8-120">Se puede agregar el argumento `--keyvault` para almacenar el certificado en Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="035e8-120">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="035e8-121">Cuando se usa `--keyvault`, el argumento `--cert` también es necesario.</span><span class="sxs-lookup"><span data-stu-id="035e8-121">When using `--keyvault`, the `--cert` argument is also required.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
  ```

<span data-ttu-id="035e8-122">Si no se incluye un argumento para indicar el tipo de autenticación, se utiliza `--password` de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="035e8-122">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="035e8-123">La salida JSON del comando `create-for-rbac` tiene el formato siguiente:</span><span class="sxs-lookup"><span data-stu-id="035e8-123">The JSON output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="035e8-124">Los valores `appId`, `tenant` y `password` se utilizan para la autenticación.</span><span class="sxs-lookup"><span data-stu-id="035e8-124">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="035e8-125">El valor `displayName` se utiliza cuando se busca una entidad de servicio existente.</span><span class="sxs-lookup"><span data-stu-id="035e8-125">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="035e8-126">Si su cuenta no tiene permisos suficientes para crear una entidad de servicio, verá un mensaje de error que contiene el texto "Privilegios suficientes para completar la operación".</span><span class="sxs-lookup"><span data-stu-id="035e8-126">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="035e8-127">Póngase en contacto con el administrador de Azure Active Directory para crear a una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="035e8-127">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="035e8-128">Administración de roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="035e8-128">Manage service principal roles</span></span>

<span data-ttu-id="035e8-129">La CLI de Azure proporciona los siguientes comandos para administrar las asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="035e8-129">The Azure CLI provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="035e8-130">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="035e8-130">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="035e8-131">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="035e8-131">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="035e8-132">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="035e8-132">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="035e8-133">El rol predeterminado de una entidad de servicio es **colaborador**.</span><span class="sxs-lookup"><span data-stu-id="035e8-133">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="035e8-134">Este rol tiene permiso total para leer y escribir en una cuenta de Azure y no es adecuado para aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="035e8-134">This role has full permissions to read and write to an Azure account, and is not appropriate for applications.</span></span> <span data-ttu-id="035e8-135">El rol **Lector** es más restrictivo y proporciona acceso de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="035e8-135">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="035e8-136">Para más información sobre el control de acceso basado en roles (RBAC) y los roles, consulte [RBAC: roles integrados](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="035e8-136">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="035e8-137">En este ejemplo se agrega el rol **Lector** y se elimina el rol **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="035e8-137">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="035e8-138">La adición de un rol _no_ cambia los permisos asignados previamente.</span><span class="sxs-lookup"><span data-stu-id="035e8-138">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="035e8-139">Al restringir los permisos de una entidad de servicio, el rol __Colaborador__ siempre se debe eliminar.</span><span class="sxs-lookup"><span data-stu-id="035e8-139">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="035e8-140">Los cambios se pueden comprobar obteniendo una lista de los roles asignados.</span><span class="sxs-lookup"><span data-stu-id="035e8-140">The changes can be verified by listing the assigned roles.</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

> [!NOTE]
> <span data-ttu-id="035e8-141">Si su cuenta no tiene permisos para asignar un rol, verá un mensaje de error indicando que su cuenta "no tiene autorización para realizar la acción "Microsoft.Authorization/roleAssignments/write" sobre el ámbito "/subscriptions/{guid}". Póngase en contacto con el administrador de Azure Active Directory para administrar los roles.</span><span class="sxs-lookup"><span data-stu-id="035e8-141">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="035e8-142">Inicio de sesión mediante la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="035e8-142">Sign in using the service principal</span></span>

<span data-ttu-id="035e8-143">Puede probar las credenciales y los permisos de la nueva entidad de servicio, iniciando sesión en la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="035e8-143">You can test the new service principal's credentials and permissions by signing in under it within the Azure CLI.</span></span> <span data-ttu-id="035e8-144">Inicie sesión como la nueva entidad de servicio utilizando `appId`, `tenant` y los valores de las credenciales.</span><span class="sxs-lookup"><span data-stu-id="035e8-144">Sign in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="035e8-145">Utilice el tipo de autenticación con el que se creó la entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="035e8-145">Use the authentication type that the service principal was created with.</span></span>

<span data-ttu-id="035e8-146">Para iniciar sesión con una contraseña, debe proporcionarla como un parámetro de argumento.</span><span class="sxs-lookup"><span data-stu-id="035e8-146">To sign in with a password, provide it as an argument parameter.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="035e8-147">Para iniciar sesión con un certificado, debe estar disponible localmente en un archivo PEM o DER.</span><span class="sxs-lookup"><span data-stu-id="035e8-147">To sign in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```

## <a name="reset-credentials"></a><span data-ttu-id="035e8-148">Restablecimiento de las credenciales</span><span class="sxs-lookup"><span data-stu-id="035e8-148">Reset credentials</span></span>

<span data-ttu-id="035e8-149">Si olvida las credenciales de una entidad de servicio, se pueden restablecer mediante el comando [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="035e8-149">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset) command.</span></span> <span data-ttu-id="035e8-150">Las mismas restricciones y opciones para crear una entidad de servicio nueva también se aplican aquí.</span><span class="sxs-lookup"><span data-stu-id="035e8-150">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID --password NEW_PASSWORD
```
