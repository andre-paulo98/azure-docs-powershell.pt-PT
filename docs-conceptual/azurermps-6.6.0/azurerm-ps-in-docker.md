---
title: Executar o Azure PowerShell num contentor do Docker
description: Como executar o Azure PowerShell num contentor do Docker.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 27ac176d8bd0b142b7740b2ba6793edb500a8af3
ms.sourcegitcommit: 72086f8d368ec84bd403e802305acfc336c08978
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/14/2018
ms.locfileid: "43018530"
---
# <a name="run-azure-powershell-in-a-docker-container"></a><span data-ttu-id="43d14-103">Executar o Azure PowerShell num contentor do Docker</span><span class="sxs-lookup"><span data-stu-id="43d14-103">Run Azure PowerShell in a Docker container</span></span>

<span data-ttu-id="43d14-104">Para facilitar a execução do Azure PowerShell em ambientes portáteis, a Microsoft publica imagens do Docker com o Azure PowerShell pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="43d14-104">To make running Azure PowerShell in portable environments easy, Microsoft publishes Docker images with Azure PowerShell pre-installed.</span></span> <span data-ttu-id="43d14-105">Estas imagens oferecem um convidado do Linux que executa o PowerShell Core ou um convidado do Windows com o PowerShell Core ou PowerShell 5.</span><span class="sxs-lookup"><span data-stu-id="43d14-105">These images offer a Linux guest running PowerShell Core, or a Windows guest with either PowerShell Core or PowerShell 5.</span></span>

| <span data-ttu-id="43d14-106">Ambiente</span><span class="sxs-lookup"><span data-stu-id="43d14-106">Environment</span></span> | <span data-ttu-id="43d14-107">Imagem do Docker</span><span class="sxs-lookup"><span data-stu-id="43d14-107">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="43d14-108">PowerShell no Windows</span><span class="sxs-lookup"><span data-stu-id="43d14-108">PowerShell on Windows</span></span> | [<span data-ttu-id="43d14-109">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="43d14-109">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="43d14-110">PowerShell Core no Windows</span><span class="sxs-lookup"><span data-stu-id="43d14-110">PowerShell Core on Windows</span></span> | [<span data-ttu-id="43d14-111">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="43d14-111">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="43d14-112">PowerShell Core no Linux</span><span class="sxs-lookup"><span data-stu-id="43d14-112">PowerShell Core on Linux</span></span> | [<span data-ttu-id="43d14-113">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="43d14-113">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="43d14-114">Para executar qualquer um destes contentores, utilize `docker run -it $ImageName` para obter um terminal interativo.</span><span class="sxs-lookup"><span data-stu-id="43d14-114">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="43d14-115">Por exemplo, para executar o PowerShell Core no contentor do Linux, utilize:</span><span class="sxs-lookup"><span data-stu-id="43d14-115">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="43d14-116">Para executar um contentor do Windows no Docker, o SO anfitrião tem de ser o Windows e o Docker tem de estar definido para executar contentores do Windows.</span><span class="sxs-lookup"><span data-stu-id="43d14-116">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="43d14-117">Para saber mais sobre como alternar entre os ambientes Windows e Linux no Docker, veja a documentação do Docker [Alternar entre os contentores do Windows e do Linux](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span><span class="sxs-lookup"><span data-stu-id="43d14-117">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>

## <a name="use-a-powershell-core-container"></a><span data-ttu-id="43d14-118">Utilizar um contentor do PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="43d14-118">Use a PowerShell Core container</span></span>

<span data-ttu-id="43d14-119">Os contentores do PowerShell Core são fornecidos com o PowerShell Core v6 e o módulo `AzureRM.NetCore` pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="43d14-119">The PowerShell Core containers come with PowerShell Core v6 and the `AzureRM.NetCore` module pre-installed.</span></span> <span data-ttu-id="43d14-120">Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:</span><span class="sxs-lookup"><span data-stu-id="43d14-120">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a><span data-ttu-id="43d14-121">Utilizar o contentor do Windows com o PowerShell</span><span class="sxs-lookup"><span data-stu-id="43d14-121">Use the Windows container with PowerShell</span></span>

<span data-ttu-id="43d14-122">O contentor do Windows tem o módulo `AzureRM` pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="43d14-122">The Windows container has the `AzureRM` module pre-installed.</span></span> <span data-ttu-id="43d14-123">Execute o cmdlet [Import-Module](/powershell/module/microsoft.powershell.core/import-module) e, em seguida, inicie sessão na sua conta do Azure:</span><span class="sxs-lookup"><span data-stu-id="43d14-123">Run the [Import-Module](/powershell/module/microsoft.powershell.core/import-module) cmdlet and then sign in with your Azure account:</span></span>

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```
