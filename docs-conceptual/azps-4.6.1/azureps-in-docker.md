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
ms.locfileid: "89241768"
---
# <a name="using-azure-powershell-in-docker"></a>Utilizar o Azure PowerShell no Docker

Estamos a publicar imagens do Docker com o Azure PowerShell pré-instalado. Este artigo mostra-lhe como começar a utilizar o Azure PowerShell no contentor do Docker.

## <a name="finding-available-images"></a>Encontrar imagens disponíveis

As imagens publicadas requerem o Docker 17.05 ou mais recente. Espera-se também que possa executar o Docker sem `sudo` ou direitos administrativos locais. Siga as [instruções][install] oficiais do Docker para instalar `docker` corretamente.

A mais recente imagem de contentor inclui a última versão do PowerShell e os mais recentes módulos do Azure PowerShell suportados com o módulo Az.

Por cada nova versão do módulo Az, vamos disponibilizar uma imagem para os seguintes sistemas operativos:

- Ubuntu 18.04 (predefinição)
- Debian 9
- CentOs 7

Pode encontrar uma lista completa das imagens disponíveis na página [Imagem do Docker][az image].

## <a name="using-azure-powershell-in-a-container"></a>Utilizar o Azure PowerShell num contentor

Os passos seguintes mostram os comandos do Docker necessários para transferir a imagem e iniciar uma sessão do PowerShell interativa.

1. Transfira a imagem azure-powershell mais recente.

   ```console
   docker pull mcr.microsoft.com/azure-powershell
   ```

1. Execute o contentor azure-powershell no modo interativo:

   ```console
   docker run -it mcr.microsoft.com/azure-powershell pwsh
   ```

Para os anfitriões do Docker para Windows, tem de ativar a Partilha de Ficheiros do Docker para permitir que as unidades locais no Windows sejam partilhadas com os contentores do Linux. Para obter mais informações, veja [Introdução ao Docker for Windows][file-sharing].

### <a name="run-the-azure-powershell-container-interactively-using-host-authentication"></a>Execute o contentor azure-powershell interativamente com autenticação do anfitrião

Se tiver o Azure PowerShell já instalado no sistema de alojamento do Docker, poderá ter credenciais do Azure em cache. Estas credenciais podem ser utilizadas na sessão do PowerShell em execução no contentor do Docker.

Por predefinição, as credenciais em cache estão no diretório `$HOME/.Azure` no seu anfitrião. O serviço Docker tem de ter acesso a esta localização para aceder às credenciais. O comando seguinte inicia o contentor com a cache de credenciais montada e inicia uma sessão interativa do PowerShell.

```console
docker run -it -v ~/.Azure/AzureRmContext.json:/root/.Azure/AzureRmContext.json -v ~/.Azure/TokenCache.dat:/root/.Azure/TokenCache.dat mcr.microsoft.com/azure-powershell pwsh
```

### <a name="remove-the-image-when-no-longer-needed"></a>Remover a imagem quando já não for necessária

O comando seguinte é utilizado para eliminar o contentor do Docker quando já não for necessário.

```console
docker rmi mcr.microsoft.com/azure-powershell
```

## <a name="next-steps"></a>Passos seguintes

Para saber mais sobre os módulos do Azure PowerShell e as respetivas funcionalidades, veja [Introdução ao Azure PowerShell](get-started-azureps.md).

<!-- link references -->
[install]: https://docs.docker.com/engine/installation/
[powershell image]: https://hub.docker.com/_/microsoft-powershell
[az image]: https://hub.docker.com/_/microsoft-azure-powershell
[file-sharing]: https://docs.docker.com/docker-for-windows/#file-sharing
