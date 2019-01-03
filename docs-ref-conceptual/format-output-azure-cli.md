---
title: Formatos de salida para la CLI de Azure
description: Obtenga información acerca de cómo dar formato a la salida de los comandos de la CLI de Azure como tablas, listas o código JSON.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d83dcdda7d7485bc32f0da59163afe7ea906faa6
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593479"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="b93e7-103">Formatos de salida para los comandos de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="b93e7-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="b93e7-104">La CLI de Azure usa JSON como formato de salida predeterminado, pero ofrece otros formatos.</span><span class="sxs-lookup"><span data-stu-id="b93e7-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="b93e7-105">Use el parámetro `--output` (`--out` o `-o`) para dar formato a la salida de la CLI.</span><span class="sxs-lookup"><span data-stu-id="b93e7-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="b93e7-106">Los valores de argumento y los tipos de salida son:</span><span class="sxs-lookup"><span data-stu-id="b93e7-106">The argument values and types of output are:</span></span>

<span data-ttu-id="b93e7-107">--output</span><span class="sxs-lookup"><span data-stu-id="b93e7-107">--output</span></span> | <span data-ttu-id="b93e7-108">DESCRIPCIÓN</span><span class="sxs-lookup"><span data-stu-id="b93e7-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="b93e7-109">Cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="b93e7-109">JSON string.</span></span> <span data-ttu-id="b93e7-110">Esta es la configuración predeterminada.</span><span class="sxs-lookup"><span data-stu-id="b93e7-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="b93e7-111">JSON con colores.</span><span class="sxs-lookup"><span data-stu-id="b93e7-111">Colorized JSON.</span></span>
`yaml`   | <span data-ttu-id="b93e7-112">YAML, una alternativa a JSON legible por máquina.</span><span class="sxs-lookup"><span data-stu-id="b93e7-112">YAML, a machine-readable alternative to JSON.</span></span>
`table`  | <span data-ttu-id="b93e7-113">Tabla ASCII con claves como encabezados de columna.</span><span class="sxs-lookup"><span data-stu-id="b93e7-113">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="b93e7-114">Valores separados por tabulaciones, sin claves</span><span class="sxs-lookup"><span data-stu-id="b93e7-114">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="b93e7-115">Formato de salida JSON</span><span class="sxs-lookup"><span data-stu-id="b93e7-115">JSON output format</span></span>

<span data-ttu-id="b93e7-116">En el ejemplo siguiente se muestra la lista de máquinas virtuales de sus suscripciones en el formato json predeterminado.</span><span class="sxs-lookup"><span data-stu-id="b93e7-116">The following example displays the list of virtual machines in your subscriptions in the default json format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="b93e7-117">La salida siguiente tiene algunos campos que se omiten para mayor brevedad y se ha reemplazado la información de identificación.</span><span class="sxs-lookup"><span data-stu-id="b93e7-117">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="b93e7-118">Formato de salida YAML</span><span class="sxs-lookup"><span data-stu-id="b93e7-118">YAML output format</span></span>

<span data-ttu-id="b93e7-119">El formato `yaml` imprime la salida como [YAML](http://yaml.org/), un formato de serialización de datos de texto sin formato.</span><span class="sxs-lookup"><span data-stu-id="b93e7-119">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="b93e7-120">YAML suele ser más fácil de leer que JSON y se corresponde fácilmente con ese formato.</span><span class="sxs-lookup"><span data-stu-id="b93e7-120">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="b93e7-121">Algunas aplicaciones y los comandos de la CLI aceptan YAML como entrada de configuración, en lugar de JSON.</span><span class="sxs-lookup"><span data-stu-id="b93e7-121">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="b93e7-122">La salida siguiente tiene algunos campos que se omiten para mayor brevedad y se ha reemplazado la información de identificación.</span><span class="sxs-lookup"><span data-stu-id="b93e7-122">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

```yaml
- availabilitySet: null
  diagnosticsProfile: null
  hardwareProfile:
    vmSize: Standard_DS1_v2
  id: /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010
  identity: null
  instanceView: null
  licenseType: null
  location: westus
  name: ExampleVM1
  networkProfile:
    networkInterfaces:
    - id: /subscriptions/.../resourceGroups/DemoRG1/providers/Microsoft.Network/networkInterfaces/DemoVM010Nic
      primary: null
      resourceGroup: DemoRG1
  ...
...
```

## <a name="table-output-format"></a><span data-ttu-id="b93e7-123">Formato de salida de tabla</span><span class="sxs-lookup"><span data-stu-id="b93e7-123">Table output format</span></span>

<span data-ttu-id="b93e7-124">El formato `table` imprime la salida como una tabla ASCII, lo que facilita la lectura y la búsqueda.</span><span class="sxs-lookup"><span data-stu-id="b93e7-124">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="b93e7-125">Los objetos anidados no se incluyen en la tabla de salida, pero se pueden filtrar como parte de una consulta.</span><span class="sxs-lookup"><span data-stu-id="b93e7-125">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="b93e7-126">Algunos campos no se incluyen en la tabla, por lo que este formato es adecuado cuando se desea una revisión rápida de los datos con posibilidad de que el usuario realice búsquedas.</span><span class="sxs-lookup"><span data-stu-id="b93e7-126">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="b93e7-127">Puede usar el parámetro `--query` para personalizar las propiedades y las columnas que desea mostrar en la salida de la lista.</span><span class="sxs-lookup"><span data-stu-id="b93e7-127">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="b93e7-128">En el ejemplo siguiente se muestra cómo seleccionar el nombre de máquina virtual y el nombre del grupo de recursos en el comando `list`.</span><span class="sxs-lookup"><span data-stu-id="b93e7-128">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

```azurecli-interactive
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
> <span data-ttu-id="b93e7-129">Algunas claves no se imprimen en la vista de tabla de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="b93e7-129">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="b93e7-130">Se trata de `id`, `type` y `etag`.</span><span class="sxs-lookup"><span data-stu-id="b93e7-130">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="b93e7-131">Si necesita ver estos datos en la salida, puede usar la característica de reentrada de claves de JMESPath para cambiar el nombre de la clave y evitar el filtrado.</span><span class="sxs-lookup"><span data-stu-id="b93e7-131">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="b93e7-132">Para más información sobre el uso de consultas para filtrar los datos, consulte [Uso de consultas JMESPath con la CLI de Azure](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="b93e7-132">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="b93e7-133">Formato de salida TSV</span><span class="sxs-lookup"><span data-stu-id="b93e7-133">TSV output format</span></span>

<span data-ttu-id="b93e7-134">El formato de salida `tsv` devuelve valores separados por tabulaciones y nueva línea sin formato adicional, claves ni otros símbolos.</span><span class="sxs-lookup"><span data-stu-id="b93e7-134">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="b93e7-135">Este formato facilita el consumo de la salida en otros comandos y herramientas que necesitan procesar el texto de alguna forma.</span><span class="sxs-lookup"><span data-stu-id="b93e7-135">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="b93e7-136">Al igual que el formato `table`, `tsv` no imprime objetos anidados.</span><span class="sxs-lookup"><span data-stu-id="b93e7-136">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="b93e7-137">Mediante el ejemplo anterior con la opción `tsv` se genera un resultado separado por tabulaciones.</span><span class="sxs-lookup"><span data-stu-id="b93e7-137">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="b93e7-138">El ejemplo siguiente muestra cómo se puede canalizar la salida `tsv` a otros comandos en Bash.</span><span class="sxs-lookup"><span data-stu-id="b93e7-138">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="b93e7-139">`grep` selecciona los elementos que tienen el texto "RGD" y el comando `cut` selecciona el octavo campo para mostrar el nombre de la máquina virtual en la salida.</span><span class="sxs-lookup"><span data-stu-id="b93e7-139">`grep` selects items that have text "RGD" in them, then the `cut` command selects the eighth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

<span data-ttu-id="b93e7-140">Para fines de procesamiento de campos separados por tabulaciones, los valores están en el mismo orden que aparecen en el objeto JSON impreso.</span><span class="sxs-lookup"><span data-stu-id="b93e7-140">For the purposes of processing tab-separated fields, the values are in the same order that they appear in the printed JSON object.</span></span> <span data-ttu-id="b93e7-141">Se garantiza que este orden sea coherente entre las distintas ejecuciones del comando.</span><span class="sxs-lookup"><span data-stu-id="b93e7-141">This order is guaranteed to be consistent between runs of the command.</span></span>

## <a name="set-the-default-output-format"></a><span data-ttu-id="b93e7-142">Establecimiento del formato de salida predeterminado</span><span class="sxs-lookup"><span data-stu-id="b93e7-142">Set the default output format</span></span>

<span data-ttu-id="b93e7-143">Puede usar el comando interactivo `az configure` para configurar el entorno y establecer la configuración predeterminada de los formatos de salida.</span><span class="sxs-lookup"><span data-stu-id="b93e7-143">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="b93e7-144">El formato de salida predeterminado es `json`.</span><span class="sxs-lookup"><span data-stu-id="b93e7-144">The default output format is `json`.</span></span>

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

<span data-ttu-id="b93e7-145">Para más información sobre cómo configurar el entorno, consulte [Configuración de la CLI de Azure](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="b93e7-145">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>
