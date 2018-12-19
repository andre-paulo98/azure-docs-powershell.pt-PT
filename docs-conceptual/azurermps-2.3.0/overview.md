---
title: Descrição Geral do Azure Stack do PowerShell | Microsoft Docs
description: Descrição geral do Azure Stack do PowerShell com instruções para instalação e configuração.
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: cd415e862bfaa2b767cce108689ebaf34ef74305
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 12/13/2018
ms.locfileid: "53218158"
---
# <a name="azurerm-module-230"></a>Módulo AzureRM 2.3.0

## <a name="requirements"></a>Requisitos:
A versão mínima suportada do Azure Stack é a 1808.

Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.2.11


## <a name="install"></a>Instalar
```powershell-interactive
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module -Name AzureRM -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force -ErrorAction Continue
Uninstall-Module AzureRM.AzureStackStorage -Force -ErrorAction Continue
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force
Get-Module Azure.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

```

## <a name="release-notes"></a>Notas de Versão
* A versão 2.3.0 inclui uma lista de alterações interruptivas. Para atualizar da versão 1.2.11, criámos um guia de migração em https://aka.ms/azspowershellmigration
* Esta versão corresponde ao perfil de api específico azurestack 2018-03-01-hybrid
* Todos os módulos têm uma dependência igual ou superior no módulo AzureRm.Profile
* A versão de api suportada por cada um dos módulos foi atualizada. 
    * Computação - 2017-03-30
    * Rede - 2017-10-01
    * Armazenamento - 2016-01-01
    * Recursos - 2018-02-01
    * Key Vault - 2016-10-01
    * DNS - 2016-04-01
* O mapa das versões de api completo para cada um dos tipos de recursos está disponível em https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json

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
