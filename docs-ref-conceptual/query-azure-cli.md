---
title: Resultados del comando de consulta con la CLI de Azure 2.0
description: Use el comando --query para realizar consultas JMESPath en la salida de los comandos de la CLI de Azure 2.0.
keywords: CLI de Azure 2.0, JMESPath, consulta, Linux, Mac, Windows, OS X
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 5979acc5-21a5-41e2-a4b6-3183bfe6aa22
ms.openlocfilehash: 23c743210ccc506935f6e78489ca0df2b99d46a1
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2017
---
# <a name="using-jmespath-queries-with-azure-cli-20"></a>Uso de consultas JMESPath con la CLI de Azure 2.0

La CLI de Azure 2.0 utiliza el parámetro `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados del comando `az`. JMESPath es un potente lenguaje de consulta para salidas JSON.  Si no está familiarizado con las consultas JMESPath encontrará un tutorial en [JMESPath.org/tutorial](http:/JMESPath.org/tutorial.html).

El parámetro `Query` es compatible con todos los tipos de recurso (Container Services, Web Apps, VM, etc.) de la CLI de Azure 2.0 y puede usarse para varios propósitos diferentes.  Se muestran varios ejemplos a continuación.

## <a name="selecting-simple-properties"></a>Selección de propiedades simples

El sencillo comando `list` con el formato de salida `table` devuelve un conjunto protegido con las propiedades más comunes y sencillas de cada tipo de recurso en un formato tabular fácil de leer.

```azurecli-interactive
az vm list --out table
```

```
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

Puede usar el parámetro `--query` para que muestre únicamente el nombre del grupo de recursos y el de la máquina virtual para todas las máquinas virtuales de su suscripción.

```azurecli-interactive
az vm list \
  --query [*].[name,resourceGroup] --out table
```

```
Column1     Column2
---------   -----------
DemoVM010   DEMORG1
demovm111   DEMORG1
demovm211   DEMORG1
demovm212   DEMORG1
demovm213   DEMORG1
demovm214   DEMORG1
demovm222   DEMORG1
KBDemo001VM RGDEMO001
KBDemo020   RGDEMO001
```

En el ejemplo anterior, observe que los encabezados de columna son "Columna1" y "Columna2".  Puede también agregar etiquetas o nombres descriptivos a las propiedades que seleccione.  En el ejemplo siguiente, se agregaron las etiquetas "VMName" y "RGName" a las propiedades seleccionadas "name" y "resourceGroup".


```azurecli-interactive
az vm list \
  --query "[].{RGName:resourceGroup, VMName:name}" --out table
```

```
RGName     VMName
---------  -----------
DEMORG1    DemoVM010
DEMORG1    demovm111
DEMORG1    demovm211
DEMORG1    demovm212
DEMORG1    demovm213
DEMORG1    demovm214
DEMORG1    demovm222
RGDEMO001  KBDemo001VM
RGDEMO001  KBDemo020
```

## <a name="selecting-complex-nested-properties"></a>Selección de propiedades complejas anidadas

Si la propiedad que desea seleccionar está muy anidada en la salida JSON, debe proporcionar la ruta de acceso completa a la propiedad anidada. En el ejemplo siguiente se muestra cómo seleccionar el nombre de la máquina virtual y el tipo de sistema operativo mediante el comando de lista vm.

```azurecli-interactive
az vm list \
  --query "[].{VMName:name,OSType:storageProfile.osDisk.osType}" --out table
```

```
VMName       OSType
-----------  --------
DemoVM010    Linux
demovm111    Linux
demovm211    Linux
demovm212    Linux
demovm213    Linux
demovm214    Linux
demovm222    Linux
KBDemo001VM  Linux
KBDemo020    Linux
```

## <a name="filter-with-the-contains-function"></a>Filtrado con la función Contains

Puede usar la función `contains` de JMESPath para refinar los resultados devueltos en la consulta.
En el ejemplo siguiente, el comando selecciona solo las máquinas virtuales con el texto "RGD" en su nombre.  

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup,'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

En el ejemplo siguiente, los resultados devolverán las máquinas virtuales que tengan el vmSize 'Standard_DS1'.

```azurecli-interactive
az vm list \
  --query "[?contains(hardwareProfile.vmSize, 'Standard_DS1')]" --out table
```

```
ResourceGroup    VMName     VmId                                  Location    ProvisioningState
---------------  ---------  ------------------------------------  ----------  -------------------
DEMORG1          DemoVM010  cbd56d9b-9340-44bc-a722-25f15b578444  westus      Succeeded
DEMORG1          demovm111  c1c024eb-3837-4075-9117-bfbc212fa7da  westus      Succeeded
DEMORG1          demovm211  95eda642-417f-4036-9475-67246ac0f0d0  westus      Succeeded
DEMORG1          demovm212  4bdac85d-c2f7-410f-9907-ca7921d930b4  westus      Succeeded
DEMORG1          demovm213  2131c664-221a-4b7f-9653-f6d542fbfa34  westus      Succeeded
DEMORG1          demovm214  48f419af-d27a-4df0-87f3-9481007c2e5a  westus      Succeeded
DEMORG1          demovm222  e0f59516-1d69-4d54-b8a2-f6c4a5d031de  westus      Succeeded
```

## <a name="filter-with-grep"></a>Filtrado con grep

El formato de salida `tsv` es un texto separado por tabulaciones sin encabezados. Se puede canalizar a comandos como `grep` y `cut` para analizar aún más los valores específicos de la salida `list`. En el ejemplo siguiente, el comando `grep` selecciona solo las máquinas virtuales con el texto "RGD" en su nombre.  El comando `cut` selecciona solo el valor del octavo campo (separado por tabulaciones) para mostrarlo en la salida.

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a>Exploración con jpterm

También se puede canalizar la salida del comando a [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) y experimentar con la consulta JMESPath allí.

```bash
pip install jmespath-terminal
az vm list | jpterm
```

