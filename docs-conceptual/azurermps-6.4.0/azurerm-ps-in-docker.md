---
title: Executar o Azure PowerShell num contentor do Docker
description: Como executar o Azure PowerShell num contentor do Docker.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: b224beb95809d0e48c6f1dd5985de45b3b4df816
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406364"
---
## <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="ea790-103">Executar o Azure PowerShell num contentor do Docker</span><span class="sxs-lookup"><span data-stu-id="ea790-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="ea790-104">Existe um conjunto de imagens do Docker pré-configuradas com o Azure PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ea790-104">There are a set of Docker images preconfigured with Azure PowerShell.</span></span> <span data-ttu-id="ea790-105">Estão disponíveis dois tipos de contentor: contentores com o PowerShell tradicional em execução no Windows e um contentor com o PowerShell Core em execução no Windows ou Linux.</span><span class="sxs-lookup"><span data-stu-id="ea790-105">Two types of containers are available: Those running traditional PowerShell on Windows, and a container running PowerShell Core on either Windows or Linux.</span></span>

| <span data-ttu-id="ea790-106">Ambiente</span><span class="sxs-lookup"><span data-stu-id="ea790-106">Environment</span></span> | <span data-ttu-id="ea790-107">Imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="ea790-107">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="ea790-108">PowerShell no Windows</span><span class="sxs-lookup"><span data-stu-id="ea790-108">PowerShell on Windows</span></span> | [<span data-ttu-id="ea790-109">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="ea790-109">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="ea790-110">PowerShell Core no Windows</span><span class="sxs-lookup"><span data-stu-id="ea790-110">PowerShell Core on Windows</span></span> | [<span data-ttu-id="ea790-111">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="ea790-111">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="ea790-112">PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="ea790-112">PowerShell Core on Linux</span></span> | [<span data-ttu-id="ea790-113">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="ea790-113">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="ea790-114">Para executar qualquer um destes contentores, utilize `docker run -it $ImageName` para obter um terminal interativo.</span><span class="sxs-lookup"><span data-stu-id="ea790-114">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="ea790-115">Por exemplo, para executar o PowerShell Core no contentor do Linux, utilize:</span><span class="sxs-lookup"><span data-stu-id="ea790-115">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="ea790-116">Para executar um contentor do Windows no Docker, o SO anfitrião tem de ser o Windows e o Docker tem de estar definido para executar contentores do Windows.</span><span class="sxs-lookup"><span data-stu-id="ea790-116">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="ea790-117">Para saber mais sobre como alternar entre os ambientes Windows e Linux no Docker, veja a documentação do Docker [Alternar entre os contentores do Windows e do Linux](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span><span class="sxs-lookup"><span data-stu-id="ea790-117">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="ea790-118">Utilizar um contentor do PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="ea790-118">Use a PowerShell Core container</span></span>

<span data-ttu-id="ea790-119">Os contentores do PowerShell Core são fornecidos com o PowerShell Core v6 e o módulo `AzureRM.NetCore` pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="ea790-119">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="ea790-120">Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:</span><span class="sxs-lookup"><span data-stu-id="ea790-120">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="ea790-121">Utilizar o contentor do Windows com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="ea790-121">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="ea790-122">O contentor do Windows tem o módulo `AzureRM` pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="ea790-122">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="ea790-123">Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:</span><span class="sxs-lookup"><span data-stu-id="ea790-123">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```