---
title: Formatos de salida para la CLI de Azure
description: Obtenga información acerca de cómo dar formato a la salida de los comandos de la CLI de Azure como tablas, listas o código JSON.
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 09/23/2019
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 7bc31ba89234dbdb7b939f3a09886f31184ac65f
ms.sourcegitcommit: 18973ac471bbd12af2c8f8fa32a233b0abe5b020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2020
ms.locfileid: "75913550"
---
# <a name="output-formats-for-azure-cli-commands"></a><span data-ttu-id="ba13a-103">Formatos de salida para los comandos de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="ba13a-103">Output formats for Azure CLI commands</span></span>

<span data-ttu-id="ba13a-104">La CLI de Azure usa JSON como formato de salida predeterminado, pero ofrece otros formatos.</span><span class="sxs-lookup"><span data-stu-id="ba13a-104">The Azure CLI uses JSON as its default output format, but offers other formats.</span></span>  <span data-ttu-id="ba13a-105">Use el parámetro `--output` (`--out` o `-o`) para dar formato a la salida de la CLI.</span><span class="sxs-lookup"><span data-stu-id="ba13a-105">Use the `--output` (`--out` or `-o`) parameter to format CLI output.</span></span> <span data-ttu-id="ba13a-106">Los valores de argumento y los tipos de salida son:</span><span class="sxs-lookup"><span data-stu-id="ba13a-106">The argument values and types of output are:</span></span>

<span data-ttu-id="ba13a-107">--output</span><span class="sxs-lookup"><span data-stu-id="ba13a-107">--output</span></span> | <span data-ttu-id="ba13a-108">Descripción</span><span class="sxs-lookup"><span data-stu-id="ba13a-108">Description</span></span>
---------|-------------------------------
`json`   | <span data-ttu-id="ba13a-109">Cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="ba13a-109">JSON string.</span></span> <span data-ttu-id="ba13a-110">Esta es la configuración predeterminada.</span><span class="sxs-lookup"><span data-stu-id="ba13a-110">This setting is the default.</span></span>
`jsonc`  | <span data-ttu-id="ba13a-111">JSON con colores.</span><span class="sxs-lookup"><span data-stu-id="ba13a-111">Colorized JSON.</span></span>
`yaml`   | <span data-ttu-id="ba13a-112">YAML, una alternativa a JSON legible por máquina.</span><span class="sxs-lookup"><span data-stu-id="ba13a-112">YAML, a machine-readable alternative to JSON.</span></span>
`table`  | <span data-ttu-id="ba13a-113">Tabla ASCII con claves como encabezados de columna.</span><span class="sxs-lookup"><span data-stu-id="ba13a-113">ASCII table with keys as column headings.</span></span>
`tsv`    | <span data-ttu-id="ba13a-114">Valores separados por tabulaciones, sin claves</span><span class="sxs-lookup"><span data-stu-id="ba13a-114">Tab-separated values, with no keys</span></span>

## <a name="json-output-format"></a><span data-ttu-id="ba13a-115">Formato de salida JSON</span><span class="sxs-lookup"><span data-stu-id="ba13a-115">JSON output format</span></span>

<span data-ttu-id="ba13a-116">En el ejemplo siguiente se muestra la lista de máquinas virtuales de sus suscripciones en el formato JSON predeterminado.</span><span class="sxs-lookup"><span data-stu-id="ba13a-116">The following example displays the list of virtual machines in your subscriptions in the default JSON format.</span></span>

```azurecli-interactive
az vm list --output json
```

<span data-ttu-id="ba13a-117">La salida siguiente tiene algunos campos que se omiten para mayor brevedad y se ha reemplazado la información de identificación.</span><span class="sxs-lookup"><span data-stu-id="ba13a-117">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="yaml-output-format"></a><span data-ttu-id="ba13a-118">Formato de salida YAML</span><span class="sxs-lookup"><span data-stu-id="ba13a-118">YAML output format</span></span>

<span data-ttu-id="ba13a-119">El formato `yaml` imprime la salida como [YAML](http://yaml.org/), un formato de serialización de datos de texto sin formato.</span><span class="sxs-lookup"><span data-stu-id="ba13a-119">The `yaml` format prints output as [YAML](http://yaml.org/), a plain-text data serialization format.</span></span> <span data-ttu-id="ba13a-120">YAML suele ser más fácil de leer que JSON y se corresponde fácilmente con ese formato.</span><span class="sxs-lookup"><span data-stu-id="ba13a-120">YAML tends to be easier to read than JSON, and easily maps to that format.</span></span> <span data-ttu-id="ba13a-121">Algunas aplicaciones y los comandos de la CLI aceptan YAML como entrada de configuración, en lugar de JSON.</span><span class="sxs-lookup"><span data-stu-id="ba13a-121">Some applications and CLI commands take YAML as configuration input, instead of JSON.</span></span>

```azurecli-interactive
az vm list --out yaml
```

<span data-ttu-id="ba13a-122">La salida siguiente tiene algunos campos que se omiten para mayor brevedad y se ha reemplazado la información de identificación.</span><span class="sxs-lookup"><span data-stu-id="ba13a-122">The following output has some fields omitted for brevity, and identifying information replaced.</span></span>

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

## <a name="table-output-format"></a><span data-ttu-id="ba13a-123">Formato de salida de tabla</span><span class="sxs-lookup"><span data-stu-id="ba13a-123">Table output format</span></span>

<span data-ttu-id="ba13a-124">El formato `table` imprime la salida como una tabla ASCII, lo que facilita la lectura y la búsqueda.</span><span class="sxs-lookup"><span data-stu-id="ba13a-124">The `table` format prints output as an ASCII table, making it easy to read and scan.</span></span> <span data-ttu-id="ba13a-125">Los objetos anidados no se incluyen en la tabla de salida, pero se pueden filtrar como parte de una consulta.</span><span class="sxs-lookup"><span data-stu-id="ba13a-125">Nested objects aren't included in table output, but can still be filtered as part of a query.</span></span> <span data-ttu-id="ba13a-126">Algunos campos no se incluyen en la tabla, por lo que este formato es adecuado cuando se desea una revisión rápida de los datos con posibilidad de que el usuario realice búsquedas.</span><span class="sxs-lookup"><span data-stu-id="ba13a-126">Some fields aren't included in the table, so this format is best when you want a quick, human-searchable overview of data.</span></span>

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

<span data-ttu-id="ba13a-127">Puede usar el parámetro `--query` para personalizar las propiedades y las columnas que desea mostrar en la salida de la lista.</span><span class="sxs-lookup"><span data-stu-id="ba13a-127">You can use the `--query` parameter to customize the properties and columns you want to show in the list output.</span></span> <span data-ttu-id="ba13a-128">En el ejemplo siguiente se muestra cómo seleccionar el nombre de máquina virtual y el nombre del grupo de recursos en el comando `list`.</span><span class="sxs-lookup"><span data-stu-id="ba13a-128">The following example shows how to select just the VM Name and the Resource Group Name in the `list` command.</span></span>

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
> <span data-ttu-id="ba13a-129">Algunas claves no se imprimen en la vista de tabla de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="ba13a-129">Some keys are not printed in the table view by default.</span></span> <span data-ttu-id="ba13a-130">Se trata de `id`, `type` y `etag`.</span><span class="sxs-lookup"><span data-stu-id="ba13a-130">These are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="ba13a-131">Si necesita ver estos datos en la salida, puede usar la característica de reentrada de claves de JMESPath para cambiar el nombre de la clave y evitar el filtrado.</span><span class="sxs-lookup"><span data-stu-id="ba13a-131">If you need to see these in your output, you can use the JMESPath re-keying feature to change the key name and avoid filtering.</span></span>
>
> ```azurecli-interactive
> az vm list --query "[].{objectID:id}" -o table
> ```

<span data-ttu-id="ba13a-132">Para más información sobre el uso de consultas para filtrar los datos, consulte [Uso de consultas JMESPath con la CLI de Azure](/cli/azure/query-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="ba13a-132">For more about using queries to filter data, see [Use JMESPath queries with Azure CLI](/cli/azure/query-azure-cli).</span></span>

## <a name="tsv-output-format"></a><span data-ttu-id="ba13a-133">Formato de salida TSV</span><span class="sxs-lookup"><span data-stu-id="ba13a-133">TSV output format</span></span>

<span data-ttu-id="ba13a-134">El formato de salida `tsv` devuelve valores separados por tabulaciones y nueva línea sin formato adicional, claves ni otros símbolos.</span><span class="sxs-lookup"><span data-stu-id="ba13a-134">The `tsv` output format returns tab- and newline-separated values without additional formatting, keys, or other symbols.</span></span> <span data-ttu-id="ba13a-135">Este formato facilita el consumo de la salida en otros comandos y herramientas que necesitan procesar el texto de alguna forma.</span><span class="sxs-lookup"><span data-stu-id="ba13a-135">This format makes it easy to consume the output into other commands and tools that need to process the text in some form.</span></span> <span data-ttu-id="ba13a-136">Al igual que el formato `table`, `tsv` no imprime objetos anidados.</span><span class="sxs-lookup"><span data-stu-id="ba13a-136">Like the `table` format, `tsv` doesn't print nested objects.</span></span>

<span data-ttu-id="ba13a-137">Mediante el ejemplo anterior con la opción `tsv` se genera un resultado separado por tabulaciones.</span><span class="sxs-lookup"><span data-stu-id="ba13a-137">Using the preceding example with the `tsv` option outputs the tab-separated result.</span></span>

```azurecli-interactive
az vm list --out tsv
```

```output
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020   None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    36baa9-9b80-48a8-b4a9-854c7a858ece
```

<span data-ttu-id="ba13a-138">Una restricción del formato de salida TSV es que no hay ninguna garantía del orden de salida.</span><span class="sxs-lookup"><span data-stu-id="ba13a-138">One restriction of the TSV output format is that there isn't a guarantee on output ordering.</span></span> <span data-ttu-id="ba13a-139">La CLI hace lo que puede para conservar el orden; para ello, ordena alfabéticamente las claves en la respuesta JSON y, a continuación, imprime sus valores en orden para la salida de TSV.</span><span class="sxs-lookup"><span data-stu-id="ba13a-139">The CLI makes a best effort to preserve ordering by sorting keys in the response JSON alphebetically, and then printing their values in order for TSV output.</span></span> <span data-ttu-id="ba13a-140">Sin embargo, esto no garantiza que el orden sea siempre idéntico, ya que el formato de respuesta de servicio de Azure puede cambiar.</span><span class="sxs-lookup"><span data-stu-id="ba13a-140">This isn't a guarantee that the order is always identical though, since the Azure service response format may change.</span></span>

<span data-ttu-id="ba13a-141">Para aplicar un orden coherente, deberá usar el parámetro `--query` y el formato de lista [de selección múltiple](query-azure-cli.md#get-multiple-values).</span><span class="sxs-lookup"><span data-stu-id="ba13a-141">In order to enforce consistent ordering, you'll need to use the `--query` parameter and the [multiselect list](query-azure-cli.md#get-multiple-values) format.</span></span> <span data-ttu-id="ba13a-142">Si un comando de la CLI devuelve un solo diccionario JSON, use el formato general `[key1, key2, ..., keyN]` para forzar el orden de las claves.</span><span class="sxs-lookup"><span data-stu-id="ba13a-142">When a CLI command returns a single JSON dictionary, use the general format `[key1, key2, ..., keyN]` to force a key order.</span></span>  <span data-ttu-id="ba13a-143">Para los comandos de la CLI que devuelven una matriz, use el formato general `[].[key1, key2, ..., keyN]` para ordenar los valores de columna.</span><span class="sxs-lookup"><span data-stu-id="ba13a-143">For CLI commands which return an array, use the general format `[].[key1, key2, ..., keyN]` to order column values.</span></span>

<span data-ttu-id="ba13a-144">Por ejemplo, para ordenar la información mostrada anteriormente por identificador, ubicación, grupo de recursos y nombre de máquina virtual:</span><span class="sxs-lookup"><span data-stu-id="ba13a-144">For example, to order the information displayed above by ID, location, resource group, and VM name:</span></span>

```azurecli-interactive
az vm list --out tsv --query '[].[id, location, resourceGroup, name]'
```

```output
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    westus    DEMORG1    DemoVM010
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    westus    DEMORG1    demovm212
/subscriptions/.../resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    westus    DEMORG1    demovm213
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM     westus  RGDEMO001       KBDemo001VM
/subscriptions/.../resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo020       westus  RGDEMO001       KBDemo020
```

<span data-ttu-id="ba13a-145">El ejemplo siguiente muestra cómo se puede canalizar la salida `tsv` a otros comandos en Bash.</span><span class="sxs-lookup"><span data-stu-id="ba13a-145">The next example shows how `tsv` output can be piped to other commands in bash.</span></span> <span data-ttu-id="ba13a-146">Se utiliza la consulta para filtrar la salida y forzar el orden, `grep` selecciona los elementos que tienen el texto "RGD" y el comando `cut` selecciona el cuarto campo para mostrar el nombre de la máquina virtual en la salida.</span><span class="sxs-lookup"><span data-stu-id="ba13a-146">The query is used to filter output and force ordering, `grep` selects items that have text "RGD" in them, then the `cut` command selects the fourth field to show the name of the VM in output.</span></span>

```bash
az vm list --out tsv --query '[].[id, location, resourceGroup, name]' | grep RGD | cut -f4
```

```output
KBDemo001VM
KBDemo020
```

## <a name="set-the-default-output-format"></a><span data-ttu-id="ba13a-147">Establecimiento del formato de salida predeterminado</span><span class="sxs-lookup"><span data-stu-id="ba13a-147">Set the default output format</span></span>

<span data-ttu-id="ba13a-148">Puede usar el comando interactivo `az configure` para configurar el entorno y establecer la configuración predeterminada de los formatos de salida.</span><span class="sxs-lookup"><span data-stu-id="ba13a-148">Use the interactive `az configure` command to set up your environment and establish default settings for output formats.</span></span> <span data-ttu-id="ba13a-149">El formato de salida predeterminado es `json`.</span><span class="sxs-lookup"><span data-stu-id="ba13a-149">The default output format is `json`.</span></span>

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
 [1] json - JSON formatted output that most closely matches API responses.
 [2] jsonc - Colored JSON formatted output that most closely matches API responses.
 [3] table - Human-readable output format.
 [4] tsv - Tab- and Newline-delimited. Great for GREP, AWK, etc.
 [5] yaml - YAML formatted output. An alternative to JSON. Great for configuration files.
 [6] none - No output, except for errors and warnings.
Please enter a choice [1]:
```

<span data-ttu-id="ba13a-150">Para más información sobre cómo configurar el entorno, consulte [Configuración de la CLI de Azure](/cli/azure/azure-cli-configuration).</span><span class="sxs-lookup"><span data-stu-id="ba13a-150">To learn more about configuring your environment, see [Azure CLI configuration](/cli/azure/azure-cli-configuration).</span></span>
