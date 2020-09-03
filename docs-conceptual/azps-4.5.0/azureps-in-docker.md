---
title: Utilizar o Azure PowerShell no Docker
description: Como utilizar o Azure PowerShell pré-instalado numa imagem do Docker.
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/20/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 2b487abeecbffa6cd8b7b64276ab301619348385
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89239864"
---
# <a name="using-azure-powershell-in-docker"></a><span data-ttu-id="5a682-103">Utilizar o Azure PowerShell no Docker</span><span class="sxs-lookup"><span data-stu-id="5a682-103">Using Azure PowerShell in Docker</span></span>

<span data-ttu-id="5a682-104">Estamos a publicar imagens do Docker com o Azure PowerShell pré-instalado.</span><span class="sxs-lookup"><span data-stu-id="5a682-104">We are publishing Docker images with Azure PowerShell preinstalled.</span></span> <span data-ttu-id="5a682-105">Este artigo mostra-lhe como começar a utilizar o Azure PowerShell no contentor do Docker.</span><span class="sxs-lookup"><span data-stu-id="5a682-105">This article shows you how to get started using Azure PowerShell in the Docker container.</span></span>

## <a name="finding-available-images"></a><span data-ttu-id="5a682-106">Encontrar imagens disponíveis</span><span class="sxs-lookup"><span data-stu-id="5a682-106">Finding available images</span></span>

<span data-ttu-id="5a682-107">As imagens publicadas requerem o Docker 17.05 ou mais recente.</span><span class="sxs-lookup"><span data-stu-id="5a682-107">The released images require Docker 17.05 or newer.</span></span> <span data-ttu-id="5a682-108">Espera-se também que possa executar o Docker sem `sudo` ou direitos administrativos locais.</span><span class="sxs-lookup"><span data-stu-id="5a682-108">It is also expected that you are able to run Docker without `sudo` or local administrative rights.</span></span> <span data-ttu-id="5a682-109">Siga as [instruções][install] oficiais do Docker para instalar `docker` corretamente.</span><span class="sxs-lookup"><span data-stu-id="5a682-109">Please follow Docker's official [instructions][install] to install `docker` correctly.</span></span>

<span data-ttu-id="5a682-110">A mais recente imagem de contentor inclui a última versão do PowerShell e os mais recentes módulos do Azure PowerShell suportados com o módulo Az.</span><span class="sxs-lookup"><span data-stu-id="5a682-110">The latest container image contains the latest version of PowerShell and the latest Azure PowerShell modules supported with the Az module.</span></span>

<span data-ttu-id="5a682-111">Por cada nova versão do módulo Az, vamos disponibilizar uma imagem para os seguintes sistemas operativos:</span><span class="sxs-lookup"><span data-stu-id="5a682-111">For each new release of the Az module we are releasing an image for the following operating systems:</span></span>

- <span data-ttu-id="5a682-112">Ubuntu 18.04 (predefinição)</span><span class="sxs-lookup"><span data-stu-id="5a682-112">Ubuntu 18.04 (default)</span></span>
- <span data-ttu-id="5a682-113">Debian 9</span><span class="sxs-lookup"><span data-stu-id="5a682-113">Debian 9</span></span>
- <span data-ttu-id="5a682-114">CentOs 7</span><span class="sxs-lookup"><span data-stu-id="5a682-114">CentOs 7</span></span>

<span data-ttu-id="5a682-115">Pode encontrar uma lista completa das imagens disponíveis na página [Imagem do Docker][az image].</span><span class="sxs-lookup"><span data-stu-id="5a682-115">A full list of available images can be found on our [Docker image][az image] page.</span></span>

## <a name="using-azure-powershell-in-a-container"></a><span data-ttu-id="5a682-116">Utilizar o Azure PowerShell num contentor</span><span class="sxs-lookup"><span data-stu-id="5a682-116">Using Azure PowerShell in a container</span></span>

<span data-ttu-id="5a682-117">Os passos seguintes mostram os comandos do Docker necessários para transferir a imagem e iniciar uma sessão do PowerShell interativa.</span><span class="sxs-lookup"><span data-stu-id="5a682-117">The following steps show the Docker commands required to download the image and start an interactive PowerShell session.</span></span>

1. <span data-ttu-id="5a682-118">Transfira a imagem azure-powershell mais recente.</span><span class="sxs-lookup"><span data-stu-id="5a682-118">Download the latest azure-powershell image.</span></span>

   ```console
   docker pull mcr.microsoft.com/azure-powershell
   ```

1. <span data-ttu-id="5a682-119">Execute o contentor azure-powershell no modo interativo:</span><span class="sxs-lookup"><span data-stu-id="5a682-119">Run the azure-powershell container in interactive mode:</span></span>

   ```console
   docker run -it mcr.microsoft.com/azure-powershell pwsh
   ```

<span data-ttu-id="5a682-120">Para os anfitriões do Docker para Windows, tem de ativar a Partilha de Ficheiros do Docker para permitir que as unidades locais no Windows sejam partilhadas com os contentores do Linux.</span><span class="sxs-lookup"><span data-stu-id="5a682-120">For Windows Docker hosts, you must enable Docker File Sharing to allow local drives on Windows to be shared with Linux containers.</span></span> <span data-ttu-id="5a682-121">Para obter mais informações, veja [Introdução ao Docker for Windows][file-sharing].</span><span class="sxs-lookup"><span data-stu-id="5a682-121">For more information see [Get started with Docker for Windows][file-sharing].</span></span>

### <a name="run-the-azure-powershell-container-interactively-using-host-authentication"></a><span data-ttu-id="5a682-122">Execute o contentor azure-powershell interativamente com autenticação do anfitrião</span><span class="sxs-lookup"><span data-stu-id="5a682-122">Run the azure-powershell container interactively using host authentication</span></span>

<span data-ttu-id="5a682-123">Se tiver o Azure PowerShell já instalado no sistema de alojamento do Docker, poderá ter credenciais do Azure em cache.</span><span class="sxs-lookup"><span data-stu-id="5a682-123">If you have Azure PowerShell already installed on the system hosting Docker, you may have cached Azure credentials.</span></span> <span data-ttu-id="5a682-124">Estas credenciais podem ser utilizadas na sessão do PowerShell em execução no contentor do Docker.</span><span class="sxs-lookup"><span data-stu-id="5a682-124">These credentials can be used in the PowerShell session running in the Docker container.</span></span>

<span data-ttu-id="5a682-125">Por predefinição, as credenciais em cache estão no diretório `$HOME/.Azure` no seu anfitrião.</span><span class="sxs-lookup"><span data-stu-id="5a682-125">By default, the cached credentials are in `$HOME/.Azure` directory on your host.</span></span> <span data-ttu-id="5a682-126">O serviço Docker tem de ter acesso a esta localização para aceder às credenciais.</span><span class="sxs-lookup"><span data-stu-id="5a682-126">The Docker service must have access to this location to access the credentials.</span></span> <span data-ttu-id="5a682-127">O comando seguinte inicia o contentor com a cache de credenciais montada e inicia uma sessão interativa do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="5a682-127">The following command starts the container with the credential cache mounted and starts an interactive PowerShell session.</span></span>

```console
docker run -it -v ~/.Azure/AzureRmContext.json:/root/.Azure/AzureRmContext.json -v ~/.Azure/TokenCache.dat:/root/.Azure/TokenCache.dat mcr.microsoft.com/azure-powershell pwsh
```

### <a name="remove-the-image-when-no-longer-needed"></a><span data-ttu-id="5a682-128">Remover a imagem quando já não for necessária</span><span class="sxs-lookup"><span data-stu-id="5a682-128">Remove the image when no longer needed</span></span>

<span data-ttu-id="5a682-129">O comando seguinte é utilizado para eliminar o contentor do Docker quando já não for necessário.</span><span class="sxs-lookup"><span data-stu-id="5a682-129">The following command is used to delete the Docker container when you no longer need it.</span></span>

```console
docker rmi mcr.microsoft.com/azure-powershell
```

## <a name="next-steps"></a><span data-ttu-id="5a682-130">Passos seguintes</span><span class="sxs-lookup"><span data-stu-id="5a682-130">Next steps</span></span>

<span data-ttu-id="5a682-131">Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).</span><span class="sxs-lookup"><span data-stu-id="5a682-131">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>

<!-- link references -->
[install]: https://docs.docker.com/engine/installation/
[powershell image]: https://hub.docker.com/_/microsoft-powershell
[az image]: https://hub.docker.com/_/microsoft-azure-powershell
[file-sharing]: https://docs.docker.com/docker-for-windows/#file-sharing
