---
title: Resultados del comando de consulta con la CLI de Azure 2.0
description: "Obtenga información acerca de cómo realizar consultas JMESPath con la salida de los comandos de la CLI de Azure 2.0."
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/22/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 2a0cdc34bbaf0864885588ecaddff725c744c90e
ms.sourcegitcommit: 5a4c7205087d2f6c4800cf25178f0543a6157d99
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/24/2018
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="b1b42-103">Uso de consultas JMESPath con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="b1b42-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="b1b42-104">La CLI de Azure 2.0 utiliza el argumento `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados de los comandos.</span><span class="sxs-lookup"><span data-stu-id="b1b42-104">The Azure CLI 2.0 uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="b1b42-105">JMESPath es un lenguaje de consulta para JSON que ofrece la posibilidad de seleccionar y presentar datos de la salida de la CLI.</span><span class="sxs-lookup"><span data-stu-id="b1b42-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="b1b42-106">Estas consultas se ejecutan en la salida JSON antes de realizar cualquier otro formato de presentación.</span><span class="sxs-lookup"><span data-stu-id="b1b42-106">These queries are executed on the JSON output, before performing any other display formatting.</span></span>

<span data-ttu-id="b1b42-107">El argumento `--query` es compatible con todos los comandos de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="b1b42-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="b1b42-108">Los ejemplos de este artículo cubren los casos de uso más comunes y muestran cómo usar las características de JMESPath.</span><span class="sxs-lookup"><span data-stu-id="b1b42-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="b1b42-109">Trabajar con la salida de diccionario</span><span class="sxs-lookup"><span data-stu-id="b1b42-109">Work with dictionary output</span></span>

<span data-ttu-id="b1b42-110">Los comandos que devuelven un diccionario JSON se pueden explorar por los nombres de clave por sí mismos.</span><span class="sxs-lookup"><span data-stu-id="b1b42-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="b1b42-111">Las rutas de acceso de las claves utilizan el carácter `.` como separador.</span><span class="sxs-lookup"><span data-stu-id="b1b42-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="b1b42-112">En el ejemplo siguiente se extrae una lista de las claves SSH públicas que pueden conectarse a una máquina virtual Linux:</span><span class="sxs-lookup"><span data-stu-id="b1b42-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="b1b42-113">También puede obtener varios valores, colocándolos en una matriz ordenada.</span><span class="sxs-lookup"><span data-stu-id="b1b42-113">You can also get multiple values, putting them in an ordered array.</span></span> <span data-ttu-id="b1b42-114">La matriz no tiene ninguna información de clave, pero el orden de los elementos de la matriz coincide con el orden de las claves consultadas.</span><span class="sxs-lookup"><span data-stu-id="b1b42-114">The array doesn't have any key information, but the order of the array's elements matches the order of the queried keys.</span></span> <span data-ttu-id="b1b42-115">En el ejemplo siguiente se muestra cómo recuperar el nombre de oferta de la imagen de Azure y el tamaño del disco del sistema operativo:</span><span class="sxs-lookup"><span data-stu-id="b1b42-115">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="b1b42-116">Si desea que las claves estén presentes en la salida, puede usar una sintaxis de diccionario alternativa.</span><span class="sxs-lookup"><span data-stu-id="b1b42-116">If you want keys in your output, you can use an alternate dictionary syntax.</span></span> <span data-ttu-id="b1b42-117">La selección de múltiples elementos en un diccionario utiliza el formato `{displayKey:keyPath, ...}` para filtrar según la expresión JMESPath `keyPath`.</span><span class="sxs-lookup"><span data-stu-id="b1b42-117">Multiple element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="b1b42-118">Esto se muestra en la salida como `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="b1b42-118">This displays in the output as `{displayKey: value}`.</span></span> <span data-ttu-id="b1b42-119">En el ejemplo siguiente se toma la consulta del último ejemplo, que resulta más clara asignando claves a la salida:</span><span class="sxs-lookup"><span data-stu-id="b1b42-119">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="b1b42-120">Al mostrar información en el formato de salida `table`, la presentación del diccionario es especialmente útil.</span><span class="sxs-lookup"><span data-stu-id="b1b42-120">When displaying information in the `table` output format, dictionary display is especially useful.</span></span> <span data-ttu-id="b1b42-121">Esto permite establecer sus propios encabezados de columna, lo que hace la salida aún más fácil de leer.</span><span class="sxs-lookup"><span data-stu-id="b1b42-121">This allows for setting your own column headers, making output even easier to read.</span></span> <span data-ttu-id="b1b42-122">Para más información sobre los formatos de salida, consulte [Formatos de salida de los comandos de la CLI de Azure 2.0](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="b1b42-122">For more information on output formats, see [Output formats for Azure CLI 2.0 commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="b1b42-123">Determinadas claves se filtran y no se imprimen en la vista de tabla.</span><span class="sxs-lookup"><span data-stu-id="b1b42-123">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="b1b42-124">Estas claves son `id`, `type` y `etag`.</span><span class="sxs-lookup"><span data-stu-id="b1b42-124">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="b1b42-125">Si necesita mostrar esta información, puede cambiar el nombre de la clave y evitar el filtrado.</span><span class="sxs-lookup"><span data-stu-id="b1b42-125">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="b1b42-126">Trabajar con la salida de lista</span><span class="sxs-lookup"><span data-stu-id="b1b42-126">Work with list output</span></span>

<span data-ttu-id="b1b42-127">Los comandos de la CLI que pueden devolver más de un valor siempre devuelven una matriz.</span><span class="sxs-lookup"><span data-stu-id="b1b42-127">CLI commands that may return more than one value always return an array.</span></span> <span data-ttu-id="b1b42-128">Es posible acceder a los elementos de la matriz por su índice, pero nunca hay garantía de orden por parte de la CLI.</span><span class="sxs-lookup"><span data-stu-id="b1b42-128">Arrays can have their elements accessed by index, but there's never an order guarantee from the CLI.</span></span> <span data-ttu-id="b1b42-129">La mejor manera para consultar una matriz de valores es aplanar dichos valores con el operador `[]`.</span><span class="sxs-lookup"><span data-stu-id="b1b42-129">The best way to query an array of values is to flatten them with the `[]` operator.</span></span> <span data-ttu-id="b1b42-130">El operador se escribe después de la clave de la matriz o como el primer elemento de la expresión.</span><span class="sxs-lookup"><span data-stu-id="b1b42-130">The operator is written after the key for the array, or as the first element in the expression.</span></span> <span data-ttu-id="b1b42-131">El aplanado ejecuta la consulta con cada elemento individual de la matriz y coloca los valores resultantes en una nueva matriz.</span><span class="sxs-lookup"><span data-stu-id="b1b42-131">Flattening runs the query following it against each individual element in the array, and places the resulting values into a new array.</span></span> <span data-ttu-id="b1b42-132">En el ejemplo siguiente se imprime el nombre y el sistema operativo que se ejecuta en cada máquina virtual de un grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="b1b42-132">The following example prints out the name and OS running on each VM in a resource group.</span></span> 

```azurecli
az vm list -g QueryDemo --query '[].{name:name, image:storageProfile.imageReference.offer}'
```

```json
[
  {
    "image": "CentOS",
    "name": "CentBox"
  },
  {
    "image": "openSUSE-Leap",
    "name": "SUSEBox"
  },
  {
    "image": "UbuntuServer",
    "name": "TestVM"
  },
  {
    "image": "UbuntuServer",
    "name": "Test2"
  },
  {
    "image": "WindowsServer",
    "name": "WinServ"
  }
]
```

<span data-ttu-id="b1b42-133">También se pueden aplanar las matrices que forman parte de una ruta de acceso de clave.</span><span class="sxs-lookup"><span data-stu-id="b1b42-133">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="b1b42-134">En este ejemplo se muestra una consulta que obtiene los identificadores de objeto de Azure de las NIC a las que está conectada una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="b1b42-134">This example demonstrates a query that gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="b1b42-135">Filtrado de la salida de la matriz con predicados</span><span class="sxs-lookup"><span data-stu-id="b1b42-135">Filter array output with predicates</span></span>

<span data-ttu-id="b1b42-136">JMESPath ofrece [expresiones de filtro](http://jmespath.org/specification.html#filterexpressions) para filtrar los datos mostrados.</span><span class="sxs-lookup"><span data-stu-id="b1b42-136">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="b1b42-137">Estas expresiones son eficaces, especialmente cuando se combinan con las [funciones integradas de JMESPath](http://jmespath.org/specification.html#built-in-functions) para realizar coincidencias parciales o manipular los datos en un formato estándar.</span><span class="sxs-lookup"><span data-stu-id="b1b42-137">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to perform partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="b1b42-138">Las expresiones de filtro solo funcionan en datos de matriz y, cuando se utilizan en cualquier otra situación, devuelven el valor `null`.</span><span class="sxs-lookup"><span data-stu-id="b1b42-138">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="b1b42-139">Por ejemplo, puede tomar la salida de comandos como `vm list` y filtrarla para buscar tipos específicos de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="b1b42-139">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="b1b42-140">En el ejemplo siguiente se amplía el anterior filtrando el tipo de máquina virtual para capturar solo máquinas virtuales Windows e imprimir su nombre.</span><span class="sxs-lookup"><span data-stu-id="b1b42-140">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="b1b42-141">Experimentación con las consultas de forma interactiva</span><span class="sxs-lookup"><span data-stu-id="b1b42-141">Experiment with queries interactively</span></span>

<span data-ttu-id="b1b42-142">Para experimentar con expresiones JMESPath, puede querer trabajar de forma que pueda editar las consultas rápidamente y revisar la salida.</span><span class="sxs-lookup"><span data-stu-id="b1b42-142">To experiment with JMESPath expressions, you might want to work in a way where you can quickly edit queries and inspect the output.</span></span> <span data-ttu-id="b1b42-143">El paquete de Python [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) ofrece un entorno interactivo que permite canalizar los datos como entrada y, a continuación, escribir consultas en el programa para extraer los datos.</span><span class="sxs-lookup"><span data-stu-id="b1b42-143">An interactive environment is offered by the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package, which allows for piping data as input and then writing in-program queries to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list | jpterm
```
