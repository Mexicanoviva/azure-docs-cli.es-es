---
title: Resultados del comando de consulta con la CLI de Azure
description: Obtenga información acerca de cómo realizar consultas JMESPath con la salida de los comandos de la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/12/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: e878c467f71423cc8c9caa1f8cfe270d0019c48b
ms.sourcegitcommit: 399f0a2997675fbb280243e4234cf63c3bbca819
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/18/2019
ms.locfileid: "67194845"
---
# <a name="query-azure-cli-command-output"></a><span data-ttu-id="89987-103">Resultados de los comandos de consulta de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="89987-103">Query Azure CLI command output</span></span>

<span data-ttu-id="89987-104">La CLI de Azure utiliza el argumento `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados de los comandos.</span><span class="sxs-lookup"><span data-stu-id="89987-104">The Azure CLI uses the `--query` argument to execute a [JMESPath query](http://jmespath.org) on the results of commands.</span></span> <span data-ttu-id="89987-105">JMESPath es un lenguaje de consulta para JSON que ofrece la posibilidad de seleccionar y modificar datos de la salida de la CLI.</span><span class="sxs-lookup"><span data-stu-id="89987-105">JMESPath is a query language for JSON, giving you the ability to select and modify data from CLI output.</span></span> <span data-ttu-id="89987-106">Las consultas se ejecutan en la salida JSON antes de realizar cualquier otro formato de presentación.</span><span class="sxs-lookup"><span data-stu-id="89987-106">Queries are executed on the JSON output before any display formatting.</span></span>

<span data-ttu-id="89987-107">El argumento `--query` es compatible con todos los comandos de la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="89987-107">The `--query` argument is supported by all commands in the Azure CLI.</span></span> <span data-ttu-id="89987-108">En este artículo se explica cómo usar las características de JMESPath con una serie de pequeños y sencillos ejemplos.</span><span class="sxs-lookup"><span data-stu-id="89987-108">This article covers how to use the features of JMESPath with a series of small, simple examples.</span></span>

## <a name="dictionary-and-list-cli-results"></a><span data-ttu-id="89987-109">Diccionario y lista de resultados de la CLI</span><span class="sxs-lookup"><span data-stu-id="89987-109">Dictionary and list CLI results</span></span>

<span data-ttu-id="89987-110">Incluso cuando se utiliza un formato de salida distinto de JSON, los resultados de los comandos de la CLI se tratan primero como JSON para las consultas.</span><span class="sxs-lookup"><span data-stu-id="89987-110">Even when using an output format other than JSON, CLI command results are first treated as JSON for queries.</span></span> <span data-ttu-id="89987-111">Los resultados de CLI son una matriz JSON o un diccionario.</span><span class="sxs-lookup"><span data-stu-id="89987-111">CLI results are either a JSON array or dictionary.</span></span> <span data-ttu-id="89987-112">Las matrices son secuencias de objetos que se pueden indexar y los diccionarios son objetos desordenados a los que se accede con claves.</span><span class="sxs-lookup"><span data-stu-id="89987-112">Arrays are sequences of objects that can be indexed, and dictionaries are unordered objects accessed with keys.</span></span> <span data-ttu-id="89987-113">Los comandos que _pueden_devolver más de un objeto devuelven una matriz y los comandos que _siempre_ devuelven _únicamente_ un solo objeto devuelven un diccionario.</span><span class="sxs-lookup"><span data-stu-id="89987-113">Commands that _could_ return more than one object return an array, and commands that _always_ return _only_ a single object return a dictionary.</span></span>

## <a name="get-properties-in-a-dictionary"></a><span data-ttu-id="89987-114">Obtención de propiedades en un diccionario</span><span class="sxs-lookup"><span data-stu-id="89987-114">Get properties in a dictionary</span></span>

<span data-ttu-id="89987-115">Al trabajar con los resultados del diccionario, puede acceder a las propiedades del nivel superior con solo la clave.</span><span class="sxs-lookup"><span data-stu-id="89987-115">Working with dictionary results, you can access properties from the top level with just the key.</span></span> <span data-ttu-id="89987-116">El carácter `.` (__subexpresión__) se utiliza para acceder a las propiedades de los diccionarios anidados.</span><span class="sxs-lookup"><span data-stu-id="89987-116">The `.` (__subexpression__) character is used to access properties of nested dictionaries.</span></span> <span data-ttu-id="89987-117">Antes de introducir consultas, eche un vistazo a la salida no modificada del comando `az vm show`:</span><span class="sxs-lookup"><span data-stu-id="89987-117">Before introducing queries, take a look at the unmodified output of the `az vm show` command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

<span data-ttu-id="89987-118">El comando dará como resultado un diccionario.</span><span class="sxs-lookup"><span data-stu-id="89987-118">The command will output a dictionary.</span></span> <span data-ttu-id="89987-119">Se ha omitido parte del contenido.</span><span class="sxs-lookup"><span data-stu-id="89987-119">Some content has been omitted.</span></span>

```json
{
  "additionalCapabilities": null,
  "availabilitySet": null,
  "diagnosticsProfile": {
    "bootDiagnostics": {
      "enabled": true,
      "storageUri": "https://xxxxxx.blob.core.windows.net/"
    }
  },
  ...
  "osProfile": {
    "adminPassword": null,
    "adminUsername": "azureuser",
    "allowExtensionOperations": true,
    "computerName": "TestVM",
    "customData": null,
    "linuxConfiguration": {
      "disablePasswordAuthentication": true,
      "provisionVmAgent": true,
      "ssh": {
        "publicKeys": [
          {
            "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
            "path": "/home/azureuser/.ssh/authorized_keys"
          }
        ]
      }
    },
    "secrets": [],
    "windowsConfiguration": null
  },
  ....
}
```

<span data-ttu-id="89987-120">El siguiente comando obtiene las claves públicas SSH autorizadas para conectarse a la máquina virtual mediante la adición de una consulta:</span><span class="sxs-lookup"><span data-stu-id="89987-120">The following command gets the SSH public keys authorized to connect to the VM by adding a query:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys -o json
```

```json
[
  {
    "keyData": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso",
    "path": "/home/azureuser/.ssh/authorized_keys"
  }
]
```

<span data-ttu-id="89987-121">Para obtener más de una propiedad, coloque las expresiones entre corchetes `[ ]` (una __lista de selección múltiple__) como una lista separada por comas.</span><span class="sxs-lookup"><span data-stu-id="89987-121">To get more than one property, put expressions in square brackets  `[ ]` (a __multiselect list__) as a comma-separated list.</span></span> <span data-ttu-id="89987-122">Para obtener el nombre de la máquina virtual, el usuario administrador y la clave SSH de una sola vez, utilice el comando:</span><span class="sxs-lookup"><span data-stu-id="89987-122">To get the VM name, admin user, and SSH key all at once use the command:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '[name, osProfile.adminUsername, osProfile.linuxConfiguration.ssh.publicKeys[0].keyData]' -o json
```

```json
[
  "TestVM",
  "azureuser",
  "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
]
```

<span data-ttu-id="89987-123">Estos valores se muestran en la matriz de resultados en el orden en que se proporcionaron en la consulta.</span><span class="sxs-lookup"><span data-stu-id="89987-123">These values are listed in the result array in the order they were given in the query.</span></span> <span data-ttu-id="89987-124">Dado que el resultado es una matriz, no hay claves asociadas a los resultados.</span><span class="sxs-lookup"><span data-stu-id="89987-124">Since the result is an array, there are no keys associated with the results.</span></span>

## <a name="get-a-single-value"></a><span data-ttu-id="89987-125">Obtener un solo valor</span><span class="sxs-lookup"><span data-stu-id="89987-125">Get a single value</span></span>

<span data-ttu-id="89987-126">Un caso común es si necesita obtener solo _un_ valor de un comando de la CLI, como un identificador de recurso de Azure, un nombre de recurso, un nombre de usuario o una contraseña.</span><span class="sxs-lookup"><span data-stu-id="89987-126">A common case is that you need to only get _one_ value out of a CLI command, such as an Azure resource ID, a resource name, a username, or a password.</span></span> <span data-ttu-id="89987-127">En ese caso, se suele querer también almacenar el valor en una variable de entorno local.</span><span class="sxs-lookup"><span data-stu-id="89987-127">In that case, you also often want to store the value in a local environment variable.</span></span> <span data-ttu-id="89987-128">Para obtener una sola propiedad, primero debe asegurarse de que está obteniendo solo una propiedad de la consulta.</span><span class="sxs-lookup"><span data-stu-id="89987-128">To get a single property, first make sure that you're only getting one property out of the query.</span></span> <span data-ttu-id="89987-129">Modificamos el ejemplo anterior para obtener solo el nombre de usuario del administrador:</span><span class="sxs-lookup"><span data-stu-id="89987-129">Modifying the last example to get only the admin username:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

<span data-ttu-id="89987-130">Esto parece un valor único válido, pero tenga en cuenta que los `"` caracteres se devuelven como parte de la salida.</span><span class="sxs-lookup"><span data-stu-id="89987-130">This looks like a valid single value, but note that the `"` characters are returned as part of the output.</span></span> <span data-ttu-id="89987-131">Esto indica que el objeto es una cadena JSON.</span><span class="sxs-lookup"><span data-stu-id="89987-131">This indicates that the object is a JSON string.</span></span> <span data-ttu-id="89987-132">Es importante tener en cuenta que al asignar este valor directamente como salida del comando a una variable de entorno, el Shell podría __no__ interpretar las comillas:</span><span class="sxs-lookup"><span data-stu-id="89987-132">It's important to note that when you assign this value directly as output from the command to an environment variable, the quotes may __not__ be interpreted by the shell:</span></span>

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

<span data-ttu-id="89987-133">Es casi seguro que este no es el comportamiento que desea.</span><span class="sxs-lookup"><span data-stu-id="89987-133">This is almost certainly not what you want.</span></span> <span data-ttu-id="89987-134">En este caso, desea utilizar un formato de salida que no incluya los valores devueltos entre comillas con la información del tipo.</span><span class="sxs-lookup"><span data-stu-id="89987-134">In this case, you want to use an output format which doesn't enclose returned values with type information.</span></span> <span data-ttu-id="89987-135">La mejor opción de salida que la CLI ofrece con este fin `tsv`, valores separados por tabulaciones.</span><span class="sxs-lookup"><span data-stu-id="89987-135">The best output option that the CLI offers for this purpose is `tsv`, tab-separated values.</span></span> <span data-ttu-id="89987-136">En concreto, al recuperar un valor que es un valor solo (no diccionario o una lista), es seguro que la salida `tsv` no estará entre comillas.</span><span class="sxs-lookup"><span data-stu-id="89987-136">In particular, when retrieving a value that's only a single value (not a dictionary or list), `tsv` output is guaranteed to be unquoted.</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

<span data-ttu-id="89987-137">Para más información sobre el formato de salida de `tsv`, consulte [Formatos de salida: formato de salida TSV](format-output-azure-cli.md#tsv-output-format).</span><span class="sxs-lookup"><span data-stu-id="89987-137">For more information about the `tsv` output format, see [Output formats - TSV output format](format-output-azure-cli.md#tsv-output-format)</span></span>

## <a name="rename-properties-in-a-query"></a><span data-ttu-id="89987-138">Cambio del nombre de las propiedades en una consulta</span><span class="sxs-lookup"><span data-stu-id="89987-138">Rename properties in a query</span></span>

<span data-ttu-id="89987-139">Para obtener un diccionario en lugar de una matriz al consultar valores múltiples, utilice el operador `{ }` (__hash de selección múltiple__).</span><span class="sxs-lookup"><span data-stu-id="89987-139">To get a dictionary instead of an array when querying for multiple values, use the `{ }` (__multiselect hash__) operator.</span></span>
<span data-ttu-id="89987-140">El formato de un hash de selección múltiple es `{displayName:JMESPathExpression, ...}`.</span><span class="sxs-lookup"><span data-stu-id="89987-140">The format for a multiselect hash is `{displayName:JMESPathExpression, ...}`.</span></span>
<span data-ttu-id="89987-141">`displayName` será la cadena que se muestra en la salida y `JMESPathExpression` es la expresión JMESPath que se va a evaluar.</span><span class="sxs-lookup"><span data-stu-id="89987-141">`displayName` will be the string shown in output, and `JMESPathExpression` is the JMESPath expression to evaluate.</span></span> <span data-ttu-id="89987-142">Modificación del ejemplo de la última sección mediante el cambio de la lista de selección múltiple a un hash:</span><span class="sxs-lookup"><span data-stu-id="89987-142">Modifying the example from the last section by changing the multiselect list to a hash:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKey:osProfile.linuxConfiguration.ssh.publicKeys[0].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "ssh-key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso"
}
```

## <a name="get-properties-in-an-array"></a><span data-ttu-id="89987-143">Obtención de propiedades en una matriz</span><span class="sxs-lookup"><span data-stu-id="89987-143">Get properties in an array</span></span>

<span data-ttu-id="89987-144">Una matriz no tiene propiedades propias, pero se puede indexar.</span><span class="sxs-lookup"><span data-stu-id="89987-144">An array has no properties of its own, but it can be indexed.</span></span> <span data-ttu-id="89987-145">Esta característica se muestra en el último ejemplo con la expresión `publicKeys[0]`, que obtiene el primer elemento de la matriz `publicKeys`.</span><span class="sxs-lookup"><span data-stu-id="89987-145">This feature is shown in the last example with the expression `publicKeys[0]`, which gets the first element of the `publicKeys` array.</span></span> <span data-ttu-id="89987-146">No hay garantía de que la salida de la CLI esté ordenada, así que evite utilizar la indexación a menos que esté seguro del orden o no le importe el elemento que se obtenga.</span><span class="sxs-lookup"><span data-stu-id="89987-146">There's no guarantee CLI output is ordered, so avoid using indexing unless you're sure of the order or don't care what element you get.</span></span> <span data-ttu-id="89987-147">Para acceder a las propiedades de los elementos de una matriz, se realiza una de dos operaciones: _simplificación_  y _filtrado_.</span><span class="sxs-lookup"><span data-stu-id="89987-147">To access the properties of elements in an array, you do one of two operations: _flattening_ and _filtering_.</span></span> <span data-ttu-id="89987-148">En esta sección se explica cómo simplificar una matriz.</span><span class="sxs-lookup"><span data-stu-id="89987-148">This section covers how to flatten an array.</span></span>

<span data-ttu-id="89987-149">La simplificación de una matriz se realiza con el operador de JMESPath `[]`.</span><span class="sxs-lookup"><span data-stu-id="89987-149">Flattening an array is done with the `[]` JMESPath operator.</span></span> <span data-ttu-id="89987-150">Todas las expresiones después del operador `[]` se aplican a cada elemento de la matriz actual.</span><span class="sxs-lookup"><span data-stu-id="89987-150">All expressions after the `[]` operator are applied to each element in the current array.</span></span>
<span data-ttu-id="89987-151">Si `[]` aparece al principio de la consulta, aplana el resultado del comando de la CLI.</span><span class="sxs-lookup"><span data-stu-id="89987-151">If `[]` appears at the start of the query, it flattens the CLI command result.</span></span> <span data-ttu-id="89987-152">Los resultados de `az vm list` pueden inspeccionarse con esta característica.</span><span class="sxs-lookup"><span data-stu-id="89987-152">The results of `az vm list` can be inspected with this feature.</span></span>
<span data-ttu-id="89987-153">Para obtener el nombre, el sistema operativo y el nombre del administrador de cada máquina virtual en un grupo de recursos:</span><span class="sxs-lookup"><span data-stu-id="89987-153">To get the name, OS, and administrator name for each VM in a resource group:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, admin:osProfile.adminUsername}' -o json
```

```json
[
  {
    "Name": "Test-2",
    "OS": "Linux",
    "admin": "sttramer"
  },
  {
    "Name": "TestVM",
    "OS": "Linux",
    "admin": "azureuser"
  },
  {
    "Name": "WinTest",
    "OS": "Windows",
    "admin": "winadmin"
  }
]
```

<span data-ttu-id="89987-154">Cuando se combina con el formato de salida `--output table`, los nombres de columna coinciden con el valor `displayKey` del hash de selección múltiple:</span><span class="sxs-lookup"><span data-stu-id="89987-154">When combined with the `--output table` output format, the column names match up with the `displayKey` value of the multiselect hash:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query '[].{Name:name, OS:storageProfile.osDisk.osType, Admin:osProfile.adminUsername}' --output table
```

```output
Name     OS       Admin
-------  -------  ---------
Test-2   Linux    sttramer
TestVM   Linux    azureuser
WinTest  Windows  winadmin
```

> [!NOTE]
>
> <span data-ttu-id="89987-155">Determinadas claves se filtran y no se imprimen en la vista de tabla.</span><span class="sxs-lookup"><span data-stu-id="89987-155">Certain keys are filtered out and not printed in the table view.</span></span> <span data-ttu-id="89987-156">Estas claves son `id`, `type` y `etag`.</span><span class="sxs-lookup"><span data-stu-id="89987-156">These keys are `id`, `type`, and `etag`.</span></span> <span data-ttu-id="89987-157">Para ver estos valores, puede cambiar el nombre de la clave en un hash de selección múltiple.</span><span class="sxs-lookup"><span data-stu-id="89987-157">To see these values, you can change the key name in a multiselect hash.</span></span>
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

<span data-ttu-id="89987-158">Se puede simplificar cualquier matriz, no solo el resultado de nivel superior devuelto por el comando.</span><span class="sxs-lookup"><span data-stu-id="89987-158">Any array can be flattened, not just the top-level result returned by the command.</span></span> <span data-ttu-id="89987-159">En la última sección, se utilizó la expresión `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` para obtener la clave pública SSH para iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="89987-159">In the last section, the expression `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` was used to get the SSH public key for sign-in.</span></span> <span data-ttu-id="89987-160">Para obtener _cada_ clave pública SSH, la expresión podría escribirse como `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span><span class="sxs-lookup"><span data-stu-id="89987-160">To get _every_ SSH public key, the expression could instead be written as `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.</span></span>
<span data-ttu-id="89987-161">Esta expresión de consulta simplifica la matriz `osProfile.linuxConfiguration.ssh.publicKeys` y, después, se ejecuta la expresión `keyData` en cada elemento:</span><span class="sxs-lookup"><span data-stu-id="89987-161">This query expression flattens the `osProfile.linuxConfiguration.ssh.publicKeys` array, and then runs the `keyData` expression on each element:</span></span>

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query '{VMName:name, admin:osProfile.adminUsername, sshKeys:osProfile.linuxConfiguration.ssh.publicKeys[].keyData }' -o json
```

```json
{
  "VMName": "TestVM",
  "admin": "azureuser",
  "sshKeys": [
    "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDMobZNJTqgjWn/IB5xlilvE4Y+BMYpqkDnGRUcA0g9BYPgrGSQquCES37v2e3JmpfDPHFsaR+CPKlVr2GoVJMMHeRcMJhj50ZWq0hAnkJBhlZVWy8S7dwdGAqPyPmWM2iJDCVMVrLITAJCno47O4Ees7RCH6ku7kU86b1NOanvrNwqTHr14wtnLhgZ0gQ5GV1oLWvMEVg1YFMIgPRkTsSQKWCG5lLqQ45aU/4NMJoUxGyJTL9i8YxMavaB1Z2npfTQDQo9+womZ7SXzHaIWC858gWNl9e5UFyHDnTEDc14hKkf1CqnGJVcCJkmSfmrrHk/CkmF0ZT3whTHO1DhJTtV stramer@contoso\n"
  ]
}
```

## <a name="filter-arrays"></a><span data-ttu-id="89987-162">Filtrado de matrices</span><span class="sxs-lookup"><span data-stu-id="89987-162">Filter arrays</span></span>

<span data-ttu-id="89987-163">La otra operación utilizada para obtener datos de una matriz es el _filtrado_.</span><span class="sxs-lookup"><span data-stu-id="89987-163">The other operation used to get data from an array is _filtering_.</span></span> <span data-ttu-id="89987-164">El filtrado se realiza con el operador de JMESPath `[?...]`.</span><span class="sxs-lookup"><span data-stu-id="89987-164">Filtering is done with the `[?...]` JMESPath operator.</span></span>
<span data-ttu-id="89987-165">Este operador toma un predicado como su contenido.</span><span class="sxs-lookup"><span data-stu-id="89987-165">This operator takes a predicate as its contents.</span></span> <span data-ttu-id="89987-166">Un predicado es cualquier declaración que se puede evaluar como `true` o `false`.</span><span class="sxs-lookup"><span data-stu-id="89987-166">A predicate is any statement that can be evaluated to either `true` or `false`.</span></span> <span data-ttu-id="89987-167">En la salida se incluyen las expresiones en las que el predicado se evalúa a `true`.</span><span class="sxs-lookup"><span data-stu-id="89987-167">Expressions where the predicate evaluates to `true` are included in the output.</span></span>

<span data-ttu-id="89987-168">JMESPath ofrece la comparación estándar y los operadores lógicos.</span><span class="sxs-lookup"><span data-stu-id="89987-168">JMESPath offers the standard comparison and logical operators.</span></span> <span data-ttu-id="89987-169">Estos incluyen `<`, `<=`, `>`, `>=`, `==` y `!=`.</span><span class="sxs-lookup"><span data-stu-id="89987-169">These include `<`, `<=`, `>`, `>=`, `==`, and `!=`.</span></span>
<span data-ttu-id="89987-170">JMESPath también admite la lógica y (`&&`) o (`||`) y no (`!`).</span><span class="sxs-lookup"><span data-stu-id="89987-170">JMESPath also supports logical and (`&&`), or (`||`), and not (`!`).</span></span> <span data-ttu-id="89987-171">Las expresiones se pueden agrupar entre paréntesis, lo que permite expresiones de predicados más complejas.</span><span class="sxs-lookup"><span data-stu-id="89987-171">Expressions can be grouped within parenthesis, allowing for more complex predicate expressions.</span></span> <span data-ttu-id="89987-172">Para obtener todos los detalles sobre predicados y operaciones lógicas, consulte la [especificación de JMESPath](http://jmespath.org/specification.html).</span><span class="sxs-lookup"><span data-stu-id="89987-172">For the full details on predicates and logical operations, see the [JMESPath specification](http://jmespath.org/specification.html).</span></span>

<span data-ttu-id="89987-173">En la última sección, simplificamos una matriz para obtener la lista completa de todas las máquinas virtuales de un grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="89987-173">In the last section, we flattened an array to get the complete list of all VMs in a resource group.</span></span> <span data-ttu-id="89987-174">Mediante el uso de filtros, esta salida puede restringirse solo a las máquinas virtuales Linux:</span><span class="sxs-lookup"><span data-stu-id="89987-174">Using filters, this output can be restricted to only Linux VMs:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?storageProfile.osDisk.osType=='Linux'].{Name:name,  admin:osProfile.adminUsername}" --output table
```

```output
Name    Admin
------  ---------
Test-2  sttramer
TestVM  azureuser
```

> [!IMPORTANT]
>
> <span data-ttu-id="89987-175">En JMESPath, las cadenas siempre están rodeadas de comillas simples (`'`).</span><span class="sxs-lookup"><span data-stu-id="89987-175">In JMESPath, strings are always surrounded by single quotes (`'`).</span></span> <span data-ttu-id="89987-176">Si utiliza comillas dobles como parte de una cadena en un predicado de filtro, obtendrá una salida vacía.</span><span class="sxs-lookup"><span data-stu-id="89987-176">If you use double quotes as part of a string in a filter predicate, you'll get empty output.</span></span>

<span data-ttu-id="89987-177">JMESPath también tiene funciones integradas que pueden ayudar con el filtrado.</span><span class="sxs-lookup"><span data-stu-id="89987-177">JMESPath also has built-in functions that can help with filtering.</span></span> <span data-ttu-id="89987-178">Una de estas funciones es `contains(string, substring)`, que comprueba si una cadena contiene una subcadena.</span><span class="sxs-lookup"><span data-stu-id="89987-178">One such function is `contains(string, substring)`, which checks to see if a string contains a substring.</span></span> <span data-ttu-id="89987-179">Las expresiones se evalúan antes de llamar a la función, por lo que el primer argumento puede ser una expresión completa de JMESPath.</span><span class="sxs-lookup"><span data-stu-id="89987-179">Expressions are evaluated before calling the function, so the first argument can be a full JMESPath expression.</span></span> <span data-ttu-id="89987-180">En el siguiente ejemplo se encuentran todas las máquinas virtuales que utilizan almacenamiento SSD para su disco de sistema operativo:</span><span class="sxs-lookup"><span data-stu-id="89987-180">The next example finds all VMs using SSD storage for their OS disk:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[?contains(storageProfile.osDisk.managedDisk.storageAccountType,'SSD')].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="89987-181">Esta consulta es un poco larga.</span><span class="sxs-lookup"><span data-stu-id="89987-181">This query is a little long.</span></span> <span data-ttu-id="89987-182">La clave `storageProfile.osDisk.managedDisk.storageAccountType` se menciona dos veces y se vuelve a cambiar en la salida.</span><span class="sxs-lookup"><span data-stu-id="89987-182">The `storageProfile.osDisk.managedDisk.storageAccountType` key is mentioned twice, and rekeyed in the output.</span></span> <span data-ttu-id="89987-183">Una manera de acortarlo es aplicar el filtro después de la simplificación y selección de los datos.</span><span class="sxs-lookup"><span data-stu-id="89987-183">One way to shorten it is to apply the filter after flattening and selecting data.</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "[].{Name:name, Storage:storageProfile.osDisk.managedDisk.storageAccountType}[?contains(Storage,'SSD')]" -o json
```

```json
[
  {
    "Name": "TestVM",
    "Storage": "StandardSSD_LRS"
  },
  {
    "Name": "WinTest",
    "Storage": "StandardSSD_LRS"
  }
]
```

<span data-ttu-id="89987-184">En el caso de matrices grandes, puede ser más rápido aplicar el filtro antes de seleccionar los datos.</span><span class="sxs-lookup"><span data-stu-id="89987-184">For large arrays, it may be faster to apply the filter before selecting data.</span></span>

<span data-ttu-id="89987-185">Consulte la [especificación de JMESPath - Funciones integradas](http://jmespath.org/specification.html#built-in-functions) para ver la lista completa de funciones.</span><span class="sxs-lookup"><span data-stu-id="89987-185">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="change-output"></a><span data-ttu-id="89987-186">Cambio de la salida</span><span class="sxs-lookup"><span data-stu-id="89987-186">Change output</span></span>

<span data-ttu-id="89987-187">Las funciones JMESPath también tienen otro propósito, que es trabajar sobre los resultados de una consulta.</span><span class="sxs-lookup"><span data-stu-id="89987-187">JMESPath functions also have another purpose, which is to operate on the results of a query.</span></span> <span data-ttu-id="89987-188">Cualquier función que devuelva un valor no booleano cambia el resultado de una expresión.</span><span class="sxs-lookup"><span data-stu-id="89987-188">Any function that returns a non-boolean value changes the result of an expression.</span></span>
<span data-ttu-id="89987-189">Por ejemplo, puede ordenar los datos por un valor de propiedad con `sort_by(array, &sort_expression)`.</span><span class="sxs-lookup"><span data-stu-id="89987-189">For example, you can sort data by a property value with `sort_by(array, &sort_expression)`.</span></span> <span data-ttu-id="89987-190">JMESPath utiliza un operador especial, `&`, para expresiones que deben evaluarse posteriormente como parte de una función.</span><span class="sxs-lookup"><span data-stu-id="89987-190">JMESPath uses a special operator, `&`, for expressions that should be evaluated later as part of a function.</span></span> <span data-ttu-id="89987-191">En el ejemplo siguiente se muestra cómo ordenar una lista de máquinas virtuales por el tamaño del disco del sistema operativo:</span><span class="sxs-lookup"><span data-stu-id="89987-191">The next example shows how to sort a VM list by OS disk size:</span></span>

```azurecli-interactive
az vm list -g QueryDemo --query "sort_by([].{Name:name, Size:storageProfile.osDisk.diskSizeGb}, &Size)" --output table
```

```output
Name     Size
-------  ------
TestVM   30
Test-2   32
WinTest  127
```

<span data-ttu-id="89987-192">Consulte la [especificación de JMESPath - Funciones integradas](http://jmespath.org/specification.html#built-in-functions) para ver la lista completa de funciones.</span><span class="sxs-lookup"><span data-stu-id="89987-192">See the [JMESPath specification - Built-in Functions](http://jmespath.org/specification.html#built-in-functions) for the full list of functions.</span></span>

## <a name="experiment-with-queries-interactively"></a><span data-ttu-id="89987-193">Experimentación con las consultas de forma interactiva</span><span class="sxs-lookup"><span data-stu-id="89987-193">Experiment with queries interactively</span></span>

<span data-ttu-id="89987-194">Para empezar a experimentar con JMESPath, el paquete [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) de Python ofrece un entorno interactivo para trabajar con las consultas.</span><span class="sxs-lookup"><span data-stu-id="89987-194">To start experimenting with JMESPath, the [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) Python package offers an interactive environment to work with queries.</span></span> <span data-ttu-id="89987-195">Los datos se canalizan como entrada y, después, se escriben las consultas y se ejecutan en el editor.</span><span class="sxs-lookup"><span data-stu-id="89987-195">Data is piped as input, and then queries are written and run in the editor.</span></span>

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
