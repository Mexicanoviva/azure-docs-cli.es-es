---
title: Modo interactivo de la CLI de Azure 2.0
description: Use la CLI de Azure 2.0 en modo interactivo.
keywords: CLI de Azure 2.0, modo interactivo
author: rloutlaw
ms.author: routlaw
manager: douge
ms.date: 04/06/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: 
ms.openlocfilehash: de6a366b84efa5475fd6146ff29c32e32dfe4672
ms.sourcegitcommit: 1791991b82e6ce8ad4a050cab1695e0c93734e08
ms.contentlocale: es-ES
ms.lasthandoff: 05/12/2017
---
# <a name="interactive-azure-cli-20"></a><span data-ttu-id="87a4b-104">CLI de Azure 2.0 interactiva</span><span class="sxs-lookup"><span data-stu-id="87a4b-104">Interactive Azure CLI 2.0</span></span>

<span data-ttu-id="87a4b-105">Puede usar la CLI de Azure 2.0 en modo interactivo mediante la ejecución del comando `az interactive`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-105">You can use Azure CLI 2.0 in interactive mode by running the `az interactive` command.</span></span>
<span data-ttu-id="87a4b-106">De esta forma, se le remite a un shell interactivo donde los comandos se completan automáticamente y donde puede acceder a las descripciones de los comandos y a sus parámetros y ejemplos de comandos.</span><span class="sxs-lookup"><span data-stu-id="87a4b-106">That places you in an interactive shell where your commands are auto-completed and you have access to descriptions of commands and their parameters and command examples.</span></span>

![modo interactivo](./media/interactive-azure-cli/webapp-create.png)

> [!NOTE]
> <span data-ttu-id="87a4b-108">Aquí no se va a usar el estilo predeterminado, ya que no se lee sobre un fondo negro.</span><span class="sxs-lookup"><span data-stu-id="87a4b-108">We're not using the default style here, which doesn't read as well on a black background.</span></span>

<span data-ttu-id="87a4b-109">Si aún no se ha registrado en la cuenta, use el comando `login` para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="87a4b-109">If you're not already logged in to your account, use the `login` command to do that.</span></span>

## <a name="configure"></a><span data-ttu-id="87a4b-110">Configuración</span><span class="sxs-lookup"><span data-stu-id="87a4b-110">Configure</span></span>

<span data-ttu-id="87a4b-111">El modo interactivo muestra de manera opcional descripciones de comandos, descripciones de parámetros y ejemplos de comandos.</span><span class="sxs-lookup"><span data-stu-id="87a4b-111">Interactive mode optionally displays command descriptions, parameter descriptions, and command examples.</span></span>
<span data-ttu-id="87a4b-112">Puede activar o desactivar las descripciones y los ejemplos mediante `F1`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-112">You can turn descriptions and examples on or off using `F1`.</span></span>

![descripciones y ejemplos](./media/interactive-azure-cli/descriptions-and-examples.png)

<span data-ttu-id="87a4b-114">Puede activar o desactivar la visualización de los parámetros predeterminados mediante `F2`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-114">You can turn the display of parameter defaults on or off using `F2`.</span></span>

![parámetros predeterminados](./media/interactive-azure-cli/defaults.png)

<span data-ttu-id="87a4b-116">`F3` alterna la visualización de algunos gestos clave.</span><span class="sxs-lookup"><span data-stu-id="87a4b-116">`F3` toggles the display of some key gestures.</span></span>

![gestos](./media/interactive-azure-cli/gestures.png)

## <a name="scope"></a><span data-ttu-id="87a4b-118">Scope</span><span class="sxs-lookup"><span data-stu-id="87a4b-118">Scope</span></span>

<span data-ttu-id="87a4b-119">Puede establecer el ámbito del modo interactivo a un grupo de comandos específico, como `vm` o `vm image`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-119">You can scope your interactive mode to a specific command group like `vm` or `vm image`.</span></span>
<span data-ttu-id="87a4b-120">Al hacerlo, todos los comandos se interpretan en ese ámbito.</span><span class="sxs-lookup"><span data-stu-id="87a4b-120">When you do, all commands are interpreted in that scope.</span></span>
<span data-ttu-id="87a4b-121">Se trata de un método abreviado ideal si va a realizar todo el trabajo en dicho grupo de comandos.</span><span class="sxs-lookup"><span data-stu-id="87a4b-121">It's a great shorthand if you're doing all your work in that command group.</span></span>

<span data-ttu-id="87a4b-122">En lugar de escribir estos comandos:</span><span class="sxs-lookup"><span data-stu-id="87a4b-122">Instead of typing these commands:</span></span>

```azurecli
az>> vm create -n myVM -g myRG --image UbuntuLTS
az>> vm list -o table
```

<span data-ttu-id="87a4b-123">Puede definir el ámbito del grupo de comandos de máquina virtual y escribir estos comandos:</span><span class="sxs-lookup"><span data-stu-id="87a4b-123">You can scope to the vm command group and type these commands:</span></span>

```azurecli
az>> %%vm
az vm>> create -n myVM -g myRG --image UbuntuLTS
az vm>>list -o table
```

<span data-ttu-id="87a4b-124">También puede definir el ámbito en grupos de comandos de nivel inferior.</span><span class="sxs-lookup"><span data-stu-id="87a4b-124">You can scope to lower-level command groups as well.</span></span>
<span data-ttu-id="87a4b-125">Podría definir el ámbito en `vm image` mediante `%%vm image`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-125">You could scope to `vm image` using `%%vm image`.</span></span>
<span data-ttu-id="87a4b-126">En este caso, puesto que el ámbito ya está definido en `vm`, se usaría `%%image`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-126">In this case, since we're already scoped to `vm`, we would use `%%image`.</span></span>

```azurecli
az vm>> %%image
az vm image>>
```

<span data-ttu-id="87a4b-127">En ese punto, se puede devolver el ámbito a `vm` mediante `%%..`, o bien se puede definir el ámbito en la raíz solo con `%%`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-127">At that point, we can pop the scope back up to `vm` using `%%..`, or we can scope to the root with just `%%`.</span></span>

```azurecli
az vm image>> %%
az>>
```

## <a name="query"></a><span data-ttu-id="87a4b-128">Consultar</span><span class="sxs-lookup"><span data-stu-id="87a4b-128">Query</span></span>

<span data-ttu-id="87a4b-129">Puede ejecutar una consulta JMESPath en los resultados del último comando ejecutado.</span><span class="sxs-lookup"><span data-stu-id="87a4b-129">You can execute a JMESPath query on the results of the last command that you executed.</span></span>
<span data-ttu-id="87a4b-130">Por ejemplo, después de crear una máquina virtual, puede asegurarse de que se ha aprovisionado totalmente.</span><span class="sxs-lookup"><span data-stu-id="87a4b-130">For example, after you create a VM, you can make sure it has fully provisioned.</span></span>

```azurecli
az>> vm create --name myVM --resource-group myRG --image UbuntuLTS --no-wait
az>> ? [*].provisioningState
```

```
[
  "Creating"
]
```

<span data-ttu-id="87a4b-131">Para más información sobre cómo consultar los resultados de los comandos, vea [Resultados de comandos de consulta con Azure 2.0](query-azure-cli.md).</span><span class="sxs-lookup"><span data-stu-id="87a4b-131">To learn more about querying the results of your commands, see [Query command results with Azure 2.0](query-azure-cli.md).</span></span>

## <a name="bash-commands"></a><span data-ttu-id="87a4b-132">Comandos de Bash</span><span class="sxs-lookup"><span data-stu-id="87a4b-132">Bash commands</span></span>

<span data-ttu-id="87a4b-133">Puede ejecutar comandos shell sin salir del modo interactivo mediante `#[cmd]`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-133">You can run shell commands without leaving interactive mode using `#[cmd]`.</span></span>

```azurecli
az>> #dir
```

## <a name="examples"></a><span data-ttu-id="87a4b-134">Ejemplos</span><span class="sxs-lookup"><span data-stu-id="87a4b-134">Examples</span></span>

<span data-ttu-id="87a4b-135">Algunos comandos tienen una gran cantidad de ejemplos.</span><span class="sxs-lookup"><span data-stu-id="87a4b-135">Some commands have lots of examples.</span></span>
<span data-ttu-id="87a4b-136">Puede desplazarse a la siguiente página de ejemplos con `CTRL-N` y a la página anterior mediante `CTRL-Y`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-136">You can scroll to the next page of examples using `CTRL-N` and the previous page using `CTRL-Y`.</span></span>

![ejemplos](./media/interactive-azure-cli/examples.png)

<span data-ttu-id="87a4b-138">También puede ver un ejemplo concreto mediante `::#`.</span><span class="sxs-lookup"><span data-stu-id="87a4b-138">You can also look at a specific example using `::#`.</span></span>

```azurecli
az>> vm create ::8
```
