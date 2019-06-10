---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 05/28/2019
ms.topic: include
ms.prod: azure
ms.technology: azure-cli
ms.openlocfilehash: 676f33377a4e7122941bc789c51465b7f34aa1d3
ms.sourcegitcommit: 08043c47d3ccf23522b91e6bba3932e312c04c7f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2019
ms.locfileid: "66516264"
---
Si no puede conectarse a un recurso externo debido a un servidor proxy, asegúrese de que ha configurado correctamente las variables `HTTP_PROXY` y `HTTPS_PROXY` en el shell. Deberá ponerse en contacto con el administrador del sistema para saber qué hosts y puertos se van a usar para estos servidores proxy.

Estos valores se respetan en muchos programas de Linux, incluidos los que se usan en el proceso de instalación. Para establecer estos valores:

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> Si está detrás de un servidor proxy, estas variables de Shell deben establecerse para conectarse a los servicios de Azure con la CLI.
> Si no utiliza autenticación básica, se recomienda exportar estas variables en su archivo `.bashrc`.
> Siga siempre las directivas de seguridad de su empresa y los requisitos del administrador del sistema.
