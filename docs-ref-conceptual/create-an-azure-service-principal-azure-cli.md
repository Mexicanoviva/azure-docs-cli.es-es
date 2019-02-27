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
ms.openlocfilehash: 7ead12b35cefd7cba9e06f7905c9267c569d98dd
ms.sourcegitcommit: 014d89aa21f90561eb69792ad01947e481ea640a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/23/2019
ms.locfileid: "56741724"
---
# <a name="create-an-azure-service-principal-with-azure-cli"></a><span data-ttu-id="fff0e-103">Creación de una entidad de servicio de Azure con la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="fff0e-103">Create an Azure service principal with Azure CLI</span></span>

<span data-ttu-id="fff0e-104">Las herramientas automatizadas que usan los servicios de Azure deberán tener siempre permisos restringidos.</span><span class="sxs-lookup"><span data-stu-id="fff0e-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="fff0e-105">En lugar de que las aplicaciones inicien sesión como un usuario con privilegios totales, Azure ofrece las entidades de servicio.</span><span class="sxs-lookup"><span data-stu-id="fff0e-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="fff0e-106">Una entidad de servicio de Azure es una identidad creada para su uso con aplicaciones, servicios hospedados y herramientas automatizadas que acceden a los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="fff0e-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="fff0e-107">Este acceso está restringido por los roles asignados a la entidad de servicio, lo que permite controlar a qué recursos pueden tener acceso y en qué nivel.</span><span class="sxs-lookup"><span data-stu-id="fff0e-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="fff0e-108">Por motivos de seguridad, se recomienda usar siempre entidades de servicio con las herramientas automatizadas, en lugar de permitirles iniciar sesión con una identidad de usuario.</span><span class="sxs-lookup"><span data-stu-id="fff0e-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="fff0e-109">En este artículo se muestra los pasos para crear una entidad de servicio, obtener información sobre ella y restablecerla con la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="fff0e-109">This article shows you the steps for creating, getting information about, and resetting a service principal with the Azure CLI.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="fff0e-110">Creación de una entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="fff0e-110">Create a service principal</span></span>

<span data-ttu-id="fff0e-111">Cree una entidad de servicio con el comando [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac).</span><span class="sxs-lookup"><span data-stu-id="fff0e-111">Create a service principal with the [az ad sp create-for-rbac](/cli/azure/ad/sp#az-ad-sp-create-for-rbac) command.</span></span> <span data-ttu-id="fff0e-112">Al crear una entidad de servicio, elija el tipo de autenticación de inicio de sesión que usa.</span><span class="sxs-lookup"><span data-stu-id="fff0e-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span> 

> [!NOTE]
>
> <span data-ttu-id="fff0e-113">Si su cuenta no tiene permisos suficientes para crear una entidad de servicio, `az ad sp create-for-rbac` devolverá un mensaje de error que contiene el texto "Privilegios insuficientes para completar la operación".</span><span class="sxs-lookup"><span data-stu-id="fff0e-113">If your account doesn't have permission to create a service principal, `az ad sp create-for-rbac` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="fff0e-114">Póngase en contacto con el administrador de Azure Active Directory para crear a una entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="fff0e-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="fff0e-115">Hay dos tipos de autenticación disponibles para las entidades de servicio: Autenticación basada en contraseña y autenticación basada en certificado.</span><span class="sxs-lookup"><span data-stu-id="fff0e-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="fff0e-116">Autenticación basada en contraseña</span><span class="sxs-lookup"><span data-stu-id="fff0e-116">Password-based authentication</span></span>

<span data-ttu-id="fff0e-117">La autenticación basada en contraseña no tiene ningún parámetro de autenticación y se usa con una contraseña aleatoria que se crea automáticamente.</span><span class="sxs-lookup"><span data-stu-id="fff0e-117">Without any authentication parameters, password-based authentication is used with a random password created for you.</span></span> <span data-ttu-id="fff0e-118">Si desea usar la autenticación basada en contraseña, se recomienda este método.</span><span class="sxs-lookup"><span data-stu-id="fff0e-118">If you want password-based authentication, this method is recommended.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName
  ```

<span data-ttu-id="fff0e-119">Para usar una contraseña proporcionada por el usuario, utilice el argumento `--password`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-119">For a user-supplied password, use the `--password` argument.</span></span> <span data-ttu-id="fff0e-120">Al crear una contraseña, asegúrese de que seguir las [reglas y restricciones de contraseñas de Azure Active Directory](/azure/active-directory/active-directory-passwords-policy).</span><span class="sxs-lookup"><span data-stu-id="fff0e-120">When creating a password, make sure you follow the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="fff0e-121">No use una contraseña débil ni reutilice las contraseñas.</span><span class="sxs-lookup"><span data-stu-id="fff0e-121">Don't use a weak password or reuse a password.</span></span>

  ```azurecli-interactive
  az ad sp create-for-rbac --name ServicePrincipalName --password <Choose a strong password>
  ```

  > [!IMPORTANT]
  >
  > <span data-ttu-id="fff0e-122">Por motivos de seguridad, el argumento `--password` para la creación entidades de servicio dejará de utilizarse en una versión futura.</span><span class="sxs-lookup"><span data-stu-id="fff0e-122">For security reasons, the `--password` argument for service principal creation will be deprecated in a future release.</span></span> <span data-ttu-id="fff0e-123">Si desea usar la autenticación basada en contraseña, evite `--password` y deje que la CLI genere automáticamente una contraseña segura.</span><span class="sxs-lookup"><span data-stu-id="fff0e-123">If you want to use password-based authentication, avoid `--password` and let the CLI generate a secure password for you.</span></span>

<span data-ttu-id="fff0e-124">La salida para una entidad de servicio con autenticación por contraseña incluye la clave `password`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-124">The output for a service principal with password authentication includes the `password` key.</span></span> <span data-ttu-id="fff0e-125">__No olvide__ copiar este valor porque no se puede recuperar.</span><span class="sxs-lookup"><span data-stu-id="fff0e-125">__Make sure__ you copy this value - it can't be retrieved.</span></span> <span data-ttu-id="fff0e-126">Si olvida la contraseña, [restablezca las credenciales de la entidad de servicio](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="fff0e-126">If you forget the password, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="fff0e-127">Las claves `appId` y `tenant` se muestran en la salida de `az ad sp create-for-rbac` y se usan en la autenticación de la entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="fff0e-127">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="fff0e-128">Anote sus valores, aunque se pueden recuperar en cualquier momento con [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="fff0e-128">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="fff0e-129">Autenticación basada en certificados</span><span class="sxs-lookup"><span data-stu-id="fff0e-129">Certificate-based authentication</span></span>

<span data-ttu-id="fff0e-130">Para la autenticación basada en certificado, use el argumento `--cert`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-130">For certificate-based authentication, use the `--cert` argument.</span></span> <span data-ttu-id="fff0e-131">Este argumento requiere que tenga un certificado.</span><span class="sxs-lookup"><span data-stu-id="fff0e-131">This argument requires that you hold an existing certificate.</span></span> <span data-ttu-id="fff0e-132">Asegúrese de que todas las herramientas que usan esta entidad de servicio tienen acceso a la clave privada del certificado.</span><span class="sxs-lookup"><span data-stu-id="fff0e-132">Make sure any tool that uses this service principal has access to the certificate's private key.</span></span> <span data-ttu-id="fff0e-133">Los certificados deben estar en formato ASCII, como PEM, CER o DER.</span><span class="sxs-lookup"><span data-stu-id="fff0e-133">Certificates should be in an ASCII format such as PEM, CER, or DER.</span></span> <span data-ttu-id="fff0e-134">Pase el certificado como una cadena o use el formato `@path` para cargar el certificado desde un archivo.</span><span class="sxs-lookup"><span data-stu-id="fff0e-134">Pass the certificate as a string, or use the `@path` format to load the certificate from a file.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert "-----BEGIN CERTIFICATE-----
...
-----END CERTIFICATE-----"
```

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert @/path/to/cert.pem
```

<span data-ttu-id="fff0e-135">Se puede agregar el argumento `--keyvault` para usar un certificado de Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="fff0e-135">The `--keyvault` argument can be added to use a certificate in Azure Key Vault.</span></span> <span data-ttu-id="fff0e-136">En este caso, el valor `--cert` es el nombre del certificado.</span><span class="sxs-lookup"><span data-stu-id="fff0e-136">In this case, the `--cert` value is the name of the certificate.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --cert CertName --keyvault VaultName
```

<span data-ttu-id="fff0e-137">Para crear un certificado _autofirmado_ para la autenticación, use el argumento `--create-cert`:</span><span class="sxs-lookup"><span data-stu-id="fff0e-137">To create a _self-signed_ certificate for authentication, use the `--create-cert` argument:</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert
```

<span data-ttu-id="fff0e-138">Se puede agregar el argumento `--keyvault` para almacenar el certificado en Azure Key Vault.</span><span class="sxs-lookup"><span data-stu-id="fff0e-138">The `--keyvault` argument can be added to store the certificate in Azure Key Vault.</span></span> <span data-ttu-id="fff0e-139">Cuando se usa `--keyvault`, el argumento `--cert` también es __necesario__.</span><span class="sxs-lookup"><span data-stu-id="fff0e-139">When using `--keyvault`, the `--cert` argument is __required__.</span></span>

```azurecli-interactive
az ad sp create-for-rbac --name ServicePrincipalName --create-cert --cert CertName --keyvault VaultName
```

<span data-ttu-id="fff0e-140">A menos que almacene el certificado en Key Vault, la salida incluirá la clave `fileWithCertAndPrivateKey`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-140">Unless you store the certificate in Key Vault, the output includes the `fileWithCertAndPrivateKey` key.</span></span> <span data-ttu-id="fff0e-141">Este valor de clave indica donde está almacenado el certificado generado.</span><span class="sxs-lookup"><span data-stu-id="fff0e-141">This key's value tells you where the generated certificate is stored.</span></span>
<span data-ttu-id="fff0e-142">__No olvide__ copiar el certificado en una ubicación segura o no podrá iniciar sesión con esta entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="fff0e-142">__Make sure__ that you copy the certificate to a secure location, or you can't sign in with this service principal.</span></span>

<span data-ttu-id="fff0e-143">En el caso de los certificados almacenados en Key Vault, puede recuperar la clave privada del certificado con [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span><span class="sxs-lookup"><span data-stu-id="fff0e-143">For certificates stored in Key Vault, retrieve the certificate's private key with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show).</span></span> <span data-ttu-id="fff0e-144">En Key Vault, el nombre del secreto del certificado es el mismo que el nombre del certificado.</span><span class="sxs-lookup"><span data-stu-id="fff0e-144">In Key Vault, the name of the certificate's secret is the same as the certificate name.</span></span> <span data-ttu-id="fff0e-145">Si pierde el acceso a la clave privada de un certificado, [restablezca las credenciales de la entidad de servicio](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="fff0e-145">If you lose access to a certificate's private key, [reset the service principal credentials](#reset-credentials).</span></span>

<span data-ttu-id="fff0e-146">Las claves `appId` y `tenant` se muestran en la salida de `az ad sp create-for-rbac` y se usan en la autenticación de la entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="fff0e-146">The `appId` and `tenant` keys appear in the output of `az ad sp create-for-rbac` and are used in service principal authentication.</span></span>
<span data-ttu-id="fff0e-147">Anote sus valores, aunque se pueden recuperar en cualquier momento con [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="fff0e-147">Record their values, but they can be retrieved at any point with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span>

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="fff0e-148">Recuperación de una entidad de servicio existente</span><span class="sxs-lookup"><span data-stu-id="fff0e-148">Get an existing service principal</span></span>

<span data-ttu-id="fff0e-149">Para obtener una lista de las entidades de servicio de un inquilino, use [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span><span class="sxs-lookup"><span data-stu-id="fff0e-149">A list of the service principals in a tenant can be retrieved with [az ad sp list](/cli/azure/ad/sp#az-ad-sp-list).</span></span> <span data-ttu-id="fff0e-150">De forma predeterminada, este comando devuelve las primeras 100 entidades de servicio del inquilino.</span><span class="sxs-lookup"><span data-stu-id="fff0e-150">By default this command returns the first 100 service principals for your tenant.</span></span> <span data-ttu-id="fff0e-151">Para obtener todas las entidades de servicio del inquilino, use el argumento `--all`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-151">To get all of a tenant's service principals, use the `--all` argument.</span></span> <span data-ttu-id="fff0e-152">Generar esta lista puede tardar tiempo, por lo que se recomienda filtrarla con uno de los argumentos siguientes:</span><span class="sxs-lookup"><span data-stu-id="fff0e-152">Getting this list can take a long time, so it's recommended that you filter the list with one of the following arguments:</span></span>

* <span data-ttu-id="fff0e-153">`--display-name` solicita las entidades de servicio que tengan un _prefijo_ que coincida con el nombre proporcionado.</span><span class="sxs-lookup"><span data-stu-id="fff0e-153">`--display-name` requests service principals that have a _prefix_ that match the provided name.</span></span> <span data-ttu-id="fff0e-154">El nombre para mostrar de una entidad de servicio es el valor que se establece con el parámetro `--name` durante la creación.</span><span class="sxs-lookup"><span data-stu-id="fff0e-154">The display name of a service principal is the value set with the `--name` parameter during creation.</span></span> <span data-ttu-id="fff0e-155">Si no ha configurado `--name` durante la creación de la entidad de servicio, el prefijo del nombre es `azure-cli-`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-155">If you didn't set `--name` during service principal creation, the name prefix is `azure-cli-`.</span></span>
* <span data-ttu-id="fff0e-156">`--spn` filtra por los nombres de entidad de servicio que coincidan exactamente.</span><span class="sxs-lookup"><span data-stu-id="fff0e-156">`--spn` filters on exact service principal name matching.</span></span> <span data-ttu-id="fff0e-157">El nombre de la entidad de servicio siempre empieza con `https://`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-157">The service principal name always starts with `https://`.</span></span>
  <span data-ttu-id="fff0e-158">Si el valor utilizado para `--name` no era un URI, este valor `https://`, seguido por el nombre para mostrar.</span><span class="sxs-lookup"><span data-stu-id="fff0e-158">if the value you used for `--name` wasn't a URI, this value is `https://` followed by the display name.</span></span>
* <span data-ttu-id="fff0e-159">`--show-mine` solicita solo las entidades de servicio creadas por el usuario que ha iniciado sesión.</span><span class="sxs-lookup"><span data-stu-id="fff0e-159">`--show-mine` requests only service principals created by the signed-in user.</span></span>
* <span data-ttu-id="fff0e-160">`--filter` toma un filtro OData y filtra _en el lado del servidor_.</span><span class="sxs-lookup"><span data-stu-id="fff0e-160">`--filter` takes an OData filter, and performs _server-side_ filtering.</span></span> <span data-ttu-id="fff0e-161">Se recomienda este método frente al filtrado en el lado del cliente con el argumento `--query` de la CLI.</span><span class="sxs-lookup"><span data-stu-id="fff0e-161">This method is recommended over filtering client-side with the CLI's `--query` argument.</span></span> <span data-ttu-id="fff0e-162">Para más información acerca de los filtros OData, consulte la [sintaxis de expresiones OData para filtros](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span><span class="sxs-lookup"><span data-stu-id="fff0e-162">To learn about OData filters, see [OData expression syntax for filters](/rest/api/searchservice/odata-expression-syntax-for-azure-search).</span></span>

<span data-ttu-id="fff0e-163">La información que se devuelve para los objetos de entidad de servicio es detallada.</span><span class="sxs-lookup"><span data-stu-id="fff0e-163">The information returned for service principal objects is verbose.</span></span> <span data-ttu-id="fff0e-164">Para obtener solo la información necesaria para iniciar sesión, use la cadena de consulta `[].{"id":"appId", "tenant":"appOwnerTenantId"}`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-164">To get only the information necessary for sign-in, use the query string `[].{"id":"appId", "tenant":"appOwnerTenantId"}`.</span></span> <span data-ttu-id="fff0e-165">Por ejemplo, para obtener la información de inicio de sesión de todas las entidades de servicio creadas por el usuario que haya iniciado la sesión actual:</span><span class="sxs-lookup"><span data-stu-id="fff0e-165">For example, to get the sign-in information for all service principals created by the currently logged in user:</span></span>

```azurecli-interactive
az ad sp list --show-mine --query '[].{"id":"appId", "tenant":"appOwnerTenantId"}'
```

> [!IMPORTANT]
>
> <span data-ttu-id="fff0e-166">`az ad sp list` o [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) obtienen el usuario y el inquilino, pero no los secretos de autenticación _ni_ el método de autenticación.</span><span class="sxs-lookup"><span data-stu-id="fff0e-166">`az ad sp list` or [az ad sp show](/cli/azure/ad/sp#az-ad-sp-show) get the user and tenant, but not any authentication secrets _or_ the authentication method.</span></span>
> <span data-ttu-id="fff0e-167">Los secretos de los certificados de Key Vault se pueden recuperar con [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), pero no otros secretos que se almacenen de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="fff0e-167">Secrets for certificates in Key Vault can be retrieved with [az keyvault secret show](/cli/azure/keyvault/secret#az-keyvault-secret-show), but no other secrets are stored by default.</span></span>
> <span data-ttu-id="fff0e-168">Si olvida un método de autenticación o un secreto, [restablezca las credenciales de la entidad de servicio](#reset-credentials).</span><span class="sxs-lookup"><span data-stu-id="fff0e-168">If you forget an authentication method or secret, [reset the service principal credentials](#reset-credentials).</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="fff0e-169">Administración de roles de la entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="fff0e-169">Manage service principal roles</span></span>

<span data-ttu-id="fff0e-170">La CLI de Azure tiene los siguientes comandos para administrar las asignaciones de roles.</span><span class="sxs-lookup"><span data-stu-id="fff0e-170">The Azure CLI has the following commands to manage role assignments:</span></span>

* [<span data-ttu-id="fff0e-171">az role assignment list</span><span class="sxs-lookup"><span data-stu-id="fff0e-171">az role assignment list</span></span>](/cli/azure/role/assignment#az-role-assignment-list)
* [<span data-ttu-id="fff0e-172">az role assignment create</span><span class="sxs-lookup"><span data-stu-id="fff0e-172">az role assignment create</span></span>](/cli/azure/role/assignment#az-role-assignment-create)
* [<span data-ttu-id="fff0e-173">az role assignment delete</span><span class="sxs-lookup"><span data-stu-id="fff0e-173">az role assignment delete</span></span>](/cli/azure/role/assignment#az-role-assignment-delete)

<span data-ttu-id="fff0e-174">El rol predeterminado de una entidad de servicio es **colaborador**.</span><span class="sxs-lookup"><span data-stu-id="fff0e-174">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="fff0e-175">Este rol tiene permiso total para leer y escribir en una cuenta de Azure.</span><span class="sxs-lookup"><span data-stu-id="fff0e-175">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="fff0e-176">El rol **Lector** es más restrictivo y proporciona acceso de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="fff0e-176">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="fff0e-177">Para más información sobre el control de acceso basado en rol (RBAC), consulte [RBAC: roles integrados](/azure/active-directory/role-based-access-built-in-roles).</span><span class="sxs-lookup"><span data-stu-id="fff0e-177">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="fff0e-178">En este ejemplo se agrega el rol **Lector** y se elimina el rol **Colaborador**:</span><span class="sxs-lookup"><span data-stu-id="fff0e-178">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurecli-interactive
az role assignment create --assignee APP_ID --role Reader
az role assignment delete --assignee APP_ID --role Contributor
```

> [!NOTE]
> <span data-ttu-id="fff0e-179">Si su cuenta no tiene permisos para asignar un rol, verá un mensaje de error indicando que su cuenta "no tiene autorización para realizar la acción Microsoft.Authorization/roleAssignments/write". Póngase en contacto con el administrador de Azure Active Directory para administrar los roles.</span><span class="sxs-lookup"><span data-stu-id="fff0e-179">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="fff0e-180">Agregar un rol _no_ restringe los permisos asignados previamente.</span><span class="sxs-lookup"><span data-stu-id="fff0e-180">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="fff0e-181">Al restringir los permisos de una entidad de servicio, el rol __Colaborador__ se debe eliminar.</span><span class="sxs-lookup"><span data-stu-id="fff0e-181">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="fff0e-182">Para comprobar los cambios, puede obtener una lista de los roles asignados:</span><span class="sxs-lookup"><span data-stu-id="fff0e-182">The changes can be verified by listing the assigned roles:</span></span>

```azurecli-interactive
az role assignment list --assignee APP_ID
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="fff0e-183">Inicio de sesión mediante una entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="fff0e-183">Sign in using a service principal</span></span>

<span data-ttu-id="fff0e-184">Para probar las credenciales y los permisos de la nueva entidad de servicio, inicie sesión.</span><span class="sxs-lookup"><span data-stu-id="fff0e-184">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="fff0e-185">Para iniciar sesión con una entidad de servicio, necesita `appId`, `tenant`y las credenciales.</span><span class="sxs-lookup"><span data-stu-id="fff0e-185">To sign in with a service prinicpal, you need the `appId`, `tenant`, and credentials.</span></span>

<span data-ttu-id="fff0e-186">Para iniciar sesión con una entidad de servicio con una contraseña:</span><span class="sxs-lookup"><span data-stu-id="fff0e-186">To sign in with a service principal using a password:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --password PASSWORD --tenant TENANT_ID
```

<span data-ttu-id="fff0e-187">Para iniciar sesión con un certificado, debe estar disponible localmente en un archivo PEM o DER, en formato ASCII.</span><span class="sxs-lookup"><span data-stu-id="fff0e-187">To sign in with a certificate, it must be available locally as a PEM or DER file, in ASCII format:</span></span>

```azurecli-interactive
az login --service-principal --username APP_ID --tenant TENANT_ID --password /path/to/cert
```

<span data-ttu-id="fff0e-188">Para más información acerca de inicio de sesión con una entidad de servicio, consulte [Inicio de sesión con la CLI de Azure](authenticate-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="fff0e-188">To learn more about signing in with a service principal, see [Sign in with the Azure CLI](authenticate-azure-cli.md).</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="fff0e-189">Restablecimiento de las credenciales</span><span class="sxs-lookup"><span data-stu-id="fff0e-189">Reset credentials</span></span>

<span data-ttu-id="fff0e-190">Si olvida las credenciales de una entidad de servicio, utilice [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span><span class="sxs-lookup"><span data-stu-id="fff0e-190">If you forget the credentials for a service principal, use [az ad sp credential reset](/cli/azure/ad/sp/credential#az-ad-sp-credential-reset).</span></span> <span data-ttu-id="fff0e-191">El comando reset toma los mismos argumentos que `az ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="fff0e-191">The reset command takes the same arguments as `az ad sp create-for-rbac`.</span></span>

```azurecli-interactive
az ad sp credential reset --name APP_ID
```
