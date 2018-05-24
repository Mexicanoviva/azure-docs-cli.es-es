---
title: Formatos de salida para la CLI de Azure 2.0
description: Obtenga información acerca de cómo dar formato a la salida de los comandos de la CLI de Azure 2.0 como tablas, listas o código JSON.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/16/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 016465080e95af3ab0650146e955dd8cffc569e8
ms.sourcegitcommit: 8b4629a42ceecf30c1efbc6fdddf512f4dddfab0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/18/2018
---
# <a name="output-formats-for-azure-cli-20-commands"></a><span data-ttu-id="f73f9-103">Formatos de salida de los comandos de la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="f73f9-103">Output formats for Azure CLI 2.0 commands</span></span>

<span data-ttu-id="f73f9-104">La CLI de Azure 2.0 usa json como su opción de salida predeterminada, pero ofrece varias formas de dar formato a la salida de cualquier comando.</span><span class="sxs-lookup"><span data-stu-id="f73f9-104">Azure CLI 2.0 uses json as its default output option, but offers various ways for you to format the output of any command.</span></span>  <span data-ttu-id="f73f9-105">Use el parámetro `--output` (o `--out` o `-o`) para dar formato a la salida del comando con uno de los tipos de salida que se indican en la tabla siguiente:</span><span class="sxs-lookup"><span data-stu-id="f73f9-105">Use the `--output` (or `--out` or `-o`) parameter to format the output of the command into one of the output types noted in the following table:</span></span>

<span data-ttu-id="f73f9-106">--output</span><span class="sxs-lookup"><span data-stu-id="f73f9-106">--output</span></span> | <span data-ttu-id="f73f9-107">DESCRIPCIÓN</span><span class="sxs-lookup"><span data-stu-id="f73f9-107">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="f73f9-108">Cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="f73f9-108">JSON string.</span></span> <span data-ttu-id="f73f9-109">Esta es la configuración predeterminada.</span><span class="sxs-lookup"><span data-stu-id="f73f9-109">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="f73f9-110">JSON con colores.</span><span class="sxs-lookup"><span data-stu-id="f73f9-110">Colorized JSON.</span></span>
`table`  | <span data-ttu-id="f73f9-111">Tabla ASCII con claves como encabezados de columna.</span><span class="sxs-lookup"><span data-stu-id="f73f9-111">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="f73f9-112">Valores separados por tabulaciones, sin claves</span><span class="sxs-lookup"><span data-stu-id="f73f9-112">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="f73f9-113">Formato de salida JSON</span><span class="sxs-lookup"><span data-stu-id="f73f9-113">JSON output format</span></span>

<span data-ttu-id="f73f9-114">En el ejemplo siguiente se muestra la lista de máquinas virtuales de sus suscripciones en el formato json predeterminado.</span><span class="sxs-lookup"><span data-stu-id="f73f9-114">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="f73f9-115">La salida siguiente tiene algunos campos que se omiten para mayor brevedad y se ha reemplazado la información de identificación.</span><span class="sxs-lookup"><span data-stu-id="f73f9-115">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/.../resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
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

## <a name="table-output-format"></a><span data-ttu-id="f73f9-116">Formato de salida de tabla</span><span class="sxs-lookup"><span data-stu-id="f73f9-116">Table output format</span></span>

<span data-ttu-id="f73f9-117">El formato de salida `table` proporciona una salida con formato de filas y columnas de datos intercalados, lo que facilita la lectura y la búsqueda.</span><span class="sxs-lookup"><span data-stu-id="f73f9-117">The `table` output format provides plain output formatted as rows and columns of collated data, making it easy to read and scan.</span></span> <span data-ttu-id="f73f9-118">Los objetos anidados no se incluyen en la salida de tabla, pero se pueden filtrar como parte de una consulta.</span><span class="sxs-lookup"><span data-stu-id="f73f9-118">Nested objects are not included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="f73f9-119">Algunos campos también se omiten en la tabla de datos, por lo que este formato es adecuado cuando se desea una revisión rápida de los datos con posibilidad de que el usuario realice búsquedas.</span><span class="sxs-lookup"><span data-stu-id="f73f9-119">Some fields are also omitted from the table data, so this format is best when you want a quick, human-searchable overview of data.</span></span>

```azurecli-interactive
az vm list --out table
```

```output
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

<span data-ttu-id="f73f9-120">Puede usar el parámetro `--query` para personalizar las propiedades y las columnas que desea mostrar en la salida de la lista.</span><span class="sxs-lookup"><span data-stu-id="f73f9-120">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="f73f9-121">En el ejemplo siguiente se muestra cómo seleccionar el nombre de máquina virtual y el nombre del grupo de recursos en el comando `list`.</span><span class="sxs-lookup"><span data-stu-id="f73f9-121">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli
az vm list --query "[].{resource:resourceGroup, name:name}" -o table
```

```output
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

> [!NOTE]
> <span data-ttu-id="f73f9-122">Determinadas claves se filtran y no se imprimen en la vista de tabla.</span><span class="sxs-lookup"><span data-stu-id="f73f9-122">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="f73f9-123">Se trata de `id`, `type` y `etag`.</span><span class="sxs-lookup"><span data-stu-id="f73f9-123">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="f73f9-124">Si necesita ver estos datos en la salida, puede usar la característica de reentrada de claves de JMESPath para cambiar el nombre de la clave y evitar el filtrado.</span><span class="sxs-lookup"><span data-stu-id="f73f9-124">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="f73f9-125">Para más información sobre el uso de consultas para filtrar los datos, consulte [Uso de consultas JMESPath con la CLI de Azure 2.0](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="f73f9-125">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI 2.0](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="f73f9-126">Formato de salida TSV</span><span class="sxs-lookup"><span data-stu-id="f73f9-126">TSV output format</span></span>

<span data-ttu-id="f73f9-127">El formato de salida `tsv` devuelve valores separados por tabulaciones y nueva línea sin formato adicional, claves ni otros símbolos.</span><span class="sxs-lookup"><span data-stu-id="f73f9-127">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="f73f9-128">Este formato facilita el consumo de la salida en otros comandos y herramientas que necesitan procesar el texto de alguna forma.</span><span class="sxs-lookup"><span data-stu-id="f73f9-128">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="f73f9-129">Al igual que el formato `table`, la opción de salida `tsv` no imprime objetos anidados.</span><span class="sxs-lookup"><span data-stu-id="f73f9-129">Like the `table` format, the `tsv` output option does not print nested objects.</span></span>

<span data-ttu-id="f73f9-130">Mediante el ejemplo anterior con la opción `tsv` se genera un resultado separado por tabulaciones.</span><span class="sxs-lookup"><span data-stu-id="f73f9-130">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010 None    None    westus  DemoVM010           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212 None    None    westus  demovm212           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213 None    None    westus  demovm213           None    Succeeded   DEMORG1 None            Microsoft.Compute/virtualMachines   2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM None    None    westus  KBDemo001VM         None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines   14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus  KBDemo020           None    Succeeded   RGDEMO001   None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="f73f9-131">En el siguiente ejemplo se muestra cómo se puede canalizar la salida `tsv` a otros comandos en sistemas UNIX para extraer datos más específicos.</span><span class="sxs-lookup"><span data-stu-id="f73f9-131">The next example shows how the `tsv` output can be piped to other commands on UNIX systems to extract more specific data.</span></span> <span data-ttu-id="f73f9-132">El comando `grep` selecciona los elementos que tienen el texto "RGD" y el comando `cut` selecciona el octavo campo (separado por tabulaciones) para mostrar el nombre de la máquina virtual en la salida.</span><span class="sxs-lookup"><span data-stu-id="f73f9-132">The `grep` command selects items that have text "RGD" in them, and then the `cut` command selects the eighth field (separated by tabs) to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="f73f9-133">Para fines de procesamiento de campos separados por tabulaciones, los valores están en el mismo orden que aparecen en el objeto JSON impreso.</span><span class="sxs-lookup"><span data-stu-id="f73f9-133">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="f73f9-134">Se garantiza que este orden sea coherente entre las distintas ejecuciones del comando.</span><span class="sxs-lookup"><span data-stu-id="f73f9-134">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="f73f9-135">Establecimiento del formato de salida predeterminado</span><span class="sxs-lookup"><span data-stu-id="f73f9-135">Set the default output format</span></span>

<span data-ttu-id="f73f9-136">Puede usar el comando interactivo `az configure` para configurar el entorno y establecer la configuración predeterminada de los formatos de salida.</span><span class="sxs-lookup"><span data-stu-id="f73f9-136">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="f73f9-137">El formato de salida predeterminado es `json`.</span><span class="sxs-lookup"><span data-stu-id="f73f9-137">The default output format is `json`.</span></span> 

```azurecli-interactive
az configure
```

```output
Welcome to the Azure CLI! This command will guide you through logging in and setting some default values.

Your settings can be found at /home/defaultuser/.azure/config
Your current configuration is as follows:

  ...

Do you wish to change your settings? (y/N): y

What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab- and Newline-delimited, great for GREP, AWK, etc.
Please enter a choice [1]:
```

<span data-ttu-id="f73f9-138">Para más información sobre cómo configurar el entorno, consulte [Configuración de la CLI de Azure 2.0](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="f73f9-138">To learn more about configuring your environment, see [Azure CLI 2.0 configuration](/cli/azure/azure-cli-configuration).</span></span>