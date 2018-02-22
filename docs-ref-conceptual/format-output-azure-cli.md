---
title: Formatos de salida para la CLI de Azure 2.0
description: "Obtenga información acerca de cómo dar formato a la salida de los comandos de la CLI de Azure 2.0 como tablas, listas o código JSON."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: a5d629675b468421e3abee41b9c8bffd7e96e5b0
ms.sourcegitcommit: b93a19222e116d5880bbe64c03507c64e190331e
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/15/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="d63f8-103">Formatos de salida de los comandos de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="d63f8-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="d63f8-104">La CLI de Azure 2.0 usa json como su opción de salida predeterminada, pero ofrece varias formas de dar formato a la salida de cualquier comando.</span><span class="sxs-lookup"><span data-stu-id="d63f8-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="d63f8-105">Use el parámetro `--output` (o `--out` o `-o`) para dar formato a la salida del comando con uno de los tipos de salida que se indican en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="d63f8-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table.</span></span>

<span data-ttu-id="d63f8-106">--output</span><span class="sxs-lookup"><span data-stu-id="d63f8-106">--output</span></span> | <span data-ttu-id="d63f8-107">DESCRIPCIÓN</span><span class="sxs-lookup"><span data-stu-id="d63f8-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="d63f8-108">Cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="d63f8-108">json string.</span></span> <span data-ttu-id="d63f8-109">`json` es el valor predeterminado.</span><span class="sxs-lookup"><span data-stu-id="d63f8-109">`json` is the default.</span></span>
`jsonc`  | <span data-ttu-id="d63f8-110">Cadena json con colores.</span><span class="sxs-lookup"><span data-stu-id="d63f8-110">colorized json string.</span></span>
`table`  | <span data-ttu-id="d63f8-111">Tabla con encabezados de columna.</span><span class="sxs-lookup"><span data-stu-id="d63f8-111">table with column headings.</span></span>
`tsv`    | <span data-ttu-id="d63f8-112">Valores separados por tabulaciones.</span><span class="sxs-lookup"><span data-stu-id="d63f8-112">tab-separated values.</span></span>

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a><span data-ttu-id="d63f8-113">Uso de la opción json</span><span class="sxs-lookup"><span data-stu-id="d63f8-113">Using the json option</span></span>

<span data-ttu-id="d63f8-114">En el ejemplo siguiente se muestra la lista de máquinas virtuales de sus suscripciones en el formato json predeterminado.</span><span class="sxs-lookup"><span data-stu-id="d63f8-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="d63f8-115">Los resultados están en este formulario (solo se muestran resultados parciales por motivos de brevedad).</span><span class="sxs-lookup"><span data-stu-id="d63f8-115">The results are in this form (only showing partial output for sake of brevity).</span></span>

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
          "primary": null,
          "resourceGroup": "demorg1"
        }
      ]
    },
          ...
          ...
          ...
]
```

## <a name="using-the-table-option"></a><span data-ttu-id="d63f8-116">Uso de la opción de tabla</span><span class="sxs-lookup"><span data-stu-id="d63f8-116">Using the table option</span></span>

<span data-ttu-id="d63f8-117">La opción de tabla proporciona una forma sencilla de leer un conjunto de salidas, pero tenga en cuenta que los objetos anidados no se incluyen en la salida con el sencillo comando `--output table`, a diferencia del anterior ejemplo .json.</span><span class="sxs-lookup"><span data-stu-id="d63f8-117">The table option provides an easy to read set of output, but note that nested objects are not included in the output with the simple `--output table`, unlike the preceding .json example.</span></span>  <span data-ttu-id="d63f8-118">El uso del mismo ejemplo con formato de salida 'table' proporciona una lista protegida de los valores de propiedad más comunes.</span><span class="sxs-lookup"><span data-stu-id="d63f8-118">Using the same example with 'table' output format provides a curated list of most common property values.</span></span>

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

<span data-ttu-id="d63f8-119">Puede usar el parámetro `--query` para personalizar las propiedades y las columnas que desea mostrar en la salida de la lista.</span><span class="sxs-lookup"><span data-stu-id="d63f8-119">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="d63f8-120">En el ejemplo siguiente se muestra cómo seleccionar el nombre de máquina virtual y el nombre del grupo de recursos en el comando `list`.</span><span class="sxs-lookup"><span data-stu-id="d63f8-120">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
az vm list --query "[].{ resource: resourceGroup, name: name }" -o table
```

```
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

## <a name="using-the-tsv-option"></a><span data-ttu-id="d63f8-121">Uso de la opción tsv</span><span class="sxs-lookup"><span data-stu-id="d63f8-121">Using the tsv option</span></span>

<span data-ttu-id="d63f8-122">El formato de salida "tsv" devuelve una salida sencilla basada en texto y separada por tabulaciones sin encabezados ni guiones.</span><span class="sxs-lookup"><span data-stu-id="d63f8-122">'tsv' output format returns a simple text-based and tab-separated output with no headings and dashes.</span></span> <span data-ttu-id="d63f8-123">Este formato facilita el consumo de la salida en otros comandos y herramientas que necesitan procesar el texto de alguna forma.</span><span class="sxs-lookup"><span data-stu-id="d63f8-123">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="d63f8-124">Mediante el ejemplo anterior con la opción `tsv` se genera un resultado separado por tabulaciones.</span><span class="sxs-lookup"><span data-stu-id="d63f8-124">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None   None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="d63f8-125">En el siguiente ejemplo se muestra cómo la salida `tsv` se puede canalizar a comandos como `grep` y `cut` para analizar aún más los valores específicos de la salida `list`.</span><span class="sxs-lookup"><span data-stu-id="d63f8-125">The next example shows how the `tsv` output can be piped to commands like `grep` and `cut` to further parse specific values out of the `list` output.</span></span> <span data-ttu-id="d63f8-126">El comando `grep` solo selecciona los elementos que tienen el texto "RGD" en ellos y el comando `cut` selecciona solo el valor del octavo campo (separado por tabulaciones) para mostrar en la salida.</span><span class="sxs-lookup"><span data-stu-id="d63f8-126">The `grep` command selects only items that have text "RGD" in them and then the `cut` command selects only the eighth field (separated by tabs) value to show in the output.</span></span>

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a><span data-ttu-id="d63f8-127">Establecimiento del formato de salida predeterminado</span><span class="sxs-lookup"><span data-stu-id="d63f8-127">Setting the default output format</span></span>

<span data-ttu-id="d63f8-128">Puede usar el comando `az configure` para configurar el entorno o establecer preferencias como la configuración predeterminada de los formatos de salida.</span><span class="sxs-lookup"><span data-stu-id="d63f8-128">You can use the `az configure` command to set up your environment or establish preferences such as default settings for output formats.</span></span> <span data-ttu-id="d63f8-129">Para un uso común, el valor predeterminado del formato de salida más fácil es el formato "table". Seleccione **3** cuando se le soliciten las opciones de formato de salida.</span><span class="sxs-lookup"><span data-stu-id="d63f8-129">For common use, the easiest output format default is the "table" format - select **3** when prompted for output format choices.</span></span>

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]:
```
