---
title: Instalación de la CLI clásica de Azure
description: Instalación de la CLI clásica de Azure para Mac, Linux y Windows con el objetivo de comenzar a utilizar los servicios de Azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/11/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 65bf8cdc4ee5d74a778d29cd96e51bad5dc6b22e
ms.sourcegitcommit: f40bd067ece4e6ec13e259782ed8db3e33b61a75
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/18/2018
ms.locfileid: "53593377"
---
# <a name="install-the-azure-classic-cli"></a>Instalación de la CLI clásica de Azure

> [!IMPORTANT]
> Este tema describe cómo instalar la CLI clásica de Azure. La CLI clásica está en desuso y solo debe usarse con el modelo de implementación clásico.
> Para todas las demás implementaciones, utilice [la CLI de Azure](/cli/azure).

Instale rápidamente la CLI clásica de Azure para utilizar un conjunto de comandos de código abierto basados en shell para crear y administrar recursos en Microsoft Azure. Tiene varias opciones para instalar estas herramientas multiplataforma en su equipo:

* **Paquete de npm**: ejecute npm (el administrador de paquetes para JavaScript) para instalar el paquete de la CLI clásica de Azure en su distribución de Linux o sistema operativo. Se requieren node.js y npm.
* **Instalador**: descargue un instalador para facilitar la instalación en Mac o Windows.
* **Contenedor de Docker**: empiece a usar la CLI clásica en un contenedor de Docker listo para ejecutarse. Requiere un host de Docker.

Si desea obtener más opciones y los antecedentes, consulte el repositorio del proyecto en [GitHub](https://github.com/azure/azure-xplat-cli).

Una vez que instale la CLI clásica de Azure, conéctese con `azure login` y ejecute los comandos `azure` desde la interfaz de la línea de comandos (Bash, Terminal, símbolo del sistema, etc.) para trabajar con los recursos de Azure.

## <a name="option-1-install-an-npm-package"></a>Opción 1: Instalación de un paquete de NPM

Para instalar la CLI clásica desde un paquete de npm, asegúrese de que ha descargado e instalado la versión [más reciente de Node.js y npm](https://nodejs.org/en/download/package-manager/). A continuación, ejecute `npm install` para instalar el paquete azure-cli:

```bash
npm install -g azure-cli
```

En distribuciones de Linux, es posible que tenga que usar `sudo` para ejecutar correctamente el comando `npm`, tal como se muestra a continuación:

```bash
sudo npm install -g azure-cli
```

> [!NOTE]
> Si necesita instalar o actualizar Node.js y npm en el sistema operativo, se recomienda instalar Node.js LTS versión 4.x o posterior. Si utiliza una versión anterior, podrían producirse errores de instalación.

Si lo prefiere, también puede descargar un archivo tar desde las [versiones de GitHub](https://github.com/Azure/azure-xplat-cli/releases). Después, instale el paquete de npm descargado de la siguiente manera (en las distribuciones de Linux podría tener que usar `sudo`):

```bash
npm install -g <path to downloaded tar file>
```

## <a name="option-2-use-an-installer"></a>Opción 2: Uso de un instalador

Si usa un equipo Mac o Windows, los instaladores DMG y MSI están disponibles en [versiones de GitHub](https://github.com/Azure/azure-xplat-cli/releases).

> [!TIP]
> En Windows, también puede descargar el [Instalador de plataforma web](https://go.microsoft.com/?linkid=9828653) para instalar la CLI clásica. Este instalador ofrece la opción de instalar SDK de Azure adicionales y herramientas de la línea de comandos.

## <a name="option-3-use-a-docker-container"></a>Opción 3: Uso de un contenedor Docker

Si ha configurado el equipo como un host de [Docker](https://docs.docker.com/engine/understanding-docker/), puede ejecutar la CLI clásica de Azure en un contenedor de Docker. Ejecute el comando siguiente (en las distribuciones de Linux, es posible que tenga que usar `sudo`):

```bash
docker run -it microsoft/azure-cli:0.10.17
```

## <a name="run-azure-classic-cli-commands"></a>Ejecución de los comandos de la CLI clásica de Azure

Una vez instalada la CLI clásica de Azure, ejecute el comando `azure` desde la interfaz de usuario de la línea de comandos (Bash, Terminal, símbolo del sistema, etc.). Por ejemplo, si desea ejecutar el comando help, escriba lo siguiente:

```azurecli-interactive
azure help
```

> [!NOTE]
> En algunas distribuciones de Linux, puede recibir un error similar al `/usr/bin/env: ‘node’: No such file or directory`. Este error procede de las instalaciones recientes de Node.js que se instala en /usr/bin/nodejs. Para corregirlo, cree un vínculo simbólico a /usr/bin/node, para lo que debe ejecutar este comando:

```bash
sudo ln -s /usr/bin/nodejs /usr/bin/node
```

Para saber qué versión de la CLI clásica de Azure se ha instalado, escriba lo siguiente:

```azurecli-interactive
azure --version
```

> [!NOTE]
> La primera vez que usa la CLI clásica de Azure, verá un mensaje en el que se le pregunta si quiere permitir que Microsoft recopile información de uso. La participación es voluntaria. Si elige participar, puede dejar de hacerlo cuando desee mediante la ejecución de `azure telemetry --disable`. Para habilitar la participación en cualquier momento, ejecute `azure telemetry --enable`.

## <a name="update-the-classic-cli"></a>Actualización de la CLI clásica

Microsoft puede liberar versiones actualizadas de la CLI clásica de Azure. Vuelva a instalar la CLI clásica mediante el programa de instalación para su sistema operativo o ejecute el contenedor de Docker más reciente. O bien, si tiene las versiones de Node.js y npm más recientes instaladas, escriba lo siguiente para efectuar la actualización (en las distribuciones de Linux, es posible que necesite utilizar `sudo`).

```bash
npm update -g azure-cli
```

## <a name="enable-tab-completion"></a>Habilitación de la función de autocompletar

La función de autocompletar de los comandos de la CLI clásica es compatible con Mac y Linux.

Para habilitarla en zsh, ejecute el siguiente código:

```bash
echo '. <(azure --completion)' >> .zshrc
```

Para habilitarla en Bash, ejecute el siguiente código:

```bash
azure --completion >> ~/azure.completion.sh
echo 'source ~/azure.completion.sh' >> ~/.bash_profile
```

## <a name="next-steps"></a>Pasos siguientes

* Para más información acerca de la CLI clásica de Azure, descargar el código fuente, informar sobre problemas o colaborar con el proyecto, visite el [Repositorio de GitHub para la CLI clásica de Azure](https://github.com/azure/azure-xplat-cli).
