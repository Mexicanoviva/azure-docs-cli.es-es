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
ms.openlocfilehash: 274336acbf09a21d45b6ef3868f5f7f21757831b
ms.sourcegitcommit: 21c42ed07c9f7679e4860013ac5647cf31213f4e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/22/2017
---
# <a name="get-started-with-azure-cli-20"></a>Introducción a la CLI de Azure 2.0

La CLI de Azure 2.0 es la nueva forma de usar la línea de comandos de Azure para administrar recursos de Azure.
Puede usarla en el explorador con [Azure Cloud Shell](/azure/cloud-shell/overview) o puede [instalarla](install-azure-cli.md) en macOS, Linux y Windows y ejecutarla desde la línea de comandos.

La CLI de Azure 2.0 está optimizada para administrar recursos de Azure desde la línea de comandos y para generar scripts de automatización que funcionan con Azure Resource Manager.
Este artículo le ayuda a empezar a usarlo y explica los conceptos básicos que hay detrás.

Para más información sobre la versión más reciente, consulte las [notas de la versión](release-notes-azure-cli.md).

## <a name="connect"></a>Conectar

La manera más sencilla de empezar es [iniciar Cloud Shell](/azure.cloud-shell/quickstart).

1. Inicie Cloud Shell en la navegación superior de Azure Portal.

   ![Icono de Shell](media/get-started-with-azure-cli/shell-icon.png)

2. Elija la suscripción que desea utilizar y cree una cuenta de almacenamiento.

   ![Crear una cuenta de almacenamiento](media/get-started-with-azure-cli/storage-prompt.png)

También puede [instalar](install-azure-cli.md) la CLI y ejecutarla localmente desde la línea de comandos.

## <a name="create-a-resource-group"></a>Creación de un grupo de recursos

Ahora que todo está configurado, vamos a usar la CLI de Azure para crear recursos en Azure.

En primer lugar, cree un grupo de recursos.  En Azure, los grupos de recursos proporcionan una manera de administrar varios recursos que se desean agrupar de manera lógica.  Por ejemplo, puede crear un grupo de recursos para una aplicación o un proyecto, y agregar una máquina virtual, una base de datos y un servicio de CDN en él.

Vamos a crear un grupo de recursos denominado "MyResourceGroup" en la región *oesteeeuu2* de Azure.  Para ello, escriba el siguiente comando:

```azurecli-interactive
az group create -n MyResourceGroup -l westus2 
```

Una vez que se haya creado el grupo de recursos, el comando `az group create` genera varias propiedades del recursos recién creado:

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

## <a name="create-a-linux-virtual-machine"></a>Creación de una máquina virtual Linux

Ahora que tenemos nuestro grupo de recursos, vamos a crear una máquina virtual Linux en él.

Puede crear una máquina virtual Linux con la popular imagen de UbuntuTLS, con dos discos de almacenamiento conectados de 10 GB y 20 GB, con el siguiente comando:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --data-disk-sizes-gb 10 20
```

Al ejecutar el comando anterior, la CLI de Azure 2.0 busca un par de claves SSH almacenadas en el directorio ~/.ssh.  Si aún no tiene un par de claves SSH almacenadas ahí, puede pedir a la CLI de Azure que lo cree automáticamente pasando el parámetro --parámetro --generate-ssh-keys:

```azurecli-interactive
az vm create -n MyLinuxVM -g MyResourceGroup --image UbuntuLTS --generate-ssh-keys
```

El comando `az vm create` devuelve la salida una vez que la máquina virtual se haya creado completamente y que esté lista para usarla y para que se acceda a ella. La salida incluye varias propiedades de la máquina virtual recién creada, entre las que se incluye la dirección IP pública:

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

Una vez creada la máquina virtual, puede iniciar sesión en la nueva máquina virtual Linux mediante **SSH** con la dirección IP pública de la máquina virtual que ha creado:

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

## <a name="create-a-windows-server-virtual-machine"></a>Creación de una máquina virtual con Windows Server

Ahora se va a crear una máquina virtual basada en Windows Server 2016 Datacenter mediante el comando `az vm create` y a agregarla al mismo grupo de recursos "MyResourceGroup" que se ha usado para la máquina virtual Linux.  Al igual que en el ejemplo de la máquina virtual Linux también se van a conectar dos discos de almacenamiento mediante el parámetro `--data-disk-sizes-gb`.

Azure requiere que se evite usar nombres de usuario o contraseñas que se adivinen con facilidad. Hay reglas específicas relativas a los caracteres que se pueden usar, así como a la longitud mínima del nombre de usuario y de la contraseña.  

> [!NOTE]
> Al ejecutar este comando, se le pedirá que escriba el nombre de usuario y la contraseña.

```azurecli-interactive
az vm create -n MyWinVM -g MyResourceGroup --image Win2016Datacenter
```

El comando `az vm create` devuelve los resultados una vez que la máquina virtual se haya creado completamente y que esté lista para usarla y para que se acceda a ella.

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

A continuación, inicie sesión en la máquina virtual con Windows Server recién creada mediante el Escritorio remoto y la dirección IP pública de la máquina virtual (que se devuelve en los resultados de `az vm create`).  
Si se encuentra en un sistema basado en Windows, puede hacerlo desde la línea de comandos mediante el comando `mstsc`:

```azurecli-interactive
mstsc /v:xx.xxx.xx.xxx
```

Especifique la misma combinación de nombre de usuario y contraseña que utilizó al crear la máquina virtual para iniciar sesión.

## <a name="creating-other-resources-in-azure"></a>Creación de otros recursos en Azure

Ya se ha visto cómo se crean un grupo de recursos, una máquina virtual Linux y una VM con Windows Server. Sin embargo, también se pueden crear muchos otros tipos de recursos de Azure.  

Todos los recursos nuevos se crean mediante un patrón de nomenclatura de `az <resource type name> create` consistente.  Por ejemplo, para crear un equilibrador de carga de red de Azure que luego se pueda asociar con las máquinas virtuales recién creadas, se puede utilizar el siguiente comando create:

```azurecli-interactive
az network lb create -n MyLoadBalancer -g MyResourceGroup
```

También se puede crear una red virtual privada nueva (que se suele denominar "Red virtual" en Azure) para nuestra infraestructura con el siguiente comando create:

```azurecli-interactive
az network vnet create -n MyVirtualNetwork -g MyResourceGroup --address-prefix 10.0.0.0/16
```

Lo que hace que tanto Azure como la CLI de Azure sean muy eficaces, es que se pueden usar no solo para obtener una infraestructura en la nube, sino también para crear servicios de plataforma administrados.  Los servicios de plataforma administrados también se pueden combinar con una infraestructura para compilar soluciones aún más eficaces.

Por ejemplo, la CLI de Azure se puede utilizar para crear una instancia de Azure App Service.  Azure App Service es un servicio de plataforma administrado que proporciona una manera excelente de hospedar aplicaciones web sin tener que preocuparse de la infraestructura.  Después de crear la instancia de Azure App Service, se pueden crear dos nuevas instancias de Azure Web Apps en App Service mediante los siguientes comandos create:

```azurecli-interactive
# Create an Azure AppService that we can host any number of web apps within
az appservice plan create -n MyAppServicePlan -g MyResourceGroup

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
az webapp create -n MyWebApp43432 -g MyResourceGroup --plan MyAppServicePlan 
az webapp create -n MyWebApp43433 -g MyResourceGroup --plan MyAppServicePlan 
```

Una vez que conozca los conceptos básicos del patrón de `az <resource type name> create`, resulta fácil crear cualquier cosa. A continuación hay varios tipos de recurso de Azure y los correspondientes comandos create de la CLI de Azure para crearlos:

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

Para más información acerca de los parámetros adicionales específicos de los recursos que se pueden pasar a cada uno de los comandos anteriores y tipos de recurso que se pueden crear, visite la [documentación de referencia](/cli/azure). 

## <a name="useful-tip-optimizing-create-operations-using---no-wait"></a>Sugerencia útil: optimización de las operaciones create mediante -- no wait

De forma predeterminada cuando se crean recursos mediante la CLI de Azure 2.0, el comando `az <resource type name> create` espera hasta que el recurso se haya creado y está listo para su uso.  Por ejemplo, si crea una máquina virtual, de manera predeterminada el comando `az vm create` no se devolverá hasta que la máquina virtual se crea y está lista para usar SSH o RDP en ella.

Este enfoque se usa porque facilita la escritura de scripts de automatización que contienen varios pasos con dependencias (y necesitan que se haya completado satisfactoriamente una tarea anterior antes de continuar).

Si no tiene que esperar a la creación de un recurso antes de continuar, puede usar la opción `no-wait` para iniciar una acción create en segundo plano. La CLI se puede seguir usando para otros comandos.

Por ejemplo, el siguiente uso de `az vm create` inicia una implementación de máquina virtual y, después, volver mucho más rápidamente (y antes de que la máquina virtual se haya iniciado totalmente):

```azurecli-interactive
az vm create -n MyLinuxVM2 -g MyResourceGroup --image UbuntuLTS --no-wait
```

El uso del enfoque de `--no-wait` puede ayudarle a optimizar considerablemente el rendimiento de los scripts de automatización.

## <a name="listing-resources-and-formatting-output"></a>Enumeración de recursos y aplicación de formato al resultado

El comando `list` se puede usar en la CLI de Azure para buscar y enumerar los recursos que se ejecutan en Azure. 

Al igual que con el comando create, los recursos se pueden enumerar mediante la CLI de Azure 2.0 mediante un patrón de nomenclatura de `az <resource type name> list` que sea coherente con todos los tipos de recursos.  Existen varios formatos de salida y opciones de consulta disponibles para filtrar y ordenar la lista de recursos de la forma que prefiera para verlos.

Por ejemplo, `az vm list` muestra la lista de todas las máquinas virtuales que tiene.   

```azurecli-interactive
az vm list 
```
Los valores que se devuelven están, de forma predeterminada, en JSON (solo que muestra el resultado parcial por motivos de brevedad).

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

Opcionalmente, puede modificar el formato de salida mediante la opción `--output`.  Ejecute el comando `az vm list` para ver las máquinas virtuales Linux y con Windows Server creadas con anterioridad, junto con las propiedades más comunes de una máquina virtual, mediante la opción de formato de *table* fácil de leer:

```azurecli-interactive
az vm list --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

La opción de salida *tsv* se puede utilizar para obtener un formato de texto separado por tabulaciones sin encabezados.  Este formato resulta útil cuando se desea canalizar la salida a otra herramienta de texto como grep. 

```azurecli-interactive
az vm list --output tsv
```

```
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyLinuxVM        None    None    westus2 MyLinuxVM                   None        Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
None    None            /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/MyResourceGroup/providers/Microsoft.Compute/virtualMachines/MyWinVM  None    None    westus2 MyWinVM                 None    Succeeded       MyResourceGroup None                    Microsoft.Compute/virtualMachines       XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```
Consulte el artículo acerca de los [formatos de salida](format-output-azure-cli.md) para obtener más información sobre formas adicionales de enumerar recursos y dar formato al resultado.

## <a name="querying-resources-and-shaping-outputs"></a>Consulta de recursos y forma de las salidas

A menudo desea poder consultar solo los recursos que cumplan una condición concreta.  

El comando `list` tiene compatibilidad integrada, lo que facilita el filtro de los recursos por nombre de grupo de recursos.  Por ejemplo, puede usar un parámetro `--ResourceGroup` o `-g` con un comando `list` para recuperar solo los recursos de un grupo de recursos concreto:


```azurecli
az vm list -g MyResourceGroup --output table
```

```Output
Name       ResourceGroup    Location
---------  ---------------  ----------
MyLinuxVM  MyResourceGroup  westus2
MyWinVM    MyResourceGroup  westus2
```

Para que el soporte técnico de las consultas sea aún más eficaz, puede usar el parámetro `--query` para ejecutar una consulta JMESPath en los resultados de *cualquier* comando `az`.  Las consultas JMESPath se pueden usar tanto para filtrar como para dar forma a la salida de todos los resultados devueltos.

Por ejemplo, ejecute el siguiente comando para consultar si algún recurso de máquina virtual de todos los grupos de recursos contiene las letras "My":

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')]" 
```

```Output
ResourceGroup    ProvisioningState    Name       Location    VmId
---------------  -------------------  ---------  ----------  ------------------------------------
MYRESOURCEGROUP  Succeeded            MyLinuxVM  westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
MYRESOURCEGROUP  Succeeded            MyWinVM    westus2     XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

Luego, también puede refinar más el resultado mediante el uso de la funcionalidad de moldeado de las consultas JMESPath para generar valores diferentes.  Por ejemplo, el siguiente comando recupera el tipo de disco del sistema operativo que usa la máquina virtual para determinar si el sistema operativo es Linux o Windows:

```azurecli-interactive
az vm list --output table --query "[?contains(resourceGroup,'MY')].{ VMName:name,OSType:storageProfile.osDisk.osType }" 
```

```Output
VMName     OSType
---------  --------
MyLinuxVM  Linux
MyWinVM    Windows
```

La compatibilidad con JMESPath de la CLI de Azure es eficaz.  Para más información acerca de cómo utilizarla, consulte el siguiente artículo acerca de las [consultas](query-azure-cli.md).

## <a name="deleting-resources"></a>Eliminación de recursos

Puede usar el comando `delete` de la CLI de Azure para eliminar los recursos que no necesite. El comando `delete` se puede usar con cualquier recurso, exactamente igual que sucede con el comando `create`.

```azurecli-interactive
az vm delete -n MyLinuxVM -g MyResourceGroup
```

De manera predeterminada la CLI solicita que se confirme la eliminación.  Este mensaje se puede en los scripts automatizados.

```Output
Are you sure you want to perform this operation? (y/n): y
EndTime                           Name                                  StartTime                         Status
--------------------------------  ------------------------------------  --------------------------------  ---------
2017-02-19T02:35:56.678905+00:00  5b74ab80-9b29-4329-b483-52b406583e2f  2017-02-19T02:33:35.372769+00:00  Succeeded
```

También se puede usar el comando `delete` para eliminar varios recursos a la vez. Por ejemplo, el siguiente comando elimina todos los recursos del grupo de recursos "MyResourceGroup" que hemos usado para todos los ejemplos de este tutorial de introducción.

```azurecli-interactive
az group delete -n MyResourceGroup
```

```Output
Are you sure you want to perform this operation? (y/n): y
```

## <a name="get-samples"></a>Obtención de ejemplos

Para más información acerca de las distintas formas de usar la CLI de Azure, consulte nuestro scripts más comunes para [máquinas virtuales Linux](/azure/virtual-machines/virtual-machines-linux-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [máquinas virtuales Windows](/azure/virtual-machines/virtual-machines-windows-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json) y [base de datos SQL](/azure/sql-database/sql-database-cli-samples?toc=%2fcli%2fazure%2ftoc.json&bc=%2fcli%2fazure%2fbreadcrumb%2ftoc.json).

## <a name="read-the-api-reference-docs"></a>Lectura de los documentos de referencia de la API

[Referencia de API](/cli/azure)

## <a name="get-help"></a>Obtención de ayuda

La CLI de Azure tiene documentación de ayuda integrada, que coincide con la documentación web que se puede ejecutar desde la línea de comandos:

```azurecli-interactive
az [command-group [command]] -h
```

Por ejemplo, para ver los comandos y subgrupos disponibles para las máquinas virtuales, use:

```azurecli-interactive
az vm -h
```

Para obtener ayuda acerca del comando para crear máquinas virtuales, use:

```azurecli-interactive
az vm create -h
```

## <a name="switch-from-azure-cli-10"></a>Cambio desde la CLI de Azure 1.0

Si ya sabe usar la CLI de Azure 1.0 (azure.js), se dará cuenta de que hay sitios en los que los comandos no son exactamente los mismos.
En ocasiones, los comandos para realizar una tarea son considerablemente diferentes.
Para ayudarle a pasar de la CLI de Azure 1.0 a la 2.0, hemos iniciado esta [asignación de comandos](https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst).

## <a name="send-us-your-feedback"></a>Envíenos sus comentarios

```azurecli-interactive
az feedback
```
