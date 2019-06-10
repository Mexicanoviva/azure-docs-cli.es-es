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
<span data-ttu-id="95181-101">Si no puede conectarse a un recurso externo debido a un servidor proxy, asegúrese de que ha configurado correctamente las variables `HTTP_PROXY` y `HTTPS_PROXY` en el shell.</span><span class="sxs-lookup"><span data-stu-id="95181-101">If you're unable to connect to an external resource due to a proxy, make sure that you've correctly set the `HTTP_PROXY` and `HTTPS_PROXY` variables in your shell.</span></span> <span data-ttu-id="95181-102">Deberá ponerse en contacto con el administrador del sistema para saber qué hosts y puertos se van a usar para estos servidores proxy.</span><span class="sxs-lookup"><span data-stu-id="95181-102">You will need to contact your system administrator to know what host(s) and port(s) to use for these proxies.</span></span>

<span data-ttu-id="95181-103">Estos valores se respetan en muchos programas de Linux, incluidos los que se usan en el proceso de instalación.</span><span class="sxs-lookup"><span data-stu-id="95181-103">These values are respected by many Linux programs, including those which are used in the install process.</span></span> <span data-ttu-id="95181-104">Para establecer estos valores:</span><span class="sxs-lookup"><span data-stu-id="95181-104">To set these values:</span></span>

```bash
# No auth
export HTTP_PROXY=http://[proxy]:[port]
export HTTPS_PROXY=https://[proxy]:[port]

# Basic auth
export HTTP_PROXY=http://[username]:[password]@[proxy]:[port]
export HTTPS_PROXY=https://[username]:[password]@[proxy]:[port]
```

> [!IMPORTANT]
> <span data-ttu-id="95181-105">Si está detrás de un servidor proxy, estas variables de Shell deben establecerse para conectarse a los servicios de Azure con la CLI.</span><span class="sxs-lookup"><span data-stu-id="95181-105">If you are behind a proxy, these shell variables must be set to connect to Azure services with the CLI.</span></span>
> <span data-ttu-id="95181-106">Si no utiliza autenticación básica, se recomienda exportar estas variables en su archivo `.bashrc`.</span><span class="sxs-lookup"><span data-stu-id="95181-106">If you are not using basic auth, it's recommended to export these variables in your `.bashrc` file.</span></span>
> <span data-ttu-id="95181-107">Siga siempre las directivas de seguridad de su empresa y los requisitos del administrador del sistema.</span><span class="sxs-lookup"><span data-stu-id="95181-107">Always follow your business' security policies and the requirements of your system administrator.</span></span>
