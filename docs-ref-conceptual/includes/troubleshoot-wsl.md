---
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 11/26/2018
ms.topic: include
ms.openlocfilehash: ee0b2b0c8c557aa54255f28429bb3a174c0e21a9
ms.sourcegitcommit: a8aac038e6ede0b1b352ca6163a04b61ff4eed5b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/28/2018
ms.locfileid: "52450350"
---
### <a name="cli-fails-to-install-or-run-on-windows-subsystem-for-linux"></a>Se produce un error en la CLI al instalar o ejecutar en el subsistema de Windows para Linux

Como el [subsistema de Windows para Linux (WSL)](/windows/wsl/about) es una capa de traducción de llamadas del sistema que se ejecuta en la plataforma Windows, es posible que experimente un error al intentar instalar o ejecutar en la CLI de Azure. La CLI se basa en algunas características que podrían producir un error en WSL. Si experimenta un error, independientemente de cómo instale la CLI, es muy probable que se trate de un problema de WSL y no del proceso de instalación de la CLI.

Para solucionar los problemas de instalación de WSL:

* Si puede, ejecute un proceso de instalación idéntico en una máquina Linux para ver si se realiza correctamente. Si es así, su problema seguramente está relacionado con WSL. Para iniciar una máquina virtual Linux en Azure, consulte [Creación de una máquina virtual Linux en Azure Portal](/azure/virtual-machines/linux/quick-create-portal).
* Asegúrese de que usa la versión más reciente de WSL. Para obtener la última versión, [actualice su instalación de Windows 10](https://support.microsoft.com/help/4027667/windows-10-update).
* Consulte los [problemas abiertos](https://github.com/Microsoft/WSL/issues) con WSL que pudieran resolver el problema.
  Suele haber sugerencias sobre cómo solucionar el problema o información sobre una versión donde se corregirá el problema.
* Si no hay ninguna incidencia abierta para su problema, [abra una incidencia nueva con WSL](https://github.com/Microsoft/WSL/issues/new) y asegúrese de incluir toda la información posible.

Si aún tiene problemas para instalar o ejecutar en WSL, considere la posibilidad de [instalar la CLI para Windows](../install-azure-cli-windows.md).
