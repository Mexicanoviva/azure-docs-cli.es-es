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
ms.openlocfilehash: 0de18adc91589377d4f96a306a70c9adfeabdcab
ms.sourcegitcommit: 8606f36963e8daa6448d637393d1e4ef2c9859a0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/01/2018
---
# <a name="using-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="d8ab6-104">Uso de consultas JMESPath con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="d8ab6-104">Using JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="d8ab6-105">La CLI de Azure 2.0 utiliza el parámetro `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados del comando `az`.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-105">The Azure CLI 2.0 uses the `--query` parameter to execute a [JMESPath query](http://jmespath.org) on the results of your `az` command.</span></span> <span data-ttu-id="d8ab6-106">JMESPath es un potente lenguaje de consulta para salidas JSON.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-106">JMESPath is a powerful query language for JSON outputs.</span></span>  <span data-ttu-id="d8ab6-107">Si no está familiarizado con las consultas JMESPath encontrará un tutorial en [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="d8ab6-107">If you are unfamiliar with JMESPath queries you can find a tutorial at [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span></span>

<span data-ttu-id="d8ab6-108">El parámetro `Query` es compatible con todos los tipos de recurso (Container Services, Web Apps, VM, etc.) de la CLI de Azure 2.0 y puede usarse para varios propósitos diferentes.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-108">`Query` parameter is supported by every resource type (Container Services, Web Apps, VM, etc.) within Azure CLI 2.0 and can be used for various different purposes.</span></span>  <span data-ttu-id="d8ab6-109">Se muestran varios ejemplos a continuación.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-109">We have listed several examples below.</span></span>

## <a name="selecting-simple-properties"></a><span data-ttu-id="d8ab6-110">Selección de propiedades simples</span><span class="sxs-lookup"><span data-stu-id="d8ab6-110">Selecting simple properties</span></span>

<span data-ttu-id="d8ab6-111">El sencillo comando `list` con el formato de salida `table` devuelve un conjunto protegido con las propiedades más comunes y sencillas de cada tipo de recurso en un formato tabular fácil de leer.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-111">The simple `list` command with `table` output format returns a curated set of most common, simple properties for each resource type in an easy-to-read tabular format.</span></span>

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

<span data-ttu-id="d8ab6-112">Puede usar el parámetro `--query` para que muestre únicamente el nombre del grupo de recursos y el de la máquina virtual para todas las máquinas virtuales de su suscripción.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-112">You can use the `--query` parameter to show just the Resource Group name and VM name for all virtual machines in your subscription.</span></span>

```azurecli-interactive
az vm list \
  --query "[].[name, resourceGroup]" --out table
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

<span data-ttu-id="d8ab6-113">En el ejemplo anterior, observe que los encabezados de columna son "Columna1" y "Columna2".</span><span class="sxs-lookup"><span data-stu-id="d8ab6-113">In the previous example, you notice that the column headings are "Column1" and "Column2".</span></span>  <span data-ttu-id="d8ab6-114">Puede también agregar etiquetas o nombres descriptivos a las propiedades que seleccione.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-114">You can add friendly labels or names to the properties you select, as well.</span></span>  <span data-ttu-id="d8ab6-115">En el ejemplo siguiente, se agregaron las etiquetas "VMName" y "RGName" a las propiedades seleccionadas "name" y "resourceGroup".</span><span class="sxs-lookup"><span data-stu-id="d8ab6-115">In the following example, we added the labels "VMName" and "RGName" to the selected properties "name" and "resourceGroup".</span></span>


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

## <a name="selecting-complex-nested-properties"></a><span data-ttu-id="d8ab6-116">Selección de propiedades complejas anidadas</span><span class="sxs-lookup"><span data-stu-id="d8ab6-116">Selecting complex nested properties</span></span>

<span data-ttu-id="d8ab6-117">Si la propiedad que desea seleccionar está muy anidada en la salida JSON, debe proporcionar la ruta de acceso completa a la propiedad anidada.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-117">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="d8ab6-118">En el ejemplo siguiente se muestra cómo seleccionar el nombre de la máquina virtual y el tipo de sistema operativo mediante el comando de lista vm.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-118">The following example shows how to select the VMName and the OS type from the vm list command.</span></span>

```azurecli-interactive
az vm list \
  --query "[].{VMName:name, OSType:storageProfile.osDisk.osType}" --out table
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

## <a name="filter-with-the-contains-function"></a><span data-ttu-id="d8ab6-119">Filtrado con la función Contains</span><span class="sxs-lookup"><span data-stu-id="d8ab6-119">Filter with the contains function</span></span>

<span data-ttu-id="d8ab6-120">Puede usar la función `contains` de JMESPath para refinar los resultados devueltos en la consulta.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-120">You can use the JMESPath `contains` function to refine your results returned in the query.</span></span>
<span data-ttu-id="d8ab6-121">En el ejemplo siguiente, el comando selecciona solo las máquinas virtuales con el texto "RGD" en su nombre.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-121">In the following example, the command selects only VMs that have the text "RGD" in their name.</span></span>

```azurecli-interactive
az vm list \
  --query "[?contains(resourceGroup, 'RGD')].{ resource: resourceGroup, name: name }" --out table
```

```
Resource    VMName
----------  -----------
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

<span data-ttu-id="d8ab6-122">En el ejemplo siguiente, los resultados devolverán las máquinas virtuales que tengan el vmSize 'Standard_DS1'.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-122">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1'.</span></span>

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

## <a name="filter-with-grep"></a><span data-ttu-id="d8ab6-123">Filtrado con grep</span><span class="sxs-lookup"><span data-stu-id="d8ab6-123">Filter with grep</span></span>

<span data-ttu-id="d8ab6-124">El formato de salida `tsv` es un texto separado por tabulaciones sin encabezados.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-124">The `tsv` output format is a tab-separated text with no headers.</span></span> <span data-ttu-id="d8ab6-125">Se puede canalizar a comandos como `grep` y `cut` para analizar aún más los valores específicos de la salida `list`.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-125">It can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="d8ab6-126">En el ejemplo siguiente, el comando `grep` selecciona solo las máquinas virtuales con el texto "RGD" en su nombre.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-126">In the following example, the `grep` command selects only VMs that have text "RGD" in their name.</span></span>  <span data-ttu-id="d8ab6-127">El comando `cut` selecciona solo el valor del octavo campo (separado por tabulaciones) para mostrarlo en la salida.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-127">The `cut` command selects only the 8th field (separated by tabs) value to show in the output.</span></span>

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a><span data-ttu-id="d8ab6-128">Exploración con jpterm</span><span class="sxs-lookup"><span data-stu-id="d8ab6-128">Explore with jpterm</span></span>

<span data-ttu-id="d8ab6-129">También se puede canalizar la salida del comando a [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) y experimentar con la consulta JMESPath allí.</span><span class="sxs-lookup"><span data-stu-id="d8ab6-129">You can also pipe the command output to [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) and experiment with your JMESPath query there.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```

