---
title: Formatos de salida para la CLI de Azure 2.0
description: Use el comando --output para dar formato a la salida de los comandos de la CLI de Azure 2.0 en tablas, listas o json.
keywords: CLI de Azure 2.0, salida, formato, tabla, lista, json, Linux, Mac, Windows, OS X
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 02/27/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 74bdb727-481d-45f7-a44e-15d18dc55483
ms.openlocfilehash: d1440cc1e99ccddb18d23306cc0fcdb4b8babf14
ms.sourcegitcommit: 4fd631a58cf19c494162510d073fbbbdf0524d16
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2017
---
# <a name="output-formats-for-azure-cli-20-commands"></a>Formatos de salida de los comandos de la CLI de Azure 2.0

La CLI de Azure 2.0 usa json como su opción de salida predeterminada, pero ofrece varias formas de dar formato a la salida de cualquier comando.  Use el parámetro `--output` (o `--out` o `-o`) para dar formato a la salida del comando con uno de los tipos de salida que se indican en la tabla siguiente. 

--output | Descripción
---------|-------------------------------
`json`   | Cadena JSON. `json` es el valor predeterminado.
`jsonc`  | Cadena json con colores.
`table`  | Tabla con encabezados de columna.
`tsv`    | Valores separados por tabulaciones.

[!INCLUDE [cloud-shell-try-it.md](includes/cloud-shell-try-it.md)]

## <a name="using-the-json-option"></a>Uso de la opción json

En el ejemplo siguiente se muestra la lista de máquinas virtuales de sus suscripciones en el formato json predeterminado.

```azurecli-interactive
az vm list --output json
```

Los resultados están en este formulario (solo se muestran resultados parciales por motivos de brevedad).

```json
[
  {
    "availabilitySet": null,
    "diagnosticsProfile": null,
    "hardwareProfile": {
      "vmSize": "Standard_DS1"
    },
    "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010",
    "instanceView": null,
    "licenseType": null,
    "location": "westus",
    "name": "DemoVM010",
    "networkProfile": {
      "networkInterfaces": [
        {
          "id": "/subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/demorg1/providers/Microsoft.Network/networkInterfaces/DemoVM010VMNic",
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
 
## <a name="using-the-table-option"></a>Uso de la opción de tabla

La opción de tabla proporciona una forma sencilla de leer un conjunto de salidas, pero tenga en cuenta que los objetos anidados no se incluyen en la salida con el sencillo comando `--output table`, a diferencia del anterior ejemplo .json.  El uso del mismo ejemplo con formato de salida 'table' proporciona una lista protegida de los valores de propiedad más comunes.

```azurecli-interactive
az vm list --out table
```

```
Name         ResourceGroup    Location
-----------  ---------------  ----------
DemoVM010    DEMORG1          westus
demovm212    DEMORG1          westus
demovm213    DEMORG1          westus
KBDemo001VM  RGDEMO001        westus
KBDemo020    RGDEMO001        westus
```

Puede usar el parámetro `--query` para personalizar las propiedades y las columnas que desea mostrar en la salida de la lista. En el ejemplo siguiente se muestra cómo seleccionar el nombre de máquina virtual y el nombre del grupo de recursos en el comando `list`.

```azurecli-interactive
az vm list --query "[].{ resource: resourceGroup, name: name }" -o table
```

```
Resource    Name
----------  -----------
DEMORG1     DemoVM010
DEMORG1     demovm212
DEMORG1     demovm213
RGDEMO001   KBDemo001VM
RGDEMO001   KBDemo020
```

## <a name="using-the-tsv-option"></a>Uso de la opción tsv

El formato de salida "tsv" devuelve una salida sencilla basada en texto y separada por tabulaciones sin encabezados ni guiones. Este formato facilita el consumo de la salida en otros comandos y herramientas que necesitan procesar el texto de alguna forma. Mediante el ejemplo anterior con la opción `tsv` se genera un resultado separado por tabulaciones.

```azurecli-interactive
az vm list --out tsv
```

```
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/DemoVM010    None    None    westus    DemoVM010            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    cbd56d9b-9340-44bc-a722-25f15b578444
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm212    None    None    westus    demovm212            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    4bdac85d-c2f7-410f-9907-ca7921d930b4
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/DEMORG1/providers/Microsoft.Compute/virtualMachines/demovm213    None    None    westus    demovm213            None    Succeeded    DEMORG1    None            Microsoft.Compute/virtualMachines    2131c664-221a-4b7f-9653-f6d542fbfa34
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo001VM    None    None    westus    KBDemo001VM            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachines    14e74761-c17e-4530-a7be-9e4ff06ea74b
None    None        /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/RGDEMO001/providers/Microsoft.Compute/virtualMachines/KBDemo02None    None    westus    KBDemo020            None    Succeeded    RGDEMO001    None            Microsoft.Compute/virtualMachinesed36baa9-9b80-48a8-b4a9-854c7a858ece
```

En el siguiente ejemplo se muestra cómo la salida `tsv` se puede canalizar a comandos como `grep` y `cut` para analizar aún más los valores específicos de la salida `list`. El comando `grep` solo selecciona los elementos que tienen el texto "RGD" en ellos y el comando `cut` selecciona solo el valor del octavo campo (separado por tabulaciones) para mostrar en la salida.

```azurecli
az vm list --out tsv | grep RGD | cut -f8
```

```
KBDemo001VM
KBDemo020
```

## <a name="setting-the-default-output-format"></a>Establecimiento del formato de salida predeterminado

Puede usar el comando `az configure` para configurar el entorno o establecer preferencias como la configuración predeterminada de los formatos de salida. Para un uso común, el valor predeterminado del formato de salida más fácil es el formato "table". Seleccione **3** cuando se le soliciten las opciones de formato de salida. 

```
What default output format would you like?
 [1] json - JSON formatted output that most closely matches API responses
 [2] jsonc - Colored JSON formatted output that most closely matches API responses
 [3] table - Human-readable output format
 [4] tsv - Tab and Newline delimited, great for GREP, AWK, etc.
Please enter a choice [3]: 
```