---
title: "Introducción a la CLI de Azure 2.0"
description: "Introducción a la CLI de Azure 2.0 en Linux, Mac o Windows."
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
ms.assetid: 85c418a8-6177-4833-bb8d-ff4ce2233c1a
ms.openlocfilehash: 689b8f4d77af5a6f398c0dd85e922baa398f767a
ms.sourcegitcommit: 2e4d0bdd94c626e061434883032367b5619de4fe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2017
---
# <a name="get-started-with-azure-cli-20"></a><span data-ttu-id="654d6-104">Introducción a la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="654d6-104">Get started with Azure CLI 2.0</span></span>

<span data-ttu-id="654d6-105">La CLI de Azure 2.0 es la nueva forma de usar la línea de comandos de Azure para administrar recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="654d6-105">The Azure CLI 2.0 is Azure's new command line experience for managing Azure resources.</span></span>
<span data-ttu-id="654d6-106">Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="654d6-106">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can [install](install-azure-cli.md) it on macOS, Linux, and Windows and run it from the command line.</span></span>

<span data-ttu-id="654d6-107">La CLI de Azure 2.0 está optimizada para administrar recursos de Azure desde la línea de comandos y para generar scripts de automatización que funcionan con Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="654d6-107">Azure CLI 2.0 is optimized for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span>
<span data-ttu-id="654d6-108">Este artículo le ayuda a empezar a usarlo y explica los conceptos básicos que hay detrás.</span><span class="sxs-lookup"><span data-stu-id="654d6-108">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

<span data-ttu-id="654d6-109">Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="654d6-109">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

## <a name="connect"></a><span data-ttu-id="654d6-110">Conectar</span><span class="sxs-lookup"><span data-stu-id="654d6-110">Connect</span></span>

<span data-ttu-id="654d6-111">La manera más sencilla de empezar es [iniciar Cloud Shell](/azure/cloud-shell/quickstart).</span><span class="sxs-lookup"><span data-stu-id="654d6-111">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="654d6-112">Inicie Cloud Shell en la navegación superior de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="654d6-112">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Icono de Shell](media/get-started-with-azure-cli/shell-icon.png)

2. <span data-ttu-id="654d6-114">Elija la suscripción que desea utilizar y cree una cuenta de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="654d6-114">Choose the subscription you want to use and create a storage account.</span></span>

   ![Crear una cuenta de almacenamiento](media/get-started-with-azure-cli/storage-prompt.png)

<span data-ttu-id="654d6-116">También puede [instalar](install-azure-cli.md) la CLI y ejecutarla localmente desde la línea de comandos.</span><span class="sxs-lookup"><span data-stu-id="654d6-116">You can also [install](install-azure-cli.md) the CLI and run it locally from the command line.</span></span> <span data-ttu-id="654d6-117">Después de instalar la CLI, ejecute `az login` para iniciar sesión con su suscripción predeterminada.</span><span class="sxs-lookup"><span data-stu-id="654d6-117">Once you have installed the CLI, run `az login` to log in with your default subscription.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="654d6-118">Creación de un grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="654d6-118">Create a Resource Group</span></span>

<span data-ttu-id="654d6-119">Ahora que todo está configurado, vamos a usar la CLI de Azure para crear recursos en Azure.</span><span class="sxs-lookup"><span data-stu-id="654d6-119">Now that we've got everything set up, let's use the Azure CLI to create resources within Azure.</span></span>

<span data-ttu-id="654d6-120">En primer lugar, cree un grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="654d6-120">First, create a Resource Group.</span></span>  <span data-ttu-id="654d6-121">En Azure, los grupos de recursos proporcionan una manera de administrar varios recursos que se desean agrupar de manera lógica.</span><span class="sxs-lookup"><span data-stu-id="654d6-121">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group.</span></span>  <span data-ttu-id="654d6-122">Por ejemplo, puede crear un grupo de recursos para una aplicación o un proyecto, y agregar una máquina virtual, una base de datos y un servicio de CDN en él.</span><span class="sxs-lookup"><span data-stu-id="654d6-122">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="654d6-123">Vamos a crear un grupo de recursos denominado "MyResourceGroup" en la región *oesteeeuu2* de Azure.</span><span class="sxs-lookup"><span data-stu-id="654d6-123">Let's create a resource group named "MyResourceGroup" in the *westus2* region of Azure.</span></span>  <span data-ttu-id="654d6-124">Para ello, escriba el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="654d6-124">To do so type the following command:</span></span>

```azurecli-interactive
az group create -n MyResourceGroup -l westus2
```

<span data-ttu-id="654d6-125">Una vez que se haya creado el grupo de recursos, el comando `az group create` genera varias propiedades del recursos recién creado:</span><span class="sxs-lookup"><span data-stu-id="654d6-125">Once the resource group has been created, the `az group create` command outputs several properties of the newly created resource:</span></span>

```Output
{
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup",
  "location": "westus2",
  "managedBy": null,
  "name": "MyResourceGroup",
  "properties": {
    "provisioningState": "Succeeded"
  },
  "tags": null
}
```

## <a name="create-a-linux-virtual-machine"></a><span data-ttu-id="654d6-126">Creación de una máquina virtual Linux</span><span class="sxs-lookup"><span data-stu-id="654d6-126">Create a Linux Virtual Machine</span></span>

<span data-ttu-id="654d6-127">Ahora que tenemos nuestro grupo de recursos, vamos a crear una máquina virtual Linux en él.</span><span class="sxs-lookup"><span data-stu-id="654d6-127">Now that we have our resource group, let's create a Linux VM within it.</span></span>

<span data-ttu-id="654d6-128">Puede crear una máquina virtual Linux con la popular imagen de UbuntuLTS, con dos discos de almacenamiento conectados de 10 GB y 20 GB, con el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="654d6-128">You can create a Linux VM using the popular UbuntuLTS image, with two attached storage disks of 10 GB and 20 GB, with the following command:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

<span data-ttu-id="654d6-129">Al ejecutar el comando anterior, la CLI de Azure 2.0 busca un par de claves SSH almacenadas en el directorio ~/.ssh.</span><span class="sxs-lookup"><span data-stu-id="654d6-129">When you run the preceding command, the Azure CLI 2.0 looks for an SSH key pair stored under your ~/.ssh directory.</span></span>  <span data-ttu-id="654d6-130">Si aún no tiene un par de claves SSH almacenadas ahí, puede pedir a la CLI de Azure que lo cree automáticamente pasando el parámetro --parámetro --generate-ssh-keys:</span><span class="sxs-lookup"><span data-stu-id="654d6-130">If you don't already have an SSH key pair stored there, you can ask the Azure CLI to automatically create one for you by passing the --generate-ssh-keys parameter:</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20 --generate-ssh-keys
```

<span data-ttu-id="654d6-131">El comando `az vm create` devuelve la salida una vez que la máquina virtual se haya creado completamente y que esté lista para usarla y para que se acceda a ella.</span><span class="sxs-lookup"><span data-stu-id="654d6-131">The `az vm create` command returns output once the VM has been fully created and is ready to be accessed and used.</span></span> <span data-ttu-id="654d6-132">La salida incluye varias propiedades de la máquina virtual recién creada, entre las que se incluye la dirección IP pública:</span><span class="sxs-lookup"><span data-stu-id="654d6-132">The output includes several properties of the newly created VM including its public IP address:</span></span>

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xxx.xx",
  "resourceGroup": "MyResourceGroup"
}
```

<span data-ttu-id="654d6-133">Una vez creada la máquina virtual, puede iniciar sesión en la nueva máquina virtual Linux mediante **SSH** con la dirección IP pública de la máquina virtual que ha creado:</span><span class="sxs-lookup"><span data-stu-id="654d6-133">Now that the VM has been created, you can log on to your new Linux VM using **SSH** with the public IP address of the VM you created:</span></span>

```azurecli-interactive
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:~$
```

## <a name="create-a-windows-server-virtual-machine"></a><span data-ttu-id="654d6-134">Creación de una máquina virtual con Windows Server</span><span class="sxs-lookup"><span data-stu-id="654d6-134">Create a Windows Server Virtual Machine</span></span>

<span data-ttu-id="654d6-135">Ahora se va a crear una máquina virtual basada en Windows Server 2016 Datacenter mediante el comando `az vm create` y a agregarla al mismo grupo de recursos "MyResourceGroup" que se ha usado para la máquina virtual Linux.</span><span class="sxs-lookup"><span data-stu-id="654d6-135">Let's now create a Windows Server 2016 Datacenter-based VM using the `az vm create` command and add it to the same "MyResourceGroup" resource group that we used for our Linux VM.</span></span>  <span data-ttu-id="654d6-136">Al igual que en el ejemplo de la máquina virtual Linux, también se van a conectar dos discos de almacenamiento mediante el parámetro `--data-disk-sizes-gb`.</span><span class="sxs-lookup"><span data-stu-id="654d6-136">Like the Linux VM example, we'll also attach two storage disks using the `--data-disk-sizes-gb` parameter.</span></span>

<span data-ttu-id="654d6-137">Azure requiere que se evite usar nombres de usuario o contraseñas que se adivinen con facilidad.</span><span class="sxs-lookup"><span data-stu-id="654d6-137">Azure requires that you avoid using easily guessed usernames/passwords.</span></span> <span data-ttu-id="654d6-138">Hay reglas específicas relativas a los caracteres que se pueden usar, así como a la longitud mínima del nombre de usuario y de la contraseña.</span><span class="sxs-lookup"><span data-stu-id="654d6-138">There are specific rules for what characters can be used as well as the minimum length of both username and password.</span></span>

> [!NOTE]
> <span data-ttu-id="654d6-139">Al ejecutar este comando, se le pedirá que escriba el nombre de usuario y la contraseña.</span><span class="sxs-lookup"><span data-stu-id="654d6-139">You will be prompted to enter your username and password when running this command.</span></span>

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

<span data-ttu-id="654d6-140">El comando `az vm create` devuelve los resultados una vez que la máquina virtual se haya creado completamente y que esté lista para usarla y para que se acceda a ella.</span><span class="sxs-lookup"><span data-stu-id="654d6-140">The `az vm create` command output results once the VM has been fully created and is ready to be accessed and used.</span></span>

```Output
{
  "fqdns": "",
  "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM",
  "location": "westus2",
  "macAddress": "xx-xx-xx-xx-xx-xx",
  "powerState": "VM running",
  "privateIpAddress": "xx.x.x.x",
  "publicIpAddress": "xx.xxx.xx.xxx",
  "resourceGroup": "MyResourceGroup"
}
```

<span data-ttu-id="654d6-141">A continuación, inicie sesión en la máquina virtual con Windows Server recién creada mediante el Escritorio remoto y la dirección IP pública de la máquina virtual (que se devuelve en los resultados de `az vm create`).</span><span class="sxs-lookup"><span data-stu-id="654d6-141">Now log on to your newly created Windows Server VM using Remote Desktop and the public IP address of the VM (which is returned in the output from `az vm create`).</span></span>
<span data-ttu-id="654d6-142">Si se encuentra en un sistema basado en Windows, puede hacerlo desde la línea de comandos mediante el comando `mstsc`:</span><span class="sxs-lookup"><span data-stu-id="654d6-142">If you are on a Windows-based system, you can do this from the command line using the `mstsc` command:</span></span>

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

<span data-ttu-id="654d6-143">Especifique la misma combinación de nombre de usuario y contraseña que utilizó al crear la máquina virtual para iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="654d6-143">Supply the same username/password combination you used when creating the VM to log in.</span></span>

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="654d6-144">Creación de otros recursos en Azure</span><span class="sxs-lookup"><span data-stu-id="654d6-144">Creating other resources in Azure</span></span>

<span data-ttu-id="654d6-145">Ya se ha visto cómo se crean un grupo de recursos, una máquina virtual Linux y una VM con Windows Server.</span><span class="sxs-lookup"><span data-stu-id="654d6-145">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="654d6-146">Sin embargo, también se pueden crear muchos otros tipos de recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="654d6-146">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="654d6-147">Todos los recursos nuevos se crean mediante un patrón de nomenclatura de `az <resource type name> create` consistente.</span><span class="sxs-lookup"><span data-stu-id="654d6-147">All new resources are created using a consistent `az <resource type name> create` naming pattern.</span></span>  <span data-ttu-id="654d6-148">Por ejemplo, para crear un equilibrador de carga de red de Azure que luego se pueda asociar con las máquinas virtuales recién creadas, se puede utilizar el siguiente comando create:</span><span class="sxs-lookup"><span data-stu-id="654d6-148">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

<span data-ttu-id="654d6-149">También se puede crear una red virtual privada nueva (que se suele denominar "Virtual Network" en Azure) para nuestra infraestructura con el siguiente comando create:</span><span class="sxs-lookup"><span data-stu-id="654d6-149">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following create command:</span></span>

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

<span data-ttu-id="654d6-150">Lo que hace que tanto Azure como la CLI de Azure sean muy eficaces, es que se pueden usar no solo para obtener una infraestructura en la nube, sino también para crear servicios de plataforma administrados.</span><span class="sxs-lookup"><span data-stu-id="654d6-150">What makes Azure and the Azure CLI powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span>  <span data-ttu-id="654d6-151">Los servicios de plataforma administrados también se pueden combinar con una infraestructura para compilar soluciones aún más eficaces.</span><span class="sxs-lookup"><span data-stu-id="654d6-151">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="654d6-152">Por ejemplo, la CLI de Azure se puede utilizar para crear una instancia de Azure App Service.</span><span class="sxs-lookup"><span data-stu-id="654d6-152">For example, you can use the Azure CLI to create an Azure AppService.</span></span>  <span data-ttu-id="654d6-153">Azure App Service es un servicio de plataforma administrado que proporciona una manera excelente de hospedar aplicaciones web sin tener que preocuparse de la infraestructura.</span><span class="sxs-lookup"><span data-stu-id="654d6-153">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span>  <span data-ttu-id="654d6-154">Después de crear la instancia de Azure App Service, se pueden crear dos nuevas instancias de Azure Web Apps en App Service mediante los siguientes comandos create:</span><span class="sxs-lookup"><span data-stu-id="654d6-154">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following create commands:</span></span>

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan
```

<span data-ttu-id="654d6-155">Una vez que conozca los conceptos básicos del patrón de `az <resource type name> create`, resulta fácil crear cualquier cosa.</span><span class="sxs-lookup"><span data-stu-id="654d6-155">Once you understand the basics of the `az <resource type name> create` pattern, it becomes easy to create anything.</span></span> <span data-ttu-id="654d6-156">A continuación hay varios tipos de recurso de Azure y los correspondientes comandos create de la CLI de Azure para crearlos:</span><span class="sxs-lookup"><span data-stu-id="654d6-156">Following are some popular Azure resource types and the corresponding Azure CLI create commands to create them:</span></span>

```
Resource Type               Azure CLI create command
-------------               ------------------------
Resource Group              az group create
Virtual Machine             az vm create
Virtual Network             az network vnet create
Load Balancer               az network lb create
Managed Disk                az disk create
Storage account             az storage account create
Virtual Machine Scale Set   az vmss create
Azure Container Service     az acs create
Web App                     az webapp create
SQL Database Server         az sql server create
Document DB                 az documentdb create
```

<span data-ttu-id="654d6-157">Para más información acerca de los parámetros adicionales específicos de los recursos que se pueden pasar a cada uno de los comandos anteriores y tipos de recurso que se pueden crear, visite la [documentación de referencia](/cli/azure).</span><span class="sxs-lookup"><span data-stu-id="654d6-157">Visit the [Reference documentation](/cli/azure) to learn more about the additional resource-specific parameters that you can pass to each of the preceding commands and the resource types you can create.</span></span>

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a><span data-ttu-id="654d6-158">Sugerencia útil: optimización de las operaciones create mediante -- no wait</span><span class="sxs-lookup"><span data-stu-id="654d6-158">Useful tip: Optimizing create operations using --no-wait</span></span>

<span data-ttu-id="654d6-159">De forma predeterminada cuando se crean recursos mediante la CLI de Azure 2.0, el comando `az <resource type name> create` espera hasta que el recurso se haya creado y está listo para su uso.</span><span class="sxs-lookup"><span data-stu-id="654d6-159">By default when you create resources using the Azure CLI 2.0, the `az <resource type name> create` command waits until the resource has been created and is ready for you to use.</span></span>  <span data-ttu-id="654d6-160">Por ejemplo, si crea una máquina virtual, de manera predeterminada el comando `az vm create` no se devolverá hasta que la máquina virtual se crea y está lista para usar SSH o RDP en ella.</span><span class="sxs-lookup"><span data-stu-id="654d6-160">For example, if you create a VM, the `az vm create` command will, by default, not return until the VM is created and is ready for you to SSH or RDP into it.</span></span>

<span data-ttu-id="654d6-161">Este enfoque se usa porque facilita la escritura de scripts de automatización que contienen varios pasos con dependencias (y necesitan que se haya completado satisfactoriamente una tarea anterior antes de continuar).</span><span class="sxs-lookup"><span data-stu-id="654d6-161">We use this approach because it makes it easier to write automation scripts that contain multiple steps with dependencies (and need a prior task to have completed successfully before continuing).</span></span>

<span data-ttu-id="654d6-162">Si no tiene que esperar a la creación de un recurso antes de continuar, puede usar la opción `no-wait` para iniciar una acción create en segundo plano.</span><span class="sxs-lookup"><span data-stu-id="654d6-162">If you do not need to wait on creation of a resource before continuing, you can use the `no-wait` option to start a create action in the background.</span></span> <span data-ttu-id="654d6-163">La CLI se puede seguir usando para otros comandos.</span><span class="sxs-lookup"><span data-stu-id="654d6-163">You can continue using the CLI for other commands.</span></span>

<span data-ttu-id="654d6-164">Por ejemplo, el siguiente uso de `az vm create` inicia una implementación de máquina virtual y, después, volver mucho más rápidamente (y antes de que la máquina virtual se haya iniciado totalmente):</span><span class="sxs-lookup"><span data-stu-id="654d6-164">For example, the following usage of the `az vm create` starts a VM deployment and then return much more quickly (and before the VM has fully booted):</span></span>

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

<span data-ttu-id="654d6-165">El uso del enfoque de `--no-wait` puede ayudarle a optimizar considerablemente el rendimiento de los scripts de automatización.</span><span class="sxs-lookup"><span data-stu-id="654d6-165">Using the `--no-wait` approach can help you optimize the performance of your automation scripts considerably.</span></span>

## <a name="listing-resources-and-formatting-output"></a><span data-ttu-id="654d6-166">Enumeración de recursos y aplicación de formato al resultado</span><span class="sxs-lookup"><span data-stu-id="654d6-166">Listing resources and formatting output</span></span>

<span data-ttu-id="654d6-167">El comando `list` se puede usar en la CLI de Azure para buscar y enumerar los recursos que se ejecutan en Azure.</span><span class="sxs-lookup"><span data-stu-id="654d6-167">You can use the `list` command within the Azure CLI to find and list the resources running in Azure.</span></span>

<span data-ttu-id="654d6-168">Al igual que con el comando create, los recursos se pueden enumerar mediante la CLI de Azure 2.0 mediante un patrón de nomenclatura de `az <resource type name> list` que sea coherente con todos los tipos de recursos.</span><span class="sxs-lookup"><span data-stu-id="654d6-168">Like with the create command, you can list resources using the Azure CLI 2.0 using a common `az <resource type name> list` naming pattern that is consistent across all resource types.</span></span>  <span data-ttu-id="654d6-169">Existen varios formatos de salida y opciones de consulta disponibles para filtrar y ordenar la lista de recursos de la forma que prefiera para verlos.</span><span class="sxs-lookup"><span data-stu-id="654d6-169">There are various output formats and query options available to filter and sort the list of resources in the way you prefer to see them.</span></span>

<span data-ttu-id="654d6-170">Por ejemplo, `az vm list` muestra la lista de todas las máquinas virtuales que tiene.</span><span class="sxs-lookup"><span data-stu-id="654d6-170">For example, `az vm list` shows the list of all VMs you have.</span></span>

```azurecli-interactive
az vm list
```
<span data-ttu-id="654d6-171">Los valores que se devuelven están, de forma predeterminada, en JSON (solo que muestra el resultado parcial por motivos de brevedad).</span><span class="sxs-lookup"><span data-stu-id="654d6-171">The values returned are by default in JSON (only showing partial output for sake of brevity).</span></span>

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1_v2"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus2",
    "name": "MyLinuxVM",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "MyResourceGroup"
        }
      ]
    },
          ...
          ...
          ...
]
```

<span data-ttu-id="654d6-172">Opcionalmente, puede modificar el formato de salida mediante la opción `--output`.</span><span class="sxs-lookup"><span data-stu-id="654d6-172">You can optionally modify the output format using the `--output` option.</span></span>  <span data-ttu-id="654d6-173">Ejecute el comando `az vm list` para ver las máquinas virtuales Linux y con Windows Server creadas con anterioridad, junto con las propiedades más comunes de una máquina virtual, mediante la opción de formato de *table* fácil de leer:</span><span class="sxs-lookup"><span data-stu-id="654d6-173">Run the `az vm list` command to see both the Linux and Windows Server VMs created earlier, along with the most common properties of a VM, using the easy to read *table* format option:</span></span>

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="654d6-174">La opción de salida *tsv* se puede utilizar para obtener un formato de texto separado por tabulaciones sin encabezados.</span><span class="sxs-lookup"><span data-stu-id="654d6-174">The *tsv* output option can be used to get a text-based, tab-separated format without any headers.</span></span>  <span data-ttu-id="654d6-175">Este formato resulta útil cuando se desea canalizar la salida a otra herramienta de texto como grep.</span><span class="sxs-lookup"><span data-stu-id="654d6-175">This format is useful when you want to pipe the output into another text-based tool like grep.</span></span>

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
<span data-ttu-id="654d6-176">Consulte el artículo acerca de los [formatos de salida](format-output-azure-cli.md) para obtener más información sobre formas adicionales de enumerar recursos y dar formato al resultado.</span><span class="sxs-lookup"><span data-stu-id="654d6-176">Visit the [output formats](format-output-azure-cli.md) article to learn more about the additional ways to list resources and format the output.</span></span>

## <a name="querying-resources-and-shaping-outputs"></a><span data-ttu-id="654d6-177">Consulta de recursos y forma de las salidas</span><span class="sxs-lookup"><span data-stu-id="654d6-177">Querying resources and shaping outputs</span></span>

<span data-ttu-id="654d6-178">A menudo desea poder consultar solo los recursos que cumplan una condición concreta.</span><span class="sxs-lookup"><span data-stu-id="654d6-178">Often you want to be able to query for only those resources that meet a specific condition.</span></span>

<span data-ttu-id="654d6-179">El comando `list` tiene compatibilidad integrada, lo que facilita el filtro de los recursos por nombre de grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="654d6-179">The `list` command has built-in support that makes it easy to filter resources by Resource Group name.</span></span>  <span data-ttu-id="654d6-180">Por ejemplo, puede usar un parámetro `--ResourceGroup` o `-g` con un comando `list` para recuperar solo los recursos de un grupo de recursos concreto:</span><span class="sxs-lookup"><span data-stu-id="654d6-180">For example, you can pass either a `--ResourceGroup` or `-g` parameter to a `list` command to only retrieve those resources within a specific resource group:</span></span>


```azurecli-interactive
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

<span data-ttu-id="654d6-181">Para que el soporte técnico de las consultas sea aún más eficaz, puede usar el parámetro `--query` para ejecutar una consulta JMESPath en los resultados de *cualquier* comando `az`.</span><span class="sxs-lookup"><span data-stu-id="654d6-181">For even more powerful querying support, you can use the `--query` parameter to execute a JMESPath query on the results of *any* `az` command.</span></span>  <span data-ttu-id="654d6-182">Las consultas JMESPath se pueden usar tanto para filtrar como para dar forma a la salida de todos los resultados devueltos.</span><span class="sxs-lookup"><span data-stu-id="654d6-182">JMESPath queries can be used both to filter as well as shape the output of any returned result.</span></span>

<span data-ttu-id="654d6-183">Por ejemplo, ejecute el siguiente comando para consultar si algún recurso de máquina virtual de todos los grupos de recursos contiene las letras "My":</span><span class="sxs-lookup"><span data-stu-id="654d6-183">For example, execute the following command to query for any VM resource within any resource group that contains the letters "My":</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup, 'MY')]"
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="654d6-184">Luego, también puede refinar más el resultado mediante el uso de la funcionalidad de moldeado de las consultas JMESPath para generar valores diferentes.</span><span class="sxs-lookup"><span data-stu-id="654d6-184">We could then choose to further refine the output by using the shaping capability of JMESPath queries to output different values as well.</span></span>  <span data-ttu-id="654d6-185">Por ejemplo, el siguiente comando recupera el tipo de disco del sistema operativo que usa la máquina virtual para determinar si el sistema operativo es Linux o Windows:</span><span class="sxs-lookup"><span data-stu-id="654d6-185">For example, the following command retrieves the type of OS disk the VM is using to determine whether the OS is Linux or Windows based:</span></span>

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup, 'MY')].{ VMName:name, OSType:storageProfile.osDisk.osType }"
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

<span data-ttu-id="654d6-186">La compatibilidad con JMESPath de la CLI de Azure es eficaz.</span><span class="sxs-lookup"><span data-stu-id="654d6-186">The JMESPath support in Azure CLI is powerful.</span></span>  <span data-ttu-id="654d6-187">Para más información acerca de cómo utilizarla, consulte el siguiente artículo acerca de las [consultas](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="654d6-187">Learn more about how to use it in our [query](query-azure-cli.md) article.</span></span>

## <a name="deleting-resources"></a><span data-ttu-id="654d6-188">Eliminación de recursos</span><span class="sxs-lookup"><span data-stu-id="654d6-188">Deleting resources</span></span>

<span data-ttu-id="654d6-189">Puede usar el comando `delete` de la CLI de Azure para eliminar los recursos que no necesite.</span><span class="sxs-lookup"><span data-stu-id="654d6-189">You can use the `delete` command within Azure CLI to delete the resources you no longer need.</span></span> <span data-ttu-id="654d6-190">El comando `delete` se puede usar con cualquier recurso, exactamente igual que sucede con el comando `create`.</span><span class="sxs-lookup"><span data-stu-id="654d6-190">You can use the `delete` command with any resource just like you can with the `create` command.</span></span>

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

<span data-ttu-id="654d6-191">De manera predeterminada la CLI solicita que se confirme la eliminación.</span><span class="sxs-lookup"><span data-stu-id="654d6-191">By default the CLI prompts to confirm deletion.</span></span>  <span data-ttu-id="654d6-192">Este mensaje se puede en los scripts automatizados.</span><span class="sxs-lookup"><span data-stu-id="654d6-192">You can suppress this prompt for automated scripts.</span></span>

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

<span data-ttu-id="654d6-193">También se puede usar el comando `delete` para eliminar varios recursos a la vez.</span><span class="sxs-lookup"><span data-stu-id="654d6-193">You can also use the `delete` command to delete many resources at a time.</span></span> <span data-ttu-id="654d6-194">Por ejemplo, el siguiente comando elimina todos los recursos del grupo de recursos "MyResourceGroup" que hemos usado para todos los ejemplos de este tutorial de introducción.</span><span class="sxs-lookup"><span data-stu-id="654d6-194">For example, the following command deletes all the resources in the "MyResourceGroup" resource group that we've used for all the samples in this Get Started tutorial.</span></span>

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a><span data-ttu-id="654d6-195">Obtención de ejemplos</span><span class="sxs-lookup"><span data-stu-id="654d6-195">Get samples</span></span>

<span data-ttu-id="654d6-196">Para más información acerca de las distintas formas de usar la CLI de Azure, consulte nuestro scripts más comunes para [máquinas virtuales Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [máquinas virtuales Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) y [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span><span class="sxs-lookup"><span data-stu-id="654d6-196">To learn more about ways to use the Azure CLI, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), and [SQL Database](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).</span></span>

## <a name="read-the-api-reference-docs"></a><span data-ttu-id="654d6-197">Lectura de los documentos de referencia de la API</span><span class="sxs-lookup"><span data-stu-id="654d6-197">Read the API reference docs</span></span>

[<span data-ttu-id="654d6-198">Referencia de API</span><span class="sxs-lookup"><span data-stu-id="654d6-198">API reference</span></span>](/cli/azure)

## <a name="get-help"></a><span data-ttu-id="654d6-199">Obtención de ayuda</span><span class="sxs-lookup"><span data-stu-id="654d6-199">Get help</span></span>

<span data-ttu-id="654d6-200">La CLI de Azure tiene documentación de ayuda integrada, que coincide con la documentación web que se puede ejecutar desde la línea de comandos:</span><span class="sxs-lookup"><span data-stu-id="654d6-200">The Azure CLI has built-in help documentation, which matches our web documentation that you can run from the command line:</span></span>

```azurecli-interactive
az [command-group [command]] -h
```

<span data-ttu-id="654d6-201">Por ejemplo, para ver los comandos y subgrupos disponibles para las máquinas virtuales, use:</span><span class="sxs-lookup"><span data-stu-id="654d6-201">For example, to see what commands and subgroups are available for VMs, use:</span></span>

```azurecli-interactive
az vm -h
```

<span data-ttu-id="654d6-202">Para obtener ayuda acerca del comando para crear máquinas virtuales, use:</span><span class="sxs-lookup"><span data-stu-id="654d6-202">To get help with the command to create a VM, use:</span></span>

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a><span data-ttu-id="654d6-203">Cambio desde la CLI de Azure 1.0</span><span class="sxs-lookup"><span data-stu-id="654d6-203">Switch from Azure CLI 1.0</span></span>

<span data-ttu-id="654d6-204">Si ya sabe usar la CLI de Azure 1.0 (azure.js), se dará cuenta de que hay sitios en los que los comandos no son exactamente los mismos.</span><span class="sxs-lookup"><span data-stu-id="654d6-204">If you already know how to use Azure CLI 1.0 (azure.js), you'll notice places where the commands aren't quite the same.</span></span>
<span data-ttu-id="654d6-205">En ocasiones, los comandos para realizar una tarea son considerablemente diferentes.</span><span class="sxs-lookup"><span data-stu-id="654d6-205">Sometimes the commands to perform a task are significantly different.</span></span>
<span data-ttu-id="654d6-206">Para ayudarle a pasar de la CLI de Azure 1.0 a la 2.0, hemos iniciado esta [asignación de comandos](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span><span class="sxs-lookup"><span data-stu-id="654d6-206">To help you make the switch from Azure CLI 1.0 to Azure CLI 2.0, we've started this [command mapping](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).</span></span>

## <a name="send-us-your-feedback"></a><span data-ttu-id="654d6-207">Envíenos sus comentarios</span><span class="sxs-lookup"><span data-stu-id="654d6-207">Send us your feedback</span></span>

```azurecli-interactive
az feedback
```
