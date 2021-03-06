---
title: Descrição Geral do módulo Azure Stack Admin do PowerShell | Microsoft Docs
description: Descrição geral do módulo Azure Stack Admin com instruções para instalação e configuração.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: afa83a6258e57e961576b328e67fad634704dddf
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/05/2020
ms.locfileid: "63053363"
---
# <a name="azure-stack-module-150"></a>Módulo 1.5.0 do Azure Stack

## <a name="requirements"></a>Requisitos:
A versão mínima suportada do Azure Stack é a 1808.

Nota: se estiver a utilizar uma versão anterior, instale a versão 1.4.0.

## <a name="known-issues"></a>Problemas conhecidos:

- O New-AzsOffer não permite criar uma oferta com o estado público. O cmdlet Set-AzsOffer tem de ser chamado depois para alterar o estado.
- Não é possível remover um Conjunto IP sem uma reimplementação

## <a name="install"></a>Instalar
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.5.0
```

## <a name="release-notes"></a>Notas de Versão
* Todos os módulos do Azure Stack Admin foram atualizados para dependência igual ou superior no módulo AzureRm.Profile
* Suporte para processar nomes de recursos aninhados em todos os módulos
* Correção de erros em todos os módulos em que ErrorActionPreference são anulados e mudam para Parar
* Módulo Azs.Compute.Admin
    * Novas quotas de propriedades adicionadas para suportar discos geridos
    * Adição de cmdlets relacionados com a migração de discos
    * Propriedades adicionais nos objetos Imagem da Plataforma e extensão da VM
* Azs.Fabric.Admin 
    * Novo cmdlet para adicionar o nó de unidade de escala
* Azs.Backup.Admin
    * Set-AzsBackupShare é agora um alias do cmdlet Set-AzsBackupConfiguration
    * Get-AzsBackupLocation é agora um alias do cmdlet Get-AzsBackupConfiguration
    * Set-AzsBackupConfiguration, o parâmetro BackupShare é agora um alias do caminho do parâmetro
* Azs.Subscriptions
    * Get-AzsDelegatedProviderOffer, o parâmetro OfferName é agora um alias de Offer
* Azs.Subscriptions.Admin
    * Get-AzsDelegatedProviderOffer, o parâmetro OfferName é agora um alias de Offer

## <a name="content"></a>Conteúdo:
### <a name="azure-bridge"></a>Azure Bridge
Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.

### <a name="backup"></a>Cópia de segurança
Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:
- Configurar em que local as cópias de segurança são armazenadas
- Fazer cópias de segurança
- Listar e restaurar cópias de segurança concluídas

### <a name="commerce"></a>Comércio
Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.

### <a name="compute"></a>Computação
Versão de pré-visualização do módulo de administrador Computação do Azure Stack, que fornece uma funcionalidade que permite gerir quotas de computação, imagens de plataformas, discos geridos e extensões de máquina virtual.

### <a name="fabric"></a>Recursos de infraestrutura
Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:
- Parar, Iniciar e Encerrar nós de unidade de escala
- Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU
- Reparar nós de unidade de escala
- Reiniciar a função Infraestrutura
- Parar, Iniciar e Encerrar instâncias de função Infraestrutura
- Criar novos Conjuntos IP


### <a name="gallery"></a>Galeria
Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.

### <a name="infrastructure-insights"></a>Informações de Infraestrutura
Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:
- Ver o estado de funcionamento dos recursos de carimbo do Azure Stack
- Ver e gerir alertas

### <a name="keyvault"></a>KeyVault
Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.

### <a name="network"></a>Rede
Versão de pré-visualização do módulo de administrador Rede que permite:
- Gerir quotas de rede
- Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga
- Fornece um cmdlet que apresenta uma descrição geral de administrador

### <a name="storage"></a>Armazenamento
Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.  Nesta versão, fornecemos funcionalidade para:
- Gerir quotas de armazenamento
- Libertar memória de recursos de armazenamento eliminados
- Restaurar contas de armazenamento eliminadas
- Migrar contentores de uma partilha para outra
- Ver informações sobre os componentes de armazenamento individuais
- Ver informações de utilização e desempenho

### <a name="subscription-admin"></a>Administrador da Subscrição
Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.  Este módulo fornece funcionalidade que permite aos administradores:
- Gerir planos e ofertas
- Ver informações de utilização e desempenho
- Gerir o RBAC

### <a name="subscription"></a>Subscrição
Versão de pré-visualização do módulo Subscrição do Azure Stack.  Este módulo fornece funcionalidade que permite aos Utilizadores:
- Criar, Eliminar e Atualizar Subscrições

### <a name="update"></a>Atualizar
Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.  Neste módulo, os administradores podem:
- Listar e instalar atualizações disponíveis
- Retomar atualizações interrompidas
- Ver atualizações instaladas
