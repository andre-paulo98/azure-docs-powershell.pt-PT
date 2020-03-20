---
title: Utilizar o Azure PowerShell no Docker
description: Como utilizar o Azure PowerShell pré-instalado numa imagem do Docker.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: a5746b71cfc41f7c6283b0e95b0940ca4b594ec7
ms.sourcegitcommit: fb95591c45bb5f12b98e0690938d18f2ec611897
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 03/15/2020
ms.locfileid: "79402685"
---
# <a name="using-azure-powershell-in-docker"></a><span data-ttu-id="7f94d-103">Utilizar o Azure PowerShell no Docker</span><span class="sxs-lookup"><span data-stu-id="7f94d-103">Using Azure PowerShell in Docker</span></span>

<span data-ttu-id="7f94d-104">Estamos a publicar imagens do Docker com o Azure PowerShell pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="7f94d-104">We are publishing Docker images with Azure PowerShell preinstalled.</span></span> <span data-ttu-id="7f94d-105">Este artigo mostra-lhe como começar a utilizar o Azure PowerShell no contentor do Docker.</span><span class="sxs-lookup"><span data-stu-id="7f94d-105">This article shows you how to get started using Azure PowerShell in the Docker container.</span></span>

## <a name="finding-available-images"></a><span data-ttu-id="7f94d-106">Encontrar imagens disponíveis</span><span class="sxs-lookup"><span data-stu-id="7f94d-106">Finding available images</span></span>

<span data-ttu-id="7f94d-107">As imagens publicadas requerem o Docker 17.05 ou mais recente.</span><span class="sxs-lookup"><span data-stu-id="7f94d-107">The released images require Docker 17.05 or newer.</span></span> <span data-ttu-id="7f94d-108">Espera-se também que possa executar o Docker sem `sudo` ou direitos administrativos locais.</span><span class="sxs-lookup"><span data-stu-id="7f94d-108">It is also expected that you are able to run Docker without `sudo` or local administrative rights.</span></span> <span data-ttu-id="7f94d-109">Siga as [instruções][install] oficiais do Docker para instalar `docker` corretamente.</span><span class="sxs-lookup"><span data-stu-id="7f94d-109">Please follow Docker's official [instructions][install] to install `docker` correctly.</span></span>

<span data-ttu-id="7f94d-110">Os contentores publicados são criados a partir dos contentores oficiais do PowerShell e o módulo do Az é adicionado como uma camada.</span><span class="sxs-lookup"><span data-stu-id="7f94d-110">The released containers are built from the official PowerShell containers, then the Az module added as a layer.</span></span>

<span data-ttu-id="7f94d-111">A imagem estável mais recente inclui:</span><span class="sxs-lookup"><span data-stu-id="7f94d-111">The latest stable image includes:</span></span>

- <span data-ttu-id="7f94d-112">Ubuntu 18.04</span><span class="sxs-lookup"><span data-stu-id="7f94d-112">Ubuntu 18.04</span></span>
- <span data-ttu-id="7f94d-113">Versão do PowerShell 6.2.4</span><span class="sxs-lookup"><span data-stu-id="7f94d-113">PowerShell version 6.2.4</span></span>
- <span data-ttu-id="7f94d-114">Módulo do Az mais atual do Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="7f94d-114">Azure PowerShell most current Az module</span></span>

<span data-ttu-id="7f94d-115">Pode encontrar uma lista completa das imagens disponíveis na página [Imagem do Docker][az image].</span><span class="sxs-lookup"><span data-stu-id="7f94d-115">A full list of available images can be found on our [Docker image][az image] page.</span></span>

## <a name="using-azure-powershell-in-a-container"></a><span data-ttu-id="7f94d-116">Utilizar o Azure PowerShell num contentor</span><span class="sxs-lookup"><span data-stu-id="7f94d-116">Using Azure PowerShell in a container</span></span>

<span data-ttu-id="7f94d-117">Os passos seguintes mostram os comandos do Docker necessários para transferir a imagem e iniciar uma sessão do PowerShell interativa.</span><span class="sxs-lookup"><span data-stu-id="7f94d-117">The following steps show the Docker commands required to download the image and start an interactive PowerShell session.</span></span>

1. <span data-ttu-id="7f94d-118">Transfira a imagem azure-powershell mais recente.</span><span class="sxs-lookup"><span data-stu-id="7f94d-118">Download the latest azure-powershell image.</span></span>

   ```console
   docker pull mcr.microsoft.com/azure-powershell
   ```

1. <span data-ttu-id="7f94d-119">Execute o contentor azure-powershell no modo interativo:</span><span class="sxs-lookup"><span data-stu-id="7f94d-119">Run the azure-powershell container in interactive mode:</span></span>

   ```console
   docker run -it mcr.microsoft.com/azure-powershell pwsh
   ```

### <a name="run-the-azure-powershell-container-interactively-using-host-authentication"></a><span data-ttu-id="7f94d-120">Execute o contentor azure-powershell interativamente com autenticação do anfitrião</span><span class="sxs-lookup"><span data-stu-id="7f94d-120">Run the azure-powershell container interactively using host authentication</span></span>

<span data-ttu-id="7f94d-121">Se tiver o Azure PowerShell já instalado no sistema de alojamento do Docker, poderá ter credenciais do Azure em cache.</span><span class="sxs-lookup"><span data-stu-id="7f94d-121">If you have Azure PowerShell already installed on the system hosting Docker, you may have cached Azure credentials.</span></span> <span data-ttu-id="7f94d-122">Estas credenciais podem ser utilizadas na sessão do PowerShell em execução no contentor do Docker.</span><span class="sxs-lookup"><span data-stu-id="7f94d-122">These credentials can be used in the PowerShell session running in the Docker container.</span></span>

<span data-ttu-id="7f94d-123">Por predefinição, as credenciais em cache estão no diretório `$HOME/.Azure` no seu anfitrião.</span><span class="sxs-lookup"><span data-stu-id="7f94d-123">By default, the cached credentials are in `$HOME/.Azure` directory on your host.</span></span> <span data-ttu-id="7f94d-124">O serviço Docker tem de ter acesso a esta localização para aceder às credenciais.</span><span class="sxs-lookup"><span data-stu-id="7f94d-124">The Docker service must have access to this location to access the credentials.</span></span> <span data-ttu-id="7f94d-125">O comando seguinte inicia o contentor com a cache de credenciais montada e inicia uma sessão interativa do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7f94d-125">The following command starts the container with the credential cache mounted and starts an interactive PowerShell session.</span></span>

```console
docker run -it -v ~/.Azure/AzureRmContext.json:/root/.Azure/AzureRmContext.json -v ~/.Azure/TokenCache.dat:/root/.Azure/TokenCache.dat mcr.microsoft.com/azure-powershell pwsh
```

### <a name="remove-the-image-when-no-longer-needed"></a><span data-ttu-id="7f94d-126">Remover a imagem quando já não for necessária</span><span class="sxs-lookup"><span data-stu-id="7f94d-126">Remove the image when no longer needed</span></span>

<span data-ttu-id="7f94d-127">O comando seguinte é utilizado para eliminar o contentor do Docker quando já não for necessário.</span><span class="sxs-lookup"><span data-stu-id="7f94d-127">The following command is used to delete the Docker container when you no longer need it.</span></span>

```console
docker rmi mcr.microsoft.com/azure-powershell
```

## <a name="next-steps"></a><span data-ttu-id="7f94d-128">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="7f94d-128">Next steps</span></span>

<span data-ttu-id="7f94d-129">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="7f94d-129">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>

<!-- link references -->
[install]: https://docs.docker.com/engine/installation/
[powershell image]: https://hub.docker.com/_/microsoft-powershell
[az image]: https://hub.docker.com/_/microsoft-azure-powershell