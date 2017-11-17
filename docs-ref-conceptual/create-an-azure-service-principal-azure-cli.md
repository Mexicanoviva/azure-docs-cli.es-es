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
ms.openlocfilehash: 0ee794d5a732c6e8d2d52fca5810a874827930ae
ms.sourcegitcommit: 5a04b7fbb73a5f10c4021963ecd6ebe234cc3b61
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/15/2017
---
# <a name="create-an-azure-service-principal-with-azure-cli-20"></a><span data-ttu-id="1d6df-104">Creación de una entidad de servicio de Azure con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="1d6df-104">Create an Azure service principal with Azure CLI 2.0</span></span>

<span data-ttu-id="1d6df-105">Si planea administrar una aplicación o servicio con la CLI de Azure 2.0, debe ejecutarla en una entidad de servicio de Azure Active Directory (AAD), en lugar de con sus propias credenciales.</span><span class="sxs-lookup"><span data-stu-id="1d6df-105">If you plan to manage your app or service with Azure CLI 2.0, you should run it under an Azure Active Directory (AAD) service principal rather than your own credentials.</span></span>
<span data-ttu-id="1d6df-106">En este tema le ayudará a crear a una entidad de seguridad con la CLI de Azure 2.0.</span><span class="sxs-lookup"><span data-stu-id="1d6df-106">This topic steps you through creating a security principal with Azure CLI 2.0.</span></span>

> [!NOTE]
> <span data-ttu-id="1d6df-107">Las entidades de servicio también se pueden crear desde Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1d6df-107">You can also create a service principal through the Azure portal.</span></span>
> <span data-ttu-id="1d6df-108">Para más información, lea [Uso del portal para crear una aplicación de Azure Active Directory y una entidad de servicio con acceso a los recursos](/azure/azure-resource-manager/resource-group-create-service-principal-portal).</span><span class="sxs-lookup"><span data-stu-id="1d6df-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="1d6df-109">¿Qué es una "entidad de servicio"?</span><span class="sxs-lookup"><span data-stu-id="1d6df-109">What is a 'service principal'?</span></span>

<span data-ttu-id="1d6df-110">Una entidad de servicio de Azure es una identidad de seguridad que usan las aplicaciones, los servicios y las herramientas de automatización creadas por el usuario para acceder a recursos específicos de Azure.</span><span class="sxs-lookup"><span data-stu-id="1d6df-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="1d6df-111">Se puede considerar una "identidad de usuario" (inicio de sesión y una contraseña o certificado) con un rol específico y permisos estrechamente controlados para acceder a los recursos.</span><span class="sxs-lookup"><span data-stu-id="1d6df-111">Think of it as a 'user identity' (login and password or certificate) with a specific role, and tightly controlled permissions to access your resources.</span></span> <span data-ttu-id="1d6df-112">A diferencia de una identidad de usuario general, solo necesita poder realizar acciones específicas.</span><span class="sxs-lookup"><span data-stu-id="1d6df-112">It only needs to be able to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="1d6df-113">Mejora la seguridad si solo se le concede el nivel de permiso mínimo necesario para realizan sus tareas de administración.</span><span class="sxs-lookup"><span data-stu-id="1d6df-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span> 

<span data-ttu-id="1d6df-114">En la actualidad, la CLI de Azure 2.0 solo admite la creación de credenciales de autenticación basados en contraseña.</span><span class="sxs-lookup"><span data-stu-id="1d6df-114">Right now, Azure CLI 2.0 only supports the creation of password-based authentication credentials.</span></span> <span data-ttu-id="1d6df-115">En este tema, se explica cómo crear una entidad de servicio con una contraseña concreta y cómo asignarle roles concretos.</span><span class="sxs-lookup"><span data-stu-id="1d6df-115">In this topic, we cover creating a service principal with a specific password, and optionally assigning specific roles to it.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="1d6df-116">Comprobación del nivel de permiso</span><span class="sxs-lookup"><span data-stu-id="1d6df-116">Verify your own permission level</span></span>

<span data-ttu-id="1d6df-117">En primer lugar, debe tener permisos suficientes tanto en su suscripción de Azure como en Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1d6df-117">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="1d6df-118">En concreto, debe poder crear una aplicación en Active Directory y asignar un rol a la entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="1d6df-118">Specifically, you must be able to create an app in the Active Directory, and assign a role to the service principal.</span></span> 

<span data-ttu-id="1d6df-119">El portal representa la forma más sencilla de comprobar si su cuenta tiene los permisos adecuados.</span><span class="sxs-lookup"><span data-stu-id="1d6df-119">The easiest way to check whether your account has adequate permissions is through the portal.</span></span> <span data-ttu-id="1d6df-120">Consulte [Comprobación de los permisos necesarios en el portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).</span><span class="sxs-lookup"><span data-stu-id="1d6df-120">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal.md#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="1d6df-121">Creación de una entidad de servicio para una aplicación</span><span class="sxs-lookup"><span data-stu-id="1d6df-121">Create a service principal for your application</span></span>

<span data-ttu-id="1d6df-122">Debe tener uno de los elementos siguientes para identificar la aplicación para la que desea crear una entidad de servicio:</span><span class="sxs-lookup"><span data-stu-id="1d6df-122">You must have one of the following to identify the app you want to create a service principal for:</span></span>

  * <span data-ttu-id="1d6df-123">El nombre único o el identificador URI de la aplicación implementada (como "MyDemoWebApp" en los ejemplos), o bien</span><span class="sxs-lookup"><span data-stu-id="1d6df-123">The unique name or URI of your deployed app (such as "MyDemoWebApp" in the examples), or</span></span>
  * <span data-ttu-id="1d6df-124">el identificador de la aplicación, el GUID único asociado a la aplicación, el servicio o el objeto implementados</span><span class="sxs-lookup"><span data-stu-id="1d6df-124">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

<span data-ttu-id="1d6df-125">Estos valores identifican la aplicación al crear a una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="1d6df-125">These values identify your application when creating a service principal.</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="1d6df-126">Obtención de información acerca de una aplicación</span><span class="sxs-lookup"><span data-stu-id="1d6df-126">Get information about your application</span></span>

<span data-ttu-id="1d6df-127">Con `az ad app list` puede obtener información de la identidad.</span><span class="sxs-lookup"><span data-stu-id="1d6df-127">Get identity information about your application with the `az ad app list`.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

```azurecli-interactive
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

<span data-ttu-id="1d6df-128">La opción `--display-name` filtra la lista de aplicaciones devuelta para mostrar las que tengan `displayName`, a partir de MyDemoWebApp.</span><span class="sxs-lookup"><span data-stu-id="1d6df-128">The `--display-name` option filters the returned list of apps to show those with `displayName` starting with MyDemoWebApp.</span></span>

### <a name="create-the-service-principal"></a><span data-ttu-id="1d6df-129">Creación de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="1d6df-129">Create the service principal</span></span>

<span data-ttu-id="1d6df-130">Use [az ad sp crear-de-rbac](/cli/azure/ad/sp#create-for-rbac) para crear la entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="1d6df-130">Use [az ad sp create-for-rbac](/cli/azure/ad/sp#create-for-rbac) to create the service principal.</span></span> 

```azurecli-interactive
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
 > <span data-ttu-id="1d6df-131">No cree una contraseña que no sea segura.</span><span class="sxs-lookup"><span data-stu-id="1d6df-131">Don't create an insecure password.</span></span>  <span data-ttu-id="1d6df-132">Siga la guía de las [restricciones y reglas de contraseña de Azure AD](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="1d6df-132">Follow the [Azure AD password rules and restrictions](/azure/active-directory/active-directory-passwords-policy) guidance.</span></span>

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="1d6df-133">Obtención de información acerca de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="1d6df-133">Get information about the service principal</span></span>

```azurecli-interactive
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

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="1d6df-134">Inicio de sesión mediante la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="1d6df-134">Sign in using the service principal</span></span>

<span data-ttu-id="1d6df-135">Ya puede iniciar sesión como nuevo servidor principal de servicio en la aplicación mediante *appId* y *password* desde `az ad sp show`.</span><span class="sxs-lookup"><span data-stu-id="1d6df-135">You can now log in as the new service principal for your app using the *appId* and *password* from `az ad sp show`.</span></span>  <span data-ttu-id="1d6df-136">Especifique el valor *tenant* de los resultados de `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="1d6df-136">Supply the *tenant* value from the results of `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az login --service-principal -u a487e0c1-82af-47d9-9a0b-af184eb87646d --password {password} --tenant {tenant}
``` 

<span data-ttu-id="1d6df-137">Si ha iniciado sesión correctamente, verá este resultado:</span><span class="sxs-lookup"><span data-stu-id="1d6df-137">You will see this output after a successful sign-on:</span></span>

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

<span data-ttu-id="1d6df-138">Use los valores `id`, `password`, y `tenant` valores como credenciales para ejecutar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="1d6df-138">Use the `id`, `password`, and `tenant` values as the credentials for running your app.</span></span> 

## <a name="managing-roles"></a><span data-ttu-id="1d6df-139">Administración de roles</span><span class="sxs-lookup"><span data-stu-id="1d6df-139">Managing roles</span></span> 

> [!NOTE]
> <span data-ttu-id="1d6df-140">El control de acceso basado en roles (RBAC) de Azure es un modelo para definir y administrar roles tanto para usuario como para las entidades de servicio.</span><span class="sxs-lookup"><span data-stu-id="1d6df-140">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span>
> <span data-ttu-id="1d6df-141">Los roles conjuntos de permisos asociados a ellos, que son los que determinan los recursos que una entidad puede administrar o leer, a los que puede acceder o en los que puede escribir.</span><span class="sxs-lookup"><span data-stu-id="1d6df-141">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span>
> <span data-ttu-id="1d6df-142">Para más información acerca RBAC y roles, consulte [Roles integrados para el control de acceso basado en roles de Azure](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="1d6df-142">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="1d6df-143">La CLI de Azure 2.0 proporciona los siguientes comandos para administrar las asignaciones de roles:</span><span class="sxs-lookup"><span data-stu-id="1d6df-143">The Azure CLI 2.0 provides the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="1d6df-144">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="1d6df-144">az role assignment list</span></span>](/cli/azure/role/assignment#list)
* [<span data-ttu-id="1d6df-145">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="1d6df-145">az role assignment create</span></span>](/cli/azure/role/assignment#create)
* [<span data-ttu-id="1d6df-146">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="1d6df-146">az role assignment delete</span></span>](/cli/azure/role/assignment#delete)

<span data-ttu-id="1d6df-147">El rol predeterminado de una entidad de servicio es **colaborador**.</span><span class="sxs-lookup"><span data-stu-id="1d6df-147">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="1d6df-148">Dado su gran cantidad de permisos, es posible que sea la mejor opción para las interacciones de una aplicación con los servicios de Azure.</span><span class="sxs-lookup"><span data-stu-id="1d6df-148">It may not be the best choice for an app's interactions with Azure services, given its broad permissions.</span></span> <span data-ttu-id="1d6df-149">El rol **Lector** es más restrictivo y es una buena elección para el acceso de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="1d6df-149">The **Reader** role is more restrictive and is a good choice for read-only access.</span></span> <span data-ttu-id="1d6df-150">En Azure Portal encontrará más información acerca de los permisos específicos de los roles o podrá crear permisos personalizados.</span><span class="sxs-lookup"><span data-stu-id="1d6df-150">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="1d6df-151">En este ejemplo, agregue el rol de **lector** al ejemplo anterior y elimine el de **colaborador**:</span><span class="sxs-lookup"><span data-stu-id="1d6df-151">In this example, add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Reader
az role assignment delete --assignee a487e0c1-82af-47d9-9a0b-af184eb87646d --role Contributor
```

<span data-ttu-id="1d6df-152">Para comprobar los cambios, enumere los roles asignados actualmente:</span><span class="sxs-lookup"><span data-stu-id="1d6df-152">Verify the changes by listing the currently assigned roles:</span></span>

```azurecli-interactive
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
> <span data-ttu-id="1d6df-153">Si su cuenta no tiene permisos suficientes para asignar un rol, verá un mensaje de error.</span><span class="sxs-lookup"><span data-stu-id="1d6df-153">If your account does not have sufficient permissions to assign a role, you see an error message.</span></span>
> <span data-ttu-id="1d6df-154">El mensaje indica que la cuenta no tiene autorización para realizar la acción "Microsoft.Authorization/roleAssignments/write' en el ámbito '/subscriptions/{guid}".</span><span class="sxs-lookup"><span data-stu-id="1d6df-154">The message states your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write' over scope '/subscriptions/{guid}'."</span></span>
   
## <a name="change-the-credentials-of-a-security-principal"></a><span data-ttu-id="1d6df-155">Cambio de las credenciales de una entidad de seguridad</span><span class="sxs-lookup"><span data-stu-id="1d6df-155">Change the credentials of a security principal</span></span>

<span data-ttu-id="1d6df-156">A nivel de seguridad se recomienda revisar los permisos y actualizar las contraseñas periódicamente.</span><span class="sxs-lookup"><span data-stu-id="1d6df-156">It's a good security practice to review permissions and update passwords regularly.</span></span> <span data-ttu-id="1d6df-157">Si lo desea, también puede administrar y modificar las credenciales de seguridad cuando la aplicación cambie.</span><span class="sxs-lookup"><span data-stu-id="1d6df-157">You may also want to manage and modify the security credentials as your app changes.</span></span>

### <a name="reset-a-service-principal-password"></a><span data-ttu-id="1d6df-158">Restablecimiento de la contraseña de una entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="1d6df-158">Reset a service principal password</span></span>

<span data-ttu-id="1d6df-159">Use `az ad sp reset-credentials` para restablecer la contraseña actual de la entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="1d6df-159">Use `az ad sp reset-credentials` to reset the current password for the service principal.</span></span>

```azurecli-interactive
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

<span data-ttu-id="1d6df-160">La CLI genera una contraseña segura, si deja fuera la opción `--password`.</span><span class="sxs-lookup"><span data-stu-id="1d6df-160">The CLI generates a secure password if you leave out the `--password` option.</span></span>