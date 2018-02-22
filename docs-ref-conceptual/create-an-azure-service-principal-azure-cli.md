---
title: Uso de entidades de servicio de Azure con la CLI de Azure 2.0
description: Aprenda a crear y utilizar una entidad de servicio con la CLI de Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/12/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: b46c735a14240bddd07659475ada1c33c75a1e67
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="661b8-103">Creación de una entidad de servicio de Azure con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="661b8-103">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="661b8-104">Si desea crear un inicio de sesión independiente con restricciones de acceso, puede hacerlo a través de una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="661b8-104">If you want to create a separate login with access restrictions, you can do so through a service principal.</span></span> <span data-ttu-id="661b8-105">Las entidades de servicio son identidades independientes que se pueden asociar con una cuenta.</span><span class="sxs-lookup"><span data-stu-id="661b8-105">Service principals are separate identities that can be associated with an account.</span></span> <span data-ttu-id="661b8-106">Las entidades de servicio son útiles para trabajar con aplicaciones y tareas que se deben automatizar.</span><span class="sxs-lookup"><span data-stu-id="661b8-106">Service principals are useful for working with applications and tasks that must be automated.</span></span> <span data-ttu-id="661b8-107">Este artículo le guía por los pasos de creación de una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="661b8-107">This article runs you through the steps for creating a service principal.</span></span>

## <a name="create-the-service-principal"></a><span data-ttu-id="661b8-108">Creación de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="661b8-108">Create the service principal</span></span>

<span data-ttu-id="661b8-109">Use el comando [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) para crear una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="661b8-109">Use the [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) command to create a service principal.</span></span> <span data-ttu-id="661b8-110">El nombre de la entidad de servicio no está vinculado a ninguna aplicación o nombre de usuario existentes.</span><span class="sxs-lookup"><span data-stu-id="661b8-110">The Service Principal's name isn't tied to any existing application or user name.</span></span> <span data-ttu-id="661b8-111">Puede crear una entidad de servicio con el tipo de autenticación de su elección.</span><span class="sxs-lookup"><span data-stu-id="661b8-111">You can create a service principal with your choice of authentication type.</span></span>

* <span data-ttu-id="661b8-112">`--password` se utiliza para la autenticación basada en contraseña.</span><span class="sxs-lookup"><span data-stu-id="661b8-112">`--password` is used for password-based authentication.</span></span> <span data-ttu-id="661b8-113">Asegúrese de que se crea una contraseña segura siguiendo las [reglas y restricciones de contraseñas de Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="661b8-113">Make sure that you create a strong password by following the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="661b8-114">Si no especifica una contraseña, se crea una automáticamente.</span><span class="sxs-lookup"><span data-stu-id="661b8-114">If you don't specify a password, one is created for you.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --password PASSWORD
  ```

* <span data-ttu-id="661b8-115">`--cert` se utiliza para la autenticación basada en certificados para un certificado existente, ya sea como una cadena pública PEM o DER o mediante `@{file}` para cargar un archivo.</span><span class="sxs-lookup"><span data-stu-id="661b8-115">`--cert` is used for certificate-based authentication for an existing certificate, either as a PEM or DER public string, or `@{file}` to load a file.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --cert {CertStringOrFile} 
  ```

  <span data-ttu-id="661b8-116">Se puede agregar el argumento `--keyvault` para indicar que el certificado se almacena en Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="661b8-116">The `--keyvault` argument can be added to indicate the cert is stored in Azure Key Vault.</span></span> <span data-ttu-id="661b8-117">En este caso, el valor `--cert` hace referencia al nombre del certificado en el almacén de claves.</span><span class="sxs-lookup"><span data-stu-id="661b8-117">In this case, the `--cert` value refers to the name of the certificate in Key Vault.</span></span>

* <span data-ttu-id="661b8-118">`--create-cert` crea un certificado _autofirmado_ para la autenticación.</span><span class="sxs-lookup"><span data-stu-id="661b8-118">`--create-cert` creates a _self-signed_ certificate for authentication.</span></span> <span data-ttu-id="661b8-119">Se puede agregar el argumento `--keyvault` para almacenar el certificado en Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="661b8-119">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span>

  ```azurecli
  az ad sp create-for-rbac --name ServicePrincipalName --create-cert
  ```

<span data-ttu-id="661b8-120">Si no se incluye un argumento para indicar el tipo de autenticación, se utiliza `--password` de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="661b8-120">If an argument indicating the authentication type isn't included, `--password` is used by default.</span></span>

<span data-ttu-id="661b8-121">La salida del comando `create-for-rbac` tiene el formato siguiente:</span><span class="sxs-lookup"><span data-stu-id="661b8-121">The output of the `create-for-rbac` command is in the following format:</span></span>

```json
{
  "appId": "APP_ID",
  "displayName": "ServicePrincipalName",
  "name": "http://ServicePrincipalName",
  "password": ...,
  "tenant": "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
}
```

<span data-ttu-id="661b8-122">Los valores `appId`, `tenant` y `password` se utilizan para la autenticación.</span><span class="sxs-lookup"><span data-stu-id="661b8-122">The `appId`, `tenant`, and `password` values are used for authentication.</span></span> <span data-ttu-id="661b8-123">El valor `displayName` se utiliza cuando se busca una entidad de servicio existente.</span><span class="sxs-lookup"><span data-stu-id="661b8-123">The `displayName` is used when searching for an existing service principal.</span></span>

> [!NOTE]
> <span data-ttu-id="661b8-124">Si su cuenta no tiene permisos suficientes para crear una entidad de servicio, verá un mensaje de error que contiene el texto "Privilegios suficientes para completar la operación".</span><span class="sxs-lookup"><span data-stu-id="661b8-124">If your account does not have sufficient permissions to create a service principal, you see an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="661b8-125">Póngase en contacto con el administrador de Azure Active Directory para crear a una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="661b8-125">Contact your Azure Active Directory admin to create a service principal.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="661b8-126">Administración de roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="661b8-126">Manage service principal roles</span></span> 

<span data-ttu-id="661b8-127">La CLI de Azure 2.0 proporciona los siguientes comandos para administrar las asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="661b8-127">The Azure CLI 2.0 provides the following commands to manage role assignments.</span></span>

* [<span data-ttu-id="661b8-128">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="661b8-128">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="661b8-129">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="661b8-129">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="661b8-130">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="661b8-130">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="661b8-131">El rol predeterminado de una entidad de servicio es **colaborador**.</span><span class="sxs-lookup"><span data-stu-id="661b8-131">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="661b8-132">Este rol tiene permiso total para leer y escribir en una cuenta de Azure y normalmente no es adecuado para aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="661b8-132">This role has full permissions to read and write to an Azure account, and is usually not appropriate for applications.</span></span> <span data-ttu-id="661b8-133">El rol **Lector** es más restrictivo y proporciona acceso de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="661b8-133">The **Reader** role is more restrictive, providing read-only access.</span></span>  <span data-ttu-id="661b8-134">Para más información sobre el control de acceso basado en roles (RBAC) y los roles, consulte [RBAC: roles integrados](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="661b8-134">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="661b8-135">En este ejemplo se agrega el rol **Lector** y se elimina el rol **Colaborador**.</span><span class="sxs-lookup"><span data-stu-id="661b8-135">This example adds the **Reader** role and deletes the **Contributor** one.</span></span>

```azurecli
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

<span data-ttu-id="661b8-136">La adición de un rol _no_ cambia los permisos asignados previamente.</span><span class="sxs-lookup"><span data-stu-id="661b8-136">Adding a role does _not_ change any previously assigned permissions.</span></span> <span data-ttu-id="661b8-137">Al restringir los permisos de una entidad de servicio, el rol __Colaborador__ siempre se debe eliminar.</span><span class="sxs-lookup"><span data-stu-id="661b8-137">When restricting a service principal's permissions, the __Contributor__ role should always be removed.</span></span>

<span data-ttu-id="661b8-138">Los cambios se pueden comprobar obteniendo una lista de los roles asignados.</span><span class="sxs-lookup"><span data-stu-id="661b8-138">The changes can be verified by listing the assigned roles.</span></span>

```azurecli
az role assignment list --assignee APP_ID
```

> [!NOTE] 
> <span data-ttu-id="661b8-139">Si su cuenta no tiene permisos para asignar un rol, verá un mensaje de error indicando que su cuenta "no tiene autorización para realizar la acción "Microsoft.Authorization/roleAssignments/write" sobre el ámbito "/subscriptions/{guid}". Póngase en contacto con el administrador de Azure Active Directory para administrar los roles.</span><span class="sxs-lookup"><span data-stu-id="661b8-139">If your account doesn't have the permissions to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'." Contact your Azure Active Directory admin to manage roles.</span></span>

## <a name="log-in-using-the-service-principal"></a><span data-ttu-id="661b8-140">Inicio de sesión con la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="661b8-140">Log in using the service principal</span></span>

<span data-ttu-id="661b8-141">Puede probar el inicio de sesión y los permisos de la nueva entidad de servicio, iniciando sesión en la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="661b8-141">You can test the new service principal's login and permissions by logging in under it within the Azure CLI.</span></span> <span data-ttu-id="661b8-142">Inicie sesión como la nueva entidad de servicio utilizando `appId`, `tenant` y los valores de las credenciales.</span><span class="sxs-lookup"><span data-stu-id="661b8-142">Log in as the new service principal using the `appId`, `tenant`, and credentials values.</span></span> <span data-ttu-id="661b8-143">La información de autenticación que debe proporcionar cambia en función de si eligió crear la entidad de servicio con una contraseña o con un certificado.</span><span class="sxs-lookup"><span data-stu-id="661b8-143">The authentication information you provide changes based on whether you chose to create the service principal with a password, or a certificate.</span></span>

<span data-ttu-id="661b8-144">Para iniciar sesión con una contraseña, debe proporcionarla como un parámetro de argumento.</span><span class="sxs-lookup"><span data-stu-id="661b8-144">To log in with a password, provide it as an argument parameter.</span></span>

```azurecli
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="661b8-145">Para iniciar sesión con un certificado, debe estar disponible localmente en un archivo PEM o DER.</span><span class="sxs-lookup"><span data-stu-id="661b8-145">To log in with a certificate, it must be available locally as a PEM or DER file.</span></span>

```azurecli
az login --service-principal --username APP_ID --tenant TENANT_ID --password PATH_TO_CERT
```
## <a name="reset-credentials"></a><span data-ttu-id="661b8-146">Restablecimiento de las credenciales</span><span class="sxs-lookup"><span data-stu-id="661b8-146">Reset credentials</span></span>

<span data-ttu-id="661b8-147">En caso de que olvide las credenciales de una entidad de servicio, se pueden restablecer mediante el comando [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp?view=azure-cli-latest#az_ad_sp_reset_credentials).</span><span class="sxs-lookup"><span data-stu-id="661b8-147">In the event that you forget the credentials for a service principal, they can be reset with the [az ad sp reset-credentials](https://docs.microsoft.com/en-us/cli/azure/ad/sp?view=azure-cli-latest#az_ad_sp_reset_credentials) command.</span></span> <span data-ttu-id="661b8-148">Las mismas restricciones y opciones para crear una entidad de servicio nueva también se aplican aquí.</span><span class="sxs-lookup"><span data-stu-id="661b8-148">The same restrictions and options for creating a new service principal also apply here.</span></span>

```azurecli
az ad sp reset-credentials --name APP_ID --password NEW_PASSWORD
```
