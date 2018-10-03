---
title: Resultados del comando de consulta con la CLI de Azure
description: Obtenga información acerca de cómo realizar consultas JMESPath con la salida de los comandos de la CLI de Azure.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 4522242952e5d257449c9c593885c62de2f56d0f
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2018
ms.locfileid: "47178038"
---
# <a name="use-jmespath-queries-with-azure-cli"></a>Uso de consultas JMESPath con la CLI de Azure 

La CLI de Azure utiliza el argumento `--query` para ejecutar una [consulta JMESPath](http://jmespath.org) en los resultados de los comandos. JMESPath es un lenguaje de consulta para JSON que ofrece la posibilidad de seleccionar y presentar datos de la salida de la CLI. Estas consultas se ejecutan en la salida JSON antes de realizar cualquier otro formato de presentación.

El argumento `--query` es compatible con todos los comandos de la CLI de Azure. Los ejemplos de este artículo cubren los casos de uso más comunes y muestran cómo usar las características de JMESPath.

## <a name="work-with-dictionary-output"></a>Trabajar con la salida de diccionario

Los comandos que devuelven un diccionario JSON se pueden explorar por los nombres de clave por sí mismos. Las rutas de acceso de las claves utilizan el carácter `.` como separador. En el ejemplo siguiente se extrae una lista de las claves SSH públicas que pueden conectarse a una máquina virtual Linux:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query osProfile.linuxConfiguration.ssh.publicKeys
```

Si hay varios valores, se pueden colocar en una matriz ordenada. En el ejemplo siguiente se muestra cómo recuperar el nombre de oferta de la imagen de Azure y el tamaño del disco del sistema operativo:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.[imageReference.offer, osDisk.diskSizeGb]'
```

```json
[
  "UbuntuServer",
  30
]
```

Si desea que las claves estén presentes en la salida, puede usar una sintaxis de diccionario alternativa.  La selección de elementos en un diccionario utiliza el formato `{displayKey:keyPath, ...}` para filtrar según la expresión JMESPath `keyPath`. En los valores de salida, los pares clave-valor se cambian a `{displayKey: value}`. En el ejemplo siguiente se toma la consulta del último ejemplo, que resulta más clara asignando claves a la salida:

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'storageProfile.{image:imageReference.offer, diskSize:osDisk.diskSizeGb}'
```

```json
{
  "diskSize": 30,
  "image": "UbuntuServer"
}
```

Al mostrar información con el formato de salida `table`, la presentación del diccionario permite establecer sus propios encabezados de columna. Para más información sobre los formatos de salida, consulte [Formatos de salida de los comandos de la CLI de Azure](/cli/azure/format-output-azure-cli).

> [!NOTE]
> Determinadas claves se filtran y no se imprimen en la vista de tabla. Estas claves son `id`, `type` y `etag`. Si necesita mostrar esta información, puede cambiar el nombre de la clave y evitar el filtrado.
>
> ```azurecli
> az vm show -g QueryDemo -n TestVM --query "{objectID:id}" -o table
> ```

## <a name="work-with-list-output"></a>Trabajar con la salida de lista

Los comandos de la CLI que pueden devolver más de un valor devuelven una matriz. A los elementos de la matriz se accede por el índice y no se pueden devolver en el mismo orden cada vez. Para consultar todos los elementos de una matriz a la vez, puede aplanarla con el operador `[]`. El operador se escribe después de la matriz o como el primer elemento de una expresión. Para aplanar una matriz, se ejecuta la consulta posterior en cada elemento de la matriz.

En el ejemplo siguiente se imprime el nombre y el sistema operativo que se ejecuta en cada máquina virtual de un grupo de recursos.

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

También se pueden aplanar las matrices que forman parte de una ruta de acceso de clave. La siguiente consulta obtiene los identificadores de objeto de Azure de las NIC a las que está conectada una máquina virtual.

```azurecli-interactive
az vm show -g QueryDemo -n TestVM --query 'networkProfile.networkInterfaces[].id'
```

## <a name="filter-array-output-with-predicates"></a>Filtrado de la salida de la matriz con predicados

JMESPath ofrece [expresiones de filtro](http://jmespath.org/specification.html#filterexpressions) para filtrar los datos mostrados. Estas expresiones son eficaces, especialmente cuando se combinan con las [funciones integradas de JMESPath](http://jmespath.org/specification.html#built-in-functions) para realizar coincidencias parciales o manipular los datos en un formato estándar. Las expresiones de filtro solo funcionan en datos de matriz y, cuando se utilizan en cualquier otra situación, devuelven el valor `null`. Por ejemplo, puede tomar la salida de comandos como `vm list` y filtrarla para buscar tipos específicos de máquinas virtuales. En el ejemplo siguiente se amplía el anterior filtrando el tipo de máquina virtual para capturar solo máquinas virtuales Windows e imprimir su nombre.

```azurecli-interactive
az vm list --query '[?osProfile.windowsConfiguration!=null].name'
```

```json
[
  "WinServ"
]
```

## <a name="experiment-with-queries-interactively"></a>Experimentación con las consultas de forma interactiva

Para empezar a aprender JMESPath, el paquete [JMESPath-terminal](https://github.com/jmespath/jmespath.terminal) de Python ofrece un entorno interactivo para experimentar con las consultas. Los datos se canalizan como entrada y, a continuación, se escriben consultas en el programa y se puede editar para extraer los datos.

```bash
pip install jmespath-terminal
az vm list --output json | jpterm
```
