---
title: Resultados del comando de consulta con la CLI de Azure 2.0
description: Obtenga información acerca de cómo realizar consultas JMESPath con la salida de los comandos de la CLI de Azure 2.0.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 55880b87e1bffc37bbdeaeb84206deb5b9b7b227
ms.sourcegitcommit: 0e688704889fc88b91588bb6678a933c2d54f020
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/11/2018
ms.locfileid: "44388384"
---
# <a name="use-jmespath-queries-with-azure-cli-20"></a><span data-ttu-id="e6fe2-103">Uso de consultas JMESPath con la CLI de Azure 2.0</span><span class="sxs-lookup"><span data-stu-id="e6fe2-103">Use JMESPath queries with Azure CLI 2.0</span></span>

<span data-ttu-id="e6fe2-104">La CLI de Azure 2.0 utiliza el argumento `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados de los comandos.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-104">The Azure CLI 2.0 uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="e6fe2-105">JMESPath es un lenguaje de consulta para JSON que ofrece la posibilidad de seleccionar y presentar datos de la salida de la CLI.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-105">JMESPath is a query language for JSON, giving you the ability to select and present data from CLI output.</span></span> <span data-ttu-id="e6fe2-106">Estas consultas se ejecutan en la salida JSON antes de realizar cualquier otro formato de presentación.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-106">These queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="e6fe2-107">El argumento `--query` es compatible con todos los comandos de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="e6fe2-108">Los ejemplos de este artículo cubren los casos de uso más comunes y muestran cómo usar las características de JMESPath.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-108">This article's examples cover common use cases and demonstrate how to use the features of JMESPath.</span></span>

## <a name="work-with-dictionary-output"></a><span data-ttu-id="e6fe2-109">Trabajar con la salida de diccionario</span><span class="sxs-lookup"><span data-stu-id="e6fe2-109">Work with dictionary output</span></span>

<span data-ttu-id="e6fe2-110">Los comandos que devuelven un diccionario JSON se pueden explorar por los nombres de clave por sí mismos.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-110">Commands that return a JSON dictionary can be explored by their key names alone.</span></span> <span data-ttu-id="e6fe2-111">Las rutas de acceso de las claves utilizan el carácter `.` como separador.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-111">Key paths use the `.` character as a separator.</span></span> <span data-ttu-id="e6fe2-112">En el ejemplo siguiente se extrae una lista de las claves SSH públicas que pueden conectarse a una máquina virtual Linux:</span><span class="sxs-lookup"><span data-stu-id="e6fe2-112">The following example pulls a list of the public SSH keys allowed to connect to a Linux VM:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

<span data-ttu-id="e6fe2-113">Si hay varios valores, se pueden colocar en una matriz ordenada.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-113">Multiple values can be put into an ordered array.</span></span> <span data-ttu-id="e6fe2-114">En el ejemplo siguiente se muestra cómo recuperar el nombre de oferta de la imagen de Azure y el tamaño del disco del sistema operativo:</span><span class="sxs-lookup"><span data-stu-id="e6fe2-114">The following example shows how to retrieve the Azure image offering name and the size of the OS disk:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

<span data-ttu-id="e6fe2-115">Si desea que las claves estén presentes en la salida, puede usar una sintaxis de diccionario alternativa.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-115">If you want keys in your output, you can use an alternate dictionary syntax.</span></span>  <span data-ttu-id="e6fe2-116">La selección de elementos en un diccionario utiliza el formato `{displayKey:keyPath, ...}` para filtrar según la expresión JMESPath `keyPath`.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-116">Element selection into a dictionary uses the format `{displayKey:keyPath, ...}` to filter on the `keyPath` JMESPath expression.</span></span> <span data-ttu-id="e6fe2-117">En los valores de salida, los pares clave-valor se cambian a `{displayKey: value}`.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-117">In the output values, the key/value pairs are changed to `{displayKey: value}`.</span></span> <span data-ttu-id="e6fe2-118">En el ejemplo siguiente se toma la consulta del último ejemplo, que resulta más clara asignando claves a la salida:</span><span class="sxs-lookup"><span data-stu-id="e6fe2-118">The next example takes the last example's query, and makes it clearer by assigning keys to the output:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

<span data-ttu-id="e6fe2-119">Al mostrar información con el formato de salida `table`, la presentación del diccionario permite establecer sus propios encabezados de columna.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-119">When displaying information in the `table` output format, dictionary display allows setting your own column headers.</span></span> <span data-ttu-id="e6fe2-120">Para más información sobre los formatos de salida, consulte [Formatos de salida de los comandos de la CLI de Azure 2.0](/cli/azure/format-output-azure-cli).</span><span class="sxs-lookup"><span data-stu-id="e6fe2-120">For more information on output formats, see [Output formats for Azure CLI 2.0 commands](/cli/azure/format-output-azure-cli).</span></span>

> [!NOTE]
> <span data-ttu-id="e6fe2-121">Determinadas claves se filtran y no se imprimen en la vista de tabla.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-121">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="e6fe2-122">Estas claves son `id`, `type` y `etag`.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-122">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="e6fe2-123">Si necesita mostrar esta información, puede cambiar el nombre de la clave y evitar el filtrado.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-123">If you need to see this information, you can change the key name and avoid filtering.</span></span>
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a><span data-ttu-id="e6fe2-124">Trabajar con la salida de lista</span><span class="sxs-lookup"><span data-stu-id="e6fe2-124">Work with list output</span></span>

<span data-ttu-id="e6fe2-125">Los comandos de la CLI que pueden devolver más de un valor devuelven una matriz.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-125">CLI commands that may return  more than one value return an array.</span></span> <span data-ttu-id="e6fe2-126">A los elementos de la matriz se accede por el índice y no se pueden devolver en el mismo orden cada vez.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-126">Array elements are accessed by index and may not be returned in the same order every time.</span></span> <span data-ttu-id="e6fe2-127">Para consultar todos los elementos de una matriz a la vez, puede aplanarla con el operador `[]`.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-127">You can query all array elements at once by flattening them with the `[]` operator.</span></span> <span data-ttu-id="e6fe2-128">El operador se escribe después de la matriz o como el primer elemento de una expresión.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-128">The operator is put after the array or as the first element in an expression.</span></span> <span data-ttu-id="e6fe2-129">Para aplanar una matriz, se ejecuta la consulta posterior en cada elemento de la matriz.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-129">Flattening an array runs the query after it against each element of the array.</span></span>

<span data-ttu-id="e6fe2-130">En el ejemplo siguiente se imprime el nombre y el sistema operativo que se ejecuta en cada máquina virtual de un grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-130">The following example prints out the name and OS running on each VM in a resource group.</span></span>

```azurecli-interactive
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

<span data-ttu-id="e6fe2-131">También se pueden aplanar las matrices que forman parte de una ruta de acceso de clave.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-131">Arrays that are part of a key path can be flattened as well.</span></span> <span data-ttu-id="e6fe2-132">La siguiente consulta obtiene los identificadores de objeto de Azure de las NIC a las que está conectada una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-132">The following query gets the Azure object IDs for the NICs a VM is connected to.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a><span data-ttu-id="e6fe2-133">Filtrado de la salida de la matriz con predicados</span><span class="sxs-lookup"><span data-stu-id="e6fe2-133">Filter array output with predicates</span></span>

<span data-ttu-id="e6fe2-134">JMESPath ofrece [expresiones de filtro](http://jmespath.org/specification.html#filterexpressions) para filtrar los datos mostrados.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-134">JMESPath offers [filtering expressions](http://jmespath.org/specification.html#filterexpressions) to filter out the data displayed.</span></span> <span data-ttu-id="e6fe2-135">Estas expresiones son eficaces, especialmente cuando se combinan con las [funciones integradas de JMESPath](http://jmespath.org/specification.html#built-in-functions) para realizar coincidencias parciales o manipular los datos en un formato estándar.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-135">These expressions are powerful, especially when combined with [JMESPath built-in functions](http://jmespath.org/specification.html#built-in-functions) to do partial matches or manipulate data into a standard format.</span></span> <span data-ttu-id="e6fe2-136">Las expresiones de filtro solo funcionan en datos de matriz y, cuando se utilizan en cualquier otra situación, devuelven el valor `null`.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-136">Filtering expressions only work on array data, and when used in any other situation, return the `null` value.</span></span> <span data-ttu-id="e6fe2-137">Por ejemplo, puede tomar la salida de comandos como `vm list` y filtrarla para buscar tipos específicos de máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-137">For example, you can take the output of commands like `vm list` and filter on it to look for specific types of VMs.</span></span> <span data-ttu-id="e6fe2-138">En el ejemplo siguiente se amplía el anterior filtrando el tipo de máquina virtual para capturar solo máquinas virtuales Windows e imprimir su nombre.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-138">The following example expands on the previous by filtering out the VM type to capture only Windows VMs and print their name.</span></span>

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="e6fe2-139">Experimentación con las consultas de forma interactiva</span><span class="sxs-lookup"><span data-stu-id="e6fe2-139">Experiment with queries interactively</span></span>

<span data-ttu-id="e6fe2-140">Para empezar a aprender JMESPath, el paquete [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) de Python ofrece un entorno interactivo para experimentar con las consultas.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-140">To start learning JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to experiment with queries.</span></span> <span data-ttu-id="e6fe2-141">Los datos se canalizan como entrada y, a continuación, se escriben consultas en el programa y se puede editar para extraer los datos.</span><span class="sxs-lookup"><span data-stu-id="e6fe2-141">Data is piped as input, and then in-program queries are written and edited to extract the data.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
