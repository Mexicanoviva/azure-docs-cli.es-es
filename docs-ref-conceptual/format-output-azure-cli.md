---
title: Formatos de salida para la CLI de Azure 2.0
description: Obtenga información acerca de cómo dar formato a la salida de los comandos de la CLI de Azure 2.0 como tablas, listas o código JSON.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/07/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 1430d817a7e6c10a8f8021cf9d763f62d560ba71
ms.sourcegitcommit: 8318ce761c279afa4cd45a81a58d83fc38c616bc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/13/2018
ms.locfileid: "45561565"
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Formatos de salida de los comandos de la CLI de Azure 2.0

La CLI de Azure 2.0 usa JSON como formato de salida predeterminado, pero ofrece otros formatos.  Use el parámetro `--output` (`--out` o `-o`) para dar formato a la salida de la CLI. Los valores de argumento y los tipos de salida son:

--output | DESCRIPCIÓN
---------|-------------------------------
`json`   | Cadena JSON. Esta es la configuración predeterminada.
`jsonc`  | JSON con colores.
`yaml`   | YAML, una alternativa a JSON legible por máquina.
`table`  | Tabla ASCII con claves como encabezados de columna.
`tsv`    | Valores separados por tabulaciones, sin claves

## <a name="json-output-format"></a>Formato de salida JSON

En el ejemplo siguiente se muestra la lista de máquinas virtuales de sus suscripciones en el formato json predeterminado.

```azurecli-interactive
az vm list --output json
```

La salida siguiente tiene algunos campos que se omiten para mayor brevedad y se ha reemplazado la información de identificación.

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

## <a name="yaml-output-format"></a>Formato de salida YAML

El formato `yaml` imprime la salida como [YAML](http://yaml.org/), un formato de serialización de datos de texto sin formato. YAML suele ser más fácil de leer que JSON y se corresponde fácilmente con ese formato. Algunas aplicaciones y los comandos de la CLI aceptan YAML como entrada de configuración, en lugar de JSON.

```azurecli-interactive
az vm list --out yaml
```

La salida siguiente tiene algunos campos que se omiten para mayor brevedad y se ha reemplazado la información de identificación.

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

## <a name="table-output-format"></a>Formato de salida de tabla

El formato `table` imprime la salida como una tabla ASCII, lo que facilita la lectura y la búsqueda. Los objetos anidados no se incluyen en la tabla de salida, pero se pueden filtrar como parte de una consulta. Algunos campos no se incluyen en la tabla, por lo que este formato es adecuado cuando se desea una revisión rápida de los datos con posibilidad de que el usuario realice búsquedas.

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

Puede usar el parámetro `--query` para personalizar las propiedades y las columnas que desea mostrar en la salida de la lista. En el ejemplo siguiente se muestra cómo seleccionar el nombre de máquina virtual y el nombre del grupo de recursos en el comando `list`.

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
> Algunas claves no se imprimen en la vista de tabla de forma predeterminada. Se trata de `id`, `type` y `etag`. Si necesita ver estos datos en la salida, puede usar la característica de reentrada de claves de JMESPath para cambiar el nombre de la clave y evitar el filtrado.
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

Para más información sobre el uso de consultas para filtrar los datos, consulte [Uso de consultas JMESPath con la CLI de Azure 2.0](/cli/azure/query-azure-cli).

## <a name="tsv-output-format"></a>Formato de salida TSV

El formato de salida `tsv` devuelve valores separados por tabulaciones y nueva línea sin formato adicional, claves ni otros símbolos. Este formato facilita el consumo de la salida en otros comandos y herramientas que necesitan procesar el texto de alguna forma. Al igual que el formato `table`, `tsv` no imprime objetos anidados.

Mediante el ejemplo anterior con la opción `tsv` se genera un resultado separado por tabulaciones.

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

El ejemplo siguiente muestra cómo se puede canalizar la salida `tsv` a otros comandos en Bash. `grep` selecciona los elementos que tienen el texto "RGD" y el comando `cut` selecciona el octavo campo para mostrar el nombre de la máquina virtual en la salida.

```bash
az vm list --out tsv | grep RGD | cut -f8
```

```output
KBDemo001VM
KBDemo020
```

Para fines de procesamiento de campos separados por tabulaciones, los valores están en el mismo orden que aparecen en el objeto JSON impreso. Se garantiza que este orden sea coherente entre las distintas ejecuciones del comando.

## <a name="set-the-default-output-format"></a>Establecimiento del formato de salida predeterminado

Puede usar el comando interactivo `az configure` para configurar el entorno y establecer la configuración predeterminada de los formatos de salida. El formato de salida predeterminado es `json`.

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

Para más información sobre cómo configurar el entorno, consulte [Configuración de la CLI de Azure 2.0](/cli/azure/azure-cli-configuration).