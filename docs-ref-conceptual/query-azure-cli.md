---
title: Resultados del comando de consulta con la CLI de Azure 2.0
description: "Obtenga información acerca de cómo realizar consultas JMESPath con la salida de los comandos de la CLI de Azure 2.0."
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 98bc35c1e8136231011a2303901f42c68c9a7758
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="44dfc-103">Uso de consultas JMESPath con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="44dfc-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="44dfc-104">La CLI de Azure 2.0 utiliza el parámetro `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados del comando `az`.</span><span class="sxs-lookup"><span data-stu-id="44dfc-104">The Azure CLI 2.0 uses the `--query` parameter to execute a [JMESPath query](http://jmespath.org) on the results of your `az` command.</span></span> <span data-ttu-id="44dfc-105">JMESPath es un potente lenguaje de consulta para salidas JSON.</span><span class="sxs-lookup"><span data-stu-id="44dfc-105">JMESPath is a powerful query language for JSON outputs.</span></span>  <span data-ttu-id="44dfc-106">Si no está familiarizado con las consultas JMESPath encontrará un tutorial en [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span><span class="sxs-lookup"><span data-stu-id="44dfc-106">If you are unfamiliar with JMESPath queries you can find a tutorial at [JMESPath.org/tutorial](http://JMESPath.org/tutorial.html).</span></span>

<span data-ttu-id="44dfc-107">El parámetro `Query` es compatible con todos los tipos de recurso (Container Services, Web Apps, VM, etc.) de la CLI de Azure 2.0 y puede usarse para varios propósitos diferentes.</span><span class="sxs-lookup"><span data-stu-id="44dfc-107">`Query` parameter is supported by every resource type (Container Services, Web Apps, VM, etc.) within Azure CLI 2.0 and can be used for various different purposes.</span></span>  <span data-ttu-id="44dfc-108">Se muestran varios ejemplos a continuación.</span><span class="sxs-lookup"><span data-stu-id="44dfc-108">We have listed several examples below.</span></span>

## <a name="select-simple-properties"></a><span data-ttu-id="44dfc-109">Selección de propiedades simples</span><span class="sxs-lookup"><span data-stu-id="44dfc-109">Select simple properties</span></span>

<span data-ttu-id="44dfc-110">El sencillo comando `list` con el formato de salida `table` devuelve un conjunto protegido con las propiedades más comunes y sencillas de cada tipo de recurso en un formato tabular fácil de leer.</span><span class="sxs-lookup"><span data-stu-id="44dfc-110">The simple `list` command with `table` output format returns a curated set of most common, simple properties for each resource type in an easy-to-read tabular format.</span></span>

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

<span data-ttu-id="44dfc-111">Puede usar el parámetro `--query` para que muestre únicamente el nombre del grupo de recursos y el de la máquina virtual para todas las máquinas virtuales de su suscripción.</span><span class="sxs-lookup"><span data-stu-id="44dfc-111">You can use the `--query` parameter to show just the Resource Group name and VM name for all virtual machines in your subscription.</span></span>

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

<span data-ttu-id="44dfc-112">En el ejemplo anterior, observe que los encabezados de columna son "Columna1" y "Columna2".</span><span class="sxs-lookup"><span data-stu-id="44dfc-112">In the previous example, you notice that the column headings are "Column1" and "Column2".</span></span>  <span data-ttu-id="44dfc-113">Puede también agregar etiquetas o nombres descriptivos a las propiedades que seleccione.</span><span class="sxs-lookup"><span data-stu-id="44dfc-113">You can add friendly labels or names to the properties you select, as well.</span></span>  <span data-ttu-id="44dfc-114">En el ejemplo siguiente, se agregaron las etiquetas "VMName" y "RGName" a las propiedades seleccionadas "name" y "resourceGroup".</span><span class="sxs-lookup"><span data-stu-id="44dfc-114">In the following example, we added the labels "VMName" and "RGName" to the selected properties "name" and "resourceGroup".</span></span>


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

## <a name="select-complex-nested-properties"></a><span data-ttu-id="44dfc-115">Selección de propiedades complejas anidadas</span><span class="sxs-lookup"><span data-stu-id="44dfc-115">Select complex nested properties</span></span>

<span data-ttu-id="44dfc-116">Si la propiedad que desea seleccionar está muy anidada en la salida JSON, debe proporcionar la ruta de acceso completa a la propiedad anidada.</span><span class="sxs-lookup"><span data-stu-id="44dfc-116">If the property you want to select is nested deep in the JSON output you need to supply the full path to that nested property.</span></span> <span data-ttu-id="44dfc-117">En el ejemplo siguiente se muestra cómo seleccionar el nombre de la máquina virtual y el tipo de sistema operativo mediante el comando de lista vm.</span><span class="sxs-lookup"><span data-stu-id="44dfc-117">The following example shows how to select the VMName and the OS type from the vm list command.</span></span>

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

## <a name="filter-with-the-contains-function"></a><span data-ttu-id="44dfc-118">Filtrado con la función Contains</span><span class="sxs-lookup"><span data-stu-id="44dfc-118">Filter with the contains function</span></span>

<span data-ttu-id="44dfc-119">Puede usar la función `contains` de JMESPath para refinar los resultados devueltos en la consulta.</span><span class="sxs-lookup"><span data-stu-id="44dfc-119">You can use the JMESPath `contains` function to refine your results returned in the query.</span></span>
<span data-ttu-id="44dfc-120">En el ejemplo siguiente, el comando selecciona solo las máquinas virtuales con el texto "RGD" en su nombre.</span><span class="sxs-lookup"><span data-stu-id="44dfc-120">In the following example, the command selects only VMs that have the text "RGD" in their name.</span></span>

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

<span data-ttu-id="44dfc-121">En el ejemplo siguiente, los resultados devolverán las máquinas virtuales que tengan el vmSize 'Standard_DS1'.</span><span class="sxs-lookup"><span data-stu-id="44dfc-121">With the next example, the results will return the VMs that have the vmSize 'Standard_DS1'.</span></span>

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

## <a name="filter-with-grep"></a><span data-ttu-id="44dfc-122">Filtrado con grep</span><span class="sxs-lookup"><span data-stu-id="44dfc-122">Filter with grep</span></span>

<span data-ttu-id="44dfc-123">El formato de salida `tsv` es un texto separado por tabulaciones sin encabezados.</span><span class="sxs-lookup"><span data-stu-id="44dfc-123">The `tsv` output format is a tab-separated text with no headers.</span></span> <span data-ttu-id="44dfc-124">Se puede canalizar a comandos como `grep` y `cut` para analizar aún más los valores específicos de la salida `list`.</span><span class="sxs-lookup"><span data-stu-id="44dfc-124">It can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="44dfc-125">En el ejemplo siguiente, el comando `grep` selecciona solo las máquinas virtuales con el texto "RGD" en su nombre.</span><span class="sxs-lookup"><span data-stu-id="44dfc-125">In the following example, the `grep` command selects only VMs that have text "RGD" in their name.</span></span>  <span data-ttu-id="44dfc-126">El comando `cut` selecciona solo el valor del octavo campo (separado por tabulaciones) para mostrarlo en la salida.</span><span class="sxs-lookup"><span data-stu-id="44dfc-126">The `cut` command selects only the 8th field (separated by tabs) value to show in the output.</span></span>

```azurecli-interactive
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="explore-with-jpterm"></a><span data-ttu-id="44dfc-127">Exploración con jpterm</span><span class="sxs-lookup"><span data-stu-id="44dfc-127">Explore with jpterm</span></span>

<span data-ttu-id="44dfc-128">También se puede canalizar la salida del comando a [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) y experimentar con la consulta JMESPath allí.</span><span class="sxs-lookup"><span data-stu-id="44dfc-128">You can also pipe the command output to [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) and experiment with your JMESPath query there.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```

