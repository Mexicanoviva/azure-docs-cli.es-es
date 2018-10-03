---
title: Modo interactivo de la CLI de Azure
description: Use la CLI de Azure en modo interactivo.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 09/09/2018
ms.topic: conceptual
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 2a07b77873f4b0439e494a96243b0298f7d77b8d
ms.sourcegitcommit: c4462456dfb17993f098d47c37bc19f4d78b8179
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2018
ms.locfileid: "47177698"
---
# <a name="azure-cli-interactive-mode"></a><span data-ttu-id="99337-103">Modo interactivo de la CLI de Azure</span><span class="sxs-lookup"><span data-stu-id="99337-103">Azure CLI interactive mode</span></span>

<span data-ttu-id="99337-104">Puede usar la CLI de Azure en modo interactivo mediante la ejecución del comando `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="99337-104">You can use Azure CLI in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="99337-105">Este modo abre un shell interactivo con función autocompletar, descripciones de los comandos y ejemplos.</span><span class="sxs-lookup"><span data-stu-id="99337-105">This mode places you in an interactive shell with auto-completion, command descriptions, and examples.</span></span>

![modo interactivo](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="99337-107">Aquí no se va a usar el estilo predeterminado, ya que no se lee sobre un fondo negro.</span><span class="sxs-lookup"><span data-stu-id="99337-107">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="99337-108">Si aún no ha iniciado sesión en la cuenta, use el comando `login`.</span><span class="sxs-lookup"><span data-stu-id="99337-108">If you're not already signed in to your account, use the `login` command.</span></span>

## <a name="configure"></a><span data-ttu-id="99337-109">Configuración</span><span class="sxs-lookup"><span data-stu-id="99337-109">Configure</span></span>

<span data-ttu-id="99337-110">El modo interactivo muestra de manera opcional descripciones de comandos, descripciones de parámetros y ejemplos de comandos.</span><span class="sxs-lookup"><span data-stu-id="99337-110">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="99337-111">Active o desactive las descripciones y los ejemplos con `F1`.</span><span class="sxs-lookup"><span data-stu-id="99337-111">Turn descriptions and examples on or off using `F1`.</span></span>

![descripciones y ejemplos](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="99337-113">Puede activar o desactivar la visualización de los parámetros predeterminados mediante `F2`.</span><span class="sxs-lookup"><span data-stu-id="99337-113">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![parámetros predeterminados](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="99337-115">`F3` alterna la visualización de algunos gestos clave.</span><span class="sxs-lookup"><span data-stu-id="99337-115">`F3` toggles the display of some key gestures.</span></span>

![gestos](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="99337-117">Ámbito</span><span class="sxs-lookup"><span data-stu-id="99337-117">Scope</span></span>

<span data-ttu-id="99337-118">Puede establecer el ámbito del modo interactivo a un grupo de comandos específico, como `vm` o `vm image`.</span><span class="sxs-lookup"><span data-stu-id="99337-118">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="99337-119">Al hacerlo, todos los comandos se interpretan en ese ámbito.</span><span class="sxs-lookup"><span data-stu-id="99337-119">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="99337-120">Se trata de un método abreviado ideal si va a realizar todo el trabajo en dicho grupo de comandos.</span><span class="sxs-lookup"><span data-stu-id="99337-120">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="99337-121">En lugar de escribir estos comandos:</span><span class="sxs-lookup"><span data-stu-id="99337-121">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="99337-122">Puede definir el ámbito del grupo de comandos de máquina virtual y escribir estos comandos:</span><span class="sxs-lookup"><span data-stu-id="99337-122">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="99337-123">También puede definir el ámbito en grupos de comandos de nivel inferior.</span><span class="sxs-lookup"><span data-stu-id="99337-123">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="99337-124">Podría definir el ámbito en `vm image` mediante `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="99337-124">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="99337-125">En este caso, puesto que el ámbito ya está definido en `vm`, se usaría `%%image`.</span><span class="sxs-lookup"><span data-stu-id="99337-125">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="99337-126">En ese punto, se puede devolver el ámbito a `vm` mediante `%%..`, o bien se puede definir el ámbito en la raíz solo con `%%`.</span><span class="sxs-lookup"><span data-stu-id="99337-126">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="99337-127">Consultar</span><span class="sxs-lookup"><span data-stu-id="99337-127">Query</span></span>

<span data-ttu-id="99337-128">Puede ejecutar una consulta JMESPath en los resultados del último comando ejecutado.</span><span class="sxs-lookup"><span data-stu-id="99337-128">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="99337-129">Por ejemplo, después de crear una máquina virtual, puede asegurarse de que se ha aprovisionado totalmente.</span><span class="sxs-lookup"><span data-stu-id="99337-129">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```output
[
  "Creating"
]
```

<span data-ttu-id="99337-130">Para más información sobre cómo consultar los resultados de los comandos, examine [Consulta de resultados de los comandos con la CLI de Azure](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="99337-130">To learn more about querying the results of your commands, see [Query command results with the Azure CLI](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="99337-131">Comandos de Bash</span><span class="sxs-lookup"><span data-stu-id="99337-131">Bash commands</span></span>

<span data-ttu-id="99337-132">Puede ejecutar comandos shell sin salir del modo interactivo mediante `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="99337-132">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="99337-133">Ejemplos</span><span class="sxs-lookup"><span data-stu-id="99337-133">Examples</span></span>

<span data-ttu-id="99337-134">Algunos comandos tienen una gran cantidad de ejemplos.</span><span class="sxs-lookup"><span data-stu-id="99337-134">Some commands have lots of examples.</span></span>
<span data-ttu-id="99337-135">Puede desplazarse a la siguiente página de ejemplos con `CTRL-N` y a la página anterior mediante `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="99337-135">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![ejemplos](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="99337-137">También puede ver un ejemplo concreto mediante `::#`.</span><span class="sxs-lookup"><span data-stu-id="99337-137">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
