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
ms.locfileid: "34305985"
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Formatos de salida de los comandos de la CLI de Azure 2.0

La CLI de Azure 2.0 usa json como su opción de salida predeterminada, pero ofrece varias formas de dar formato a la salida de cualquier comando.  Use el parámetro `--output` (o `--out` o `-o`) para dar formato a la salida del comando con uno de los tipos de salida que se indican en la tabla siguiente:

--output | DESCRIPCIÓN
---------|-------------------------------
`json`   | Cadena JSON. Esta es la configuración predeterminada.
`jsonc`  | JSON con colores.
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

## <a name="table-output-format"></a>Formato de salida de tabla

El formato de salida `table` proporciona una salida con formato de filas y columnas de datos intercalados, lo que facilita la lectura y la búsqueda. Los objetos anidados no se incluyen en la salida de tabla, pero se pueden filtrar como parte de una consulta. Algunos campos también se omiten en la tabla de datos, por lo que este formato es adecuado cuando se desea una revisión rápida de los datos con posibilidad de que el usuario realice búsquedas.

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
> Determinadas claves se filtran y no se imprimen en la vista de tabla. Se trata de `id`, `type` y `etag`. Si necesita ver estos datos en la salida, puede usar la característica de reentrada de claves de JMESPath para cambiar el nombre de la clave y evitar el filtrado.
>
> ```azurecli
> az vm list --query "[].{objectID:id}" -o table
> ```

Para más información sobre el uso de consultas para filtrar los datos, consulte [Uso de consultas JMESPath con la CLI de Azure 2.0](/cli/azure/query-azure-cli).

## <a name="tsv-output-format"></a>Formato de salida TSV

El formato de salida `tsv` devuelve valores separados por tabulaciones y nueva línea sin formato adicional, claves ni otros símbolos. Este formato facilita el consumo de la salida en otros comandos y herramientas que necesitan procesar el texto de alguna forma. Al igual que el formato `table`, la opción de salida `tsv` no imprime objetos anidados.

Mediante el ejemplo anterior con la opción `tsv` se genera un resultado separado por tabulaciones.

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

En el siguiente ejemplo se muestra cómo se puede canalizar la salida `tsv` a otros comandos en sistemas UNIX para extraer datos más específicos. El comando `grep` selecciona los elementos que tienen el texto "RGD" y el comando `cut` selecciona el octavo campo (separado por tabulaciones) para mostrar el nombre de la máquina virtual en la salida.

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