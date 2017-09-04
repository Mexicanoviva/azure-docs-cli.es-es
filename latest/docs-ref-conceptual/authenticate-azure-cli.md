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
ms.openlocfilehash: fea893ebd55811527e0e92375ffc081a52cdbb57
ms.sourcegitcommit: bcf93ad8ed8802072249cd8187cd4420da89b4c6
ms.translationtype: HT
ms.contentlocale: es-ES
---
# <a name="log-in-with-azure-cli-20"></a><span data-ttu-id="e6072-104">Inicio de sesión con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e6072-104">Log in with Azure CLI 2.0</span></span>

<span data-ttu-id="e6072-105">Hay varias maneras de iniciar sesión y autenticarse con la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="e6072-105">There are several ways to log in and authenticate with the Azure CLI.</span></span> <span data-ttu-id="e6072-106">La manera más sencilla de empezar es iniciar sesión de forma interactiva mediante el explorador o en la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="e6072-106">The simplest way to get started is to log in interactively through your browser, or to log in at the command line.</span></span> <span data-ttu-id="e6072-107">El enfoque recomendado consiste en usar entidades de servicio que proporcionan una manera de crear cuentas no interactivas que puede usar para manipular recursos.</span><span class="sxs-lookup"><span data-stu-id="e6072-107">Our recommended approach is to use service principals, which provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="e6072-108">Mediante la concesión de los permisos adecuados necesarios a una entidad de servicio, puede asegurarse de que sus scripts de automatización son aún más seguros.</span><span class="sxs-lookup"><span data-stu-id="e6072-108">By granting just the appropriate permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

<span data-ttu-id="e6072-109">Los comandos que se ejecutan con la CLI se ejecutan de manera predeterminada en su suscripción.</span><span class="sxs-lookup"><span data-stu-id="e6072-109">Commands that you run with the CLI are run against your default subscription.</span></span>  <span data-ttu-id="e6072-110">Si tiene más de una suscripción, puede que desee [confirmar la suscripción predeterminada](manage-azure-subscriptions-azure-cli.md) y cambiarla según resulte adecuado.</span><span class="sxs-lookup"><span data-stu-id="e6072-110">If you have more than one subscription, you may want to [confirm your default subscription](manage-azure-subscriptions-azure-cli.md) and change it appropriately.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="e6072-111">Inicio de sesión interactivo</span><span class="sxs-lookup"><span data-stu-id="e6072-111">Interactive log-in</span></span>

<span data-ttu-id="e6072-112">Inicie sesión de forma interactiva desde el explorador web.</span><span class="sxs-lookup"><span data-stu-id="e6072-112">Log in interactively from your web browser.</span></span>

[!INCLUDE [interactive_login](includes/interactive-login.md)]

## <a name="command-line"></a><span data-ttu-id="e6072-113">Línea de comandos</span><span class="sxs-lookup"><span data-stu-id="e6072-113">Command line</span></span>

<span data-ttu-id="e6072-114">Proporcione sus credenciales en la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="e6072-114">Provide your credentials on the command line.</span></span>

> [!Note]
> <span data-ttu-id="e6072-115">Este enfoque no es compatible con cuentas de Microsoft o cuentas que tienen habilitada la autenticación en dos fases.</span><span class="sxs-lookup"><span data-stu-id="e6072-115">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurecli
az login -u <username> -p <password>
```

## <a name="logging-in-with-a-service-principal"></a><span data-ttu-id="e6072-116">Inicio de sesión con una entidad de servicio</span><span class="sxs-lookup"><span data-stu-id="e6072-116">Logging in with a service principal</span></span>

<span data-ttu-id="e6072-117">Las entidades de servicio son parecidas a las cuentas de usuario a las que puede aplicar reglas con Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e6072-117">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span>
<span data-ttu-id="e6072-118">La autenticación con una entidad de servicio es la mejor manera de proteger el uso de los recursos de Azure de sus scripts o aplicaciones que manipulan recursos.</span><span class="sxs-lookup"><span data-stu-id="e6072-118">Authenticating with a service principal is the best way to secure the usage of your Azure resources from either your scripts or applications that manipulate resources.</span></span>
<span data-ttu-id="e6072-119">Defina los roles que desea que los usuarios tengan mediante el conjunto de comandos `az role`.</span><span class="sxs-lookup"><span data-stu-id="e6072-119">You define the roles you want your users to have via the `az role` set of commands.</span></span>
<span data-ttu-id="e6072-120">Puede obtener más información y ejemplos de roles de entidad de servicio en nuestros [artículos de referencia de roles az](https://docs.microsoft.com/cli/azure/role.md).</span><span class="sxs-lookup"><span data-stu-id="e6072-120">You can learn more and see examples of service principal roles in our [az role reference articles](https://docs.microsoft.com/cli/azure/role.md).</span></span>

1. <span data-ttu-id="e6072-121">Si aún no tiene una entidad de servicio, [cree una](create-an-azure-service-principal-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="e6072-121">If you don't already have a service principal, [create one](create-an-azure-service-principal-azure-cli.md).</span></span>

1. <span data-ttu-id="e6072-122">Inicie sesión con la entidad de servicio.</span><span class="sxs-lookup"><span data-stu-id="e6072-122">Log in with the service principal.</span></span>

   ```azurecli
   az login --service-principal -u "http://my-app" -p <password> --tenant <tenant>
   ```

   <span data-ttu-id="e6072-123">Para obtener el inquilino, inicie sesión de forma interactiva y, a continuación, obtenga el valor de TenantId de su suscripción.</span><span class="sxs-lookup"><span data-stu-id="e6072-123">To get your tenant, log in interactively and then get the tenantId from your subscription.</span></span>

   ```azurecli
   az login
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