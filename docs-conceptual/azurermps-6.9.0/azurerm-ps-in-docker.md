---
title: Executar o Azure PowerShell num contentor do Docker
description: Como executar o Azure PowerShell num contentor do Docker.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 0ed8f50abbcb2aa00192196f19004446dc696b5d
ms.sourcegitcommit: 6c38e86e16da99f65cd183c63e34f7176b121ab8
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/04/2018
ms.locfileid: "47425266"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="3bb97-103">Executar o Azure PowerShell num contentor do Docker</span><span class="sxs-lookup"><span data-stu-id="3bb97-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="3bb97-104">A Microsoft publica imagens do Docker com o Azure PowerShell pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="3bb97-104">Microsoft publishes Docker images with Azure PowerShell pre-installed.</span></span> <span data-ttu-id="3bb97-105">Estas imagens permitem fazer experiências com o Azure PowerShell ou a executá-lo num ambiente isolado.</span><span class="sxs-lookup"><span data-stu-id="3bb97-105">These images allow for experimenting with Azure PowerShell or running it in an isolated environment.</span></span> <span data-ttu-id="3bb97-106">Existem imagens com o PowerShell Core e o PowerShell 5.</span><span class="sxs-lookup"><span data-stu-id="3bb97-106">There are images running both PowerShell Core and PowerShell 5.</span></span> 

| <span data-ttu-id="3bb97-107">Ambiente</span><span class="sxs-lookup"><span data-stu-id="3bb97-107">Environment</span></span> | <span data-ttu-id="3bb97-108">Imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="3bb97-108">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="3bb97-109">PowerShell no Windows</span><span class="sxs-lookup"><span data-stu-id="3bb97-109">PowerShell on Windows</span></span> | [<span data-ttu-id="3bb97-110">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="3bb97-110">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="3bb97-111">PowerShell Core no Windows</span><span class="sxs-lookup"><span data-stu-id="3bb97-111">PowerShell Core on Windows</span></span> | [<span data-ttu-id="3bb97-112">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="3bb97-112">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="3bb97-113">PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="3bb97-113">PowerShell Core on Linux</span></span> | [<span data-ttu-id="3bb97-114">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="3bb97-114">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="3bb97-115">Para executar qualquer um destes contentores, utilize `docker run -it $ImageName` para obter um terminal interativo.</span><span class="sxs-lookup"><span data-stu-id="3bb97-115">To run any of these containers, use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="3bb97-116">Por exemplo, para executar um contentor do Linux com o PowerShell Core:</span><span class="sxs-lookup"><span data-stu-id="3bb97-116">For example, to run a Linux container with PowerShell Core:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="3bb97-117">Para executar um contentor do Windows no Docker, o SO anfitrião tem de ser o Windows e o Docker tem de estar definido para executar contentores do Windows.</span><span class="sxs-lookup"><span data-stu-id="3bb97-117">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="3bb97-118">Para saber mais sobre como alternar entre os ambientes Windows e Linux no Docker, veja a documentação do Docker [Alternar entre os contentores do Windows e do Linux](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span><span class="sxs-lookup"><span data-stu-id="3bb97-118">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="3bb97-119">Utilizar um contentor do PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="3bb97-119">Use a PowerShell Core container</span></span>

<span data-ttu-id="3bb97-120">Os contentores do PowerShell Core são fornecidos com o PowerShell Core v6 e o módulo `AzureRM.NetCore` pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="3bb97-120">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="3bb97-121">Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:</span><span class="sxs-lookup"><span data-stu-id="3bb97-121">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="3bb97-122">Utilizar o contentor do Windows com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="3bb97-122">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="3bb97-123">O contentor do Windows tem o módulo `AzureRM` pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="3bb97-123">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="3bb97-124">Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:</span><span class="sxs-lookup"><span data-stu-id="3bb97-124">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
