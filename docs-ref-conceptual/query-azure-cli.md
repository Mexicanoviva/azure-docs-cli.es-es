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
ms.openlocfilehash: 5e187025e97b1d882bc575fd51970a8250f6210e
ms.sourcegitcommit: bf69c95abf3ed3d589b202c7ff04d8782e2a81ac
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/21/2019
ms.locfileid: "65993044"
---
# <a name="query-azure-cli-command-output"></a>Resultados de los comandos de consulta de la CLI de Azure

La CLI de Azure utiliza el argumento `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados de los comandos. JMESPath es un lenguaje de consulta para JSON que ofrece la posibilidad de seleccionar y modificar datos de la salida de la CLI. Las consultas se ejecutan en la salida JSON antes de realizar cualquier otro formato de presentación.

El argumento `--query` es compatible con todos los comandos de la CLI de Azure. En este artículo se explica cómo usar las características de JMESPath con una serie de pequeños y sencillos ejemplos.

## <a name="dictionary-and-list-cli-results"></a>Diccionario y lista de resultados de la CLI

Incluso cuando se utiliza un formato de salida distinto de JSON, los resultados de los comandos de la CLI se tratan primero como JSON para las consultas. Los resultados de CLI son una matriz JSON o un diccionario. Las matrices son secuencias de objetos que se pueden indexar y los diccionarios son objetos desordenados a los que se accede con claves. Los comandos que _pueden_devolver más de un objeto devuelven una matriz y los comandos que _siempre_ devuelven _únicamente_ un solo objeto devuelven un diccionario.

## <a name="get-properties-in-a-dictionary"></a>Obtención de propiedades en un diccionario

Al trabajar con los resultados del diccionario, puede acceder a las propiedades del nivel superior con solo la clave. El carácter `.` (__subexpresión__) se utiliza para acceder a las propiedades de los diccionarios anidados. Antes de introducir consultas, eche un vistazo a la salida no modificada del comando `az vm show`:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM -o json
```

El comando dará como resultado un diccionario. Se ha omitido parte del contenido.

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

El siguiente comando obtiene las claves públicas SSH autorizadas para conectarse a la máquina virtual mediante la adición de una consulta:

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

Para obtener más de una propiedad, coloque las expresiones entre corchetes `[ ]` (una __lista de selección múltiple__) como una lista separada por comas. Para obtener el nombre de la máquina virtual, el usuario administrador y la clave SSH de una sola vez, utilice el comando:

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

Estos valores se muestran en la matriz de resultados en el orden en que se proporcionaron en la consulta. Dado que el resultado es una matriz, no hay claves asociadas a los resultados.

## <a name="get-a-single-value"></a>Obtener un solo valor

Un caso común es si necesita obtener solo _un_ valor de un comando de la CLI, como un identificador de recurso de Azure, un nombre de recurso, un nombre de usuario o una contraseña. En ese caso, se suele querer también almacenar el valor en una variable de entorno local. Para obtener una sola propiedad, primero debe asegurarse de que está obteniendo solo una propiedad de la consulta. Modificamos el ejemplo anterior para obtener solo el nombre de usuario del administrador:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json
```

```JSON
"azureuser"
```

Esto parece un valor único válido, pero tenga en cuenta que los `"` caracteres se devuelven como parte de la salida. Esto indica que el objeto es una cadena JSON. Es importante tener en cuenta que al asignar este valor directamente como salida del comando a una variable de entorno, el Shell podría __no__ interpretar las comillas:

```bash
USER=$(az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o json)
echo $USER
```

```output
"azureuser"
```

Es casi seguro que este no es el comportamiento que desea. En este caso, desea utilizar un formato de salida que no incluya los valores devueltos entre comillas con la información del tipo. La mejor opción de salida que la CLI ofrece con este fin `tsv`, valores separados por tabulaciones. En concreto, al recuperar un valor que es un valor solo (no diccionario o una lista), es seguro que la salida `tsv` no estará entre comillas.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'osProfile.adminUsername' -o tsv
```

```output
azureuser
```

Para más información sobre el formato de salida de `tsv`, consulte [Formatos de salida: formato de salida TSV](format-output-azure-cli.md#tsv-output-format).

## <a name="rename-properties-in-a-query"></a>Cambio del nombre de las propiedades en una consulta

Para obtener un diccionario en lugar de una matriz al consultar valores múltiples, utilice el operador `{ }` (__hash de selección múltiple__).
El formato de un hash de selección múltiple es `{displayName:JMESPathExpression, ...}`.
`displayName` será la cadena que se muestra en la salida y `JMESPathExpression` es la expresión JMESPath que se va a evaluar. Modificación del ejemplo de la última sección mediante el cambio de la lista de selección múltiple a un hash:

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

## <a name="get-properties-in-an-array"></a>Obtención de propiedades en una matriz

Una matriz no tiene propiedades propias, pero se puede indexar. Esta característica se muestra en el último ejemplo con la expresión `publicKeys[0]`, que obtiene el primer elemento de la matriz `publicKeys`. No hay garantía de que la salida de la CLI esté ordenada, así que evite utilizar la indexación a menos que esté seguro del orden o no le importe el elemento que se obtenga. Para acceder a las propiedades de los elementos de una matriz, se realiza una de dos operaciones: _simplificación_  y _filtrado_. En esta sección se explica cómo simplificar una matriz.

La simplificación de una matriz se realiza con el operador de JMESPath `[]`. Todas las expresiones después del operador `[]` se aplican a cada elemento de la matriz actual.
Si `[]` aparece al principio de la consulta, aplana el resultado del comando de la CLI. Los resultados de `az vm list` pueden inspeccionarse con esta característica.
Para obtener el nombre, el sistema operativo y el nombre del administrador de cada máquina virtual en un grupo de recursos:

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

Cuando se combina con el formato de salida `--output table`, los nombres de columna coinciden con el valor `displayKey` del hash de selección múltiple:

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
> Determinadas claves se filtran y no se imprimen en la vista de tabla. Estas claves son `id`, `type` y `etag`. Para ver estos valores, puede cambiar el nombre de la clave en un hash de selección múltiple.
>
> ```azurecli-interactive
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

Se puede simplificar cualquier matriz, no solo el resultado de nivel superior devuelto por el comando. En la última sección, se utilizó la expresión `osProfile.linuxConfiguration.ssh.publicKeys[0].keyData` para obtener la clave pública SSH para iniciar sesión. Para obtener _cada_ clave pública SSH, la expresión podría escribirse como `osProfile.linuxConfiguration.ssh.publicKeys[].keyData`.
Esta expresión de consulta simplifica la matriz `osProfile.linuxConfiguration.ssh.publicKeys` y, después, se ejecuta la expresión `keyData` en cada elemento:

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

## <a name="filter-arrays"></a>Filtrado de matrices

La otra operación utilizada para obtener datos de una matriz es el _filtrado_. El filtrado se realiza con el operador de JMESPath `[?...]`.
Este operador toma un predicado como su contenido. Un predicado es cualquier declaración que se puede evaluar como `true` o `false`. En la salida se incluyen las expresiones en las que el predicado se evalúa a `true`.

JMESPath ofrece la comparación estándar y los operadores lógicos. Estos incluyen `<`, `<=`, `>`, `>=`, `==` y `!=`.
JMESPath también admite la lógica y (`&&`) o (`||`) y no (`!`). Las expresiones se pueden agrupar entre paréntesis, lo que permite expresiones de predicados más complejas. Para obtener todos los detalles sobre predicados y operaciones lógicas, consulte la [especificación de JMESPath](http://jmespath.org/specification.html).

En la última sección, simplificamos una matriz para obtener la lista completa de todas las máquinas virtuales de un grupo de recursos. Mediante el uso de filtros, esta salida puede restringirse solo a las máquinas virtuales Linux:

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
> En JMESPath, las cadenas siempre están rodeadas de comillas simples (`'`). Si utiliza comillas dobles como parte de una cadena en un predicado de filtro, obtendrá una salida vacía.

JMESPath también tiene funciones integradas que pueden ayudar con el filtrado. Una de estas funciones es `contains(string, substring)`, que comprueba si una cadena contiene una subcadena. Las expresiones se evalúan antes de llamar a la función, por lo que el primer argumento puede ser una expresión completa de JMESPath. En el siguiente ejemplo se encuentran todas las máquinas virtuales que utilizan almacenamiento SSD para su disco de sistema operativo:

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

Esta consulta es un poco larga. La clave `storageProfile.osDisk.managedDisk.storageAccountType` se menciona dos veces y se vuelve a cambiar en la salida. Una manera de acortarlo es aplicar el filtro después de la simplificación y selección de los datos.

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

En el caso de matrices grandes, puede ser más rápido aplicar el filtro antes de seleccionar los datos.

Consulte la [especificación de JMESPath - Funciones integradas](http://jmespath.org/specification.html#built-in-functions) para ver la lista completa de funciones.

## <a name="change-output"></a>Cambio de la salida

Las funciones JMESPath también tienen otro propósito, que es trabajar sobre los resultados de una consulta. Cualquier función que devuelva un valor no booleano cambia el resultado de una expresión.
Por ejemplo, puede ordenar los datos por un valor de propiedad con `sort_by(array, &sort_expression)`. JMESPath utiliza un operador especial, `&`, para expresiones que deben evaluarse posteriormente como parte de una función. En el ejemplo siguiente se muestra cómo ordenar una lista de máquinas virtuales por el tamaño del disco del sistema operativo:

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

Consulte la [especificación de JMESPath - Funciones integradas](http://jmespath.org/specification.html#built-in-functions) para ver la lista completa de funciones.

## <a name="experiment-with-queries-interactively"></a>Experimentación con las consultas de forma interactiva

Para empezar a experimentar con JMESPath, el paquete [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) de Python ofrece un entorno interactivo para trabajar con las consultas. Los datos se canalizan como entrada y, después, se escriben las consultas y se ejecutan en el editor.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
