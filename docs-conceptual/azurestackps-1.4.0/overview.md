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
ms.openlocfilehash: 72d147f5bc9c882083dda6b33b1c89663fd2eb34
ms.sourcegitcommit: ff44dec6418a449757bded3c6ebe0a7d4c05ee6e
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/01/2018
ms.locfileid: "50737973"
---
# <a name="azure-stack-module-140"></a><span data-ttu-id="886bd-103">Azure Stack Module 1.4.0</span><span class="sxs-lookup"><span data-stu-id="886bd-103">Azure Stack Module 1.4.0</span></span>

## <a name="requirements"></a><span data-ttu-id="886bd-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="886bd-104">Requirements:</span></span>
<span data-ttu-id="886bd-105">A versão mínima suportada do Azure Stack é a 1804.</span><span class="sxs-lookup"><span data-stu-id="886bd-105">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="886bd-106">Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.2.11</span><span class="sxs-lookup"><span data-stu-id="886bd-106">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="886bd-107">Problemas conhecidos:</span><span class="sxs-lookup"><span data-stu-id="886bd-107">Known issues:</span></span>

- <span data-ttu-id="886bd-108">Fechar Alerta requer a versão 1803 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="886bd-108">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="886bd-109">O New-AzsOffer não permite criar uma oferta com o estado público.</span><span class="sxs-lookup"><span data-stu-id="886bd-109">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="886bd-110">O cmdlet Set-AzsOffer tem de ser chamado depois para alterar o estado.</span><span class="sxs-lookup"><span data-stu-id="886bd-110">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="886bd-111">Não é possível remover um Conjunto IP sem uma reimplementação</span><span class="sxs-lookup"><span data-stu-id="886bd-111">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="886bd-112">Alterações Interruptivas</span><span class="sxs-lookup"><span data-stu-id="886bd-112">Breaking Changes</span></span>
<span data-ttu-id="886bd-113">Não há nenhuma alteração interruptiva a partir da versão 1.3.0.</span><span class="sxs-lookup"><span data-stu-id="886bd-113">There are no breaking changes from the version 1.3.0.</span></span> <span data-ttu-id="886bd-114">Todas as alterações interruptivas migradas da versão 1.2.11 estão documentadas aqui https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="886bd-114">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="886bd-115">Instalar</span><span class="sxs-lookup"><span data-stu-id="886bd-115">Install</span></span>
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a><span data-ttu-id="886bd-116">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="886bd-116">Release Notes</span></span>
    * <span data-ttu-id="886bd-117">A versão 1.4.0 do Azurestack não tem alterações interruptivas a partir da versão 1.3.0</span><span class="sxs-lookup"><span data-stu-id="886bd-117">Azurestack 1.4.0 version has no breaking changes from the previous release 1.3.0</span></span>
    * <span data-ttu-id="886bd-118">Azs.AzureBridge.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-118">Azs.AzureBridge.Admin</span></span>
        - <span data-ttu-id="886bd-119">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-119">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-120">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-120">Azs.Backup.Admin</span></span>
        - <span data-ttu-id="886bd-121">Adicionados os novos parâmetros BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays no cmdlet Set-AzsBackupShare</span><span class="sxs-lookup"><span data-stu-id="886bd-121">Added new parameters BackupFrequencyInHours, IsBackupSchedulerEnabled, BackupRetentionPeriodInDays in cmdlet Set-AzsBackupShare</span></span>
        - <span data-ttu-id="886bd-122">Adicionado um cmdlet New-EncyptionKeyBase64 para facilitar a criação da chave de encriptação</span><span class="sxs-lookup"><span data-stu-id="886bd-122">Added a cmdlet New-EncyptionKeyBase64 to facilitate creating encryption key</span></span>
        - <span data-ttu-id="886bd-123">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-123">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-124">Azs.Commerce.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-124">Azs.Commerce.Admin</span></span>
        - <span data-ttu-id="886bd-125">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-125">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-126">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-126">Azs.Fabric.Admin</span></span>
        - <span data-ttu-id="886bd-127">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-127">Fix for the bug that returned only a single page in paginated results</span></span>
        - <span data-ttu-id="886bd-128">Adicionado um cmdlet Add-AzsScaleUnitNode para permitir ao administrador adicionar novos nós de unidade de escala ao carimbo de azurestack</span><span class="sxs-lookup"><span data-stu-id="886bd-128">Added a cmdlet Add-AzsScaleUnitNode to enable admin to add new scale unit nodes to the azurestack stamp</span></span>
        - <span data-ttu-id="886bd-129">Adicionado o cmdlet e New-AzsScaleUnitNodeObject para facilitar os objetos de parâmetro de unidade de escala de criação</span><span class="sxs-lookup"><span data-stu-id="886bd-129">Added cmdlet and New-AzsScaleUnitNodeObject to facilitate the creation scale unit parameter objects</span></span>
    * <span data-ttu-id="886bd-130">Azs.Gallery.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-130">Azs.Gallery.Admin</span></span>
        - <span data-ttu-id="886bd-131">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-131">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-132">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-132">Azs.InfrastructureInsights.Admin</span></span>
        - <span data-ttu-id="886bd-133">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-133">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-134">Azs.Network.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-134">Azs.Network.Admin</span></span>
        - <span data-ttu-id="886bd-135">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-135">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-136">Azs.Update.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-136">Azs.Update.Admin</span></span>
        - <span data-ttu-id="886bd-137">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-137">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-138">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="886bd-138">Azs.Subscriptions</span></span>
        - <span data-ttu-id="886bd-139">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-139">Fix for the bug that returned only a single page in paginated results</span></span>
    * <span data-ttu-id="886bd-140">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="886bd-140">Azs.Subscriptions.Admin</span></span>
        - <span data-ttu-id="886bd-141">Foi adicionado um cmdlet Move-AzsSubscription para mover subscrições entre ofertas de fornecedores delegados</span><span class="sxs-lookup"><span data-stu-id="886bd-141">Added a cmdlet Move-AzsSubscription to move subscriptions between delegated provider offers</span></span>
        - <span data-ttu-id="886bd-142">Adicionado um cmdlet Test-AzsMoveSubscription para validar que as subscrições do utilizador podem ser movidos entre as ofertas de fornecedor delegado</span><span class="sxs-lookup"><span data-stu-id="886bd-142">Added a cmdlet Test-AzsMoveSubscription to validate that user subscriptions can be moved between delegated provider offers</span></span>
        - <span data-ttu-id="886bd-143">Correção para o bug que devolvia apenas uma única página nos resultados paginados</span><span class="sxs-lookup"><span data-stu-id="886bd-143">Fix for the bug that returned only a single page in paginated results'</span></span>

## <a name="content"></a><span data-ttu-id="886bd-144">Conteúdo:</span><span class="sxs-lookup"><span data-stu-id="886bd-144">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="886bd-145">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="886bd-145">Azure Bridge</span></span>
<span data-ttu-id="886bd-146">Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.</span><span class="sxs-lookup"><span data-stu-id="886bd-146">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="886bd-147">Cópia de segurança</span><span class="sxs-lookup"><span data-stu-id="886bd-147">Backup</span></span>
<span data-ttu-id="886bd-148">Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="886bd-148">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="886bd-149">Configurar em que local as cópias de segurança são armazenadas</span><span class="sxs-lookup"><span data-stu-id="886bd-149">Configure where backups are stored</span></span>
- <span data-ttu-id="886bd-150">Fazer cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="886bd-150">Perform backups</span></span>
- <span data-ttu-id="886bd-151">Listar e restaurar cópias de segurança concluídas</span><span class="sxs-lookup"><span data-stu-id="886bd-151">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="886bd-152">Comércio</span><span class="sxs-lookup"><span data-stu-id="886bd-152">Commerce</span></span>
<span data-ttu-id="886bd-153">Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886bd-153">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="886bd-154">Computação</span><span class="sxs-lookup"><span data-stu-id="886bd-154">Compute</span></span>
<span data-ttu-id="886bd-155">Versão de pré-visualização do módulo de administrador Computação do Azure Stack que fornece funcionalidade que permite gerir quotas de computação, imagens de plataforma e extensões de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="886bd-155">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="886bd-156">Recursos de infraestrutura</span><span class="sxs-lookup"><span data-stu-id="886bd-156">Fabric</span></span>
<span data-ttu-id="886bd-157">Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:</span><span class="sxs-lookup"><span data-stu-id="886bd-157">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="886bd-158">Parar, Iniciar e Encerrar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="886bd-158">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="886bd-159">Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU</span><span class="sxs-lookup"><span data-stu-id="886bd-159">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="886bd-160">Reparar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="886bd-160">Repair of scale unit nodes</span></span>
- <span data-ttu-id="886bd-161">Reiniciar a função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="886bd-161">Restart of Infrastructure role</span></span>
- <span data-ttu-id="886bd-162">Parar, Iniciar e Encerrar instâncias de função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="886bd-162">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="886bd-163">Criar novos Conjuntos IP</span><span class="sxs-lookup"><span data-stu-id="886bd-163">Create new IP Pools</span></span>

### <a name="gallery"></a><span data-ttu-id="886bd-164">Galeria</span><span class="sxs-lookup"><span data-stu-id="886bd-164">Gallery</span></span>
<span data-ttu-id="886bd-165">Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886bd-165">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="886bd-166">Informações de Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="886bd-166">Infrastructure Insights</span></span>
<span data-ttu-id="886bd-167">Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="886bd-167">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="886bd-168">Ver o estado de funcionamento dos recursos de carimbo do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="886bd-168">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="886bd-169">Ver e gerir alertas</span><span class="sxs-lookup"><span data-stu-id="886bd-169">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="886bd-170">KeyVault</span><span class="sxs-lookup"><span data-stu-id="886bd-170">KeyVault</span></span>
<span data-ttu-id="886bd-171">Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.</span><span class="sxs-lookup"><span data-stu-id="886bd-171">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="886bd-172">Rede</span><span class="sxs-lookup"><span data-stu-id="886bd-172">Network</span></span>
<span data-ttu-id="886bd-173">Versão de pré-visualização do módulo de administrador Rede que permite:</span><span class="sxs-lookup"><span data-stu-id="886bd-173">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="886bd-174">Gerir quotas de rede</span><span class="sxs-lookup"><span data-stu-id="886bd-174">Management of network quotas</span></span>
- <span data-ttu-id="886bd-175">Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga</span><span class="sxs-lookup"><span data-stu-id="886bd-175">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="886bd-176">Fornece um cmdlet que apresenta uma descrição geral de administrador</span><span class="sxs-lookup"><span data-stu-id="886bd-176">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="886bd-177">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="886bd-177">Storage</span></span>
<span data-ttu-id="886bd-178">Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886bd-178">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="886bd-179">Nesta versão, fornecemos funcionalidade para:</span><span class="sxs-lookup"><span data-stu-id="886bd-179">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="886bd-180">Gerir quotas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="886bd-180">Manage storage quotas</span></span>
- <span data-ttu-id="886bd-181">Libertar memória de recursos de armazenamento eliminados</span><span class="sxs-lookup"><span data-stu-id="886bd-181">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="886bd-182">Restaurar contas de armazenamento eliminadas</span><span class="sxs-lookup"><span data-stu-id="886bd-182">Restore deleted storage accounts</span></span>
- <span data-ttu-id="886bd-183">Migrar contentores de uma partilha para outra</span><span class="sxs-lookup"><span data-stu-id="886bd-183">Migrate containers from one share to another</span></span>
- <span data-ttu-id="886bd-184">Ver informações sobre os componentes de armazenamento individuais</span><span class="sxs-lookup"><span data-stu-id="886bd-184">View information about the individual storage components</span></span>
- <span data-ttu-id="886bd-185">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="886bd-185">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="886bd-186">Administrador da Subscrição</span><span class="sxs-lookup"><span data-stu-id="886bd-186">Subscription Admin</span></span>
<span data-ttu-id="886bd-187">Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886bd-187">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="886bd-188">Este módulo fornece funcionalidade que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="886bd-188">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="886bd-189">Gerir planos e ofertas</span><span class="sxs-lookup"><span data-stu-id="886bd-189">Manage plans and offers</span></span>
- <span data-ttu-id="886bd-190">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="886bd-190">View usage and performance information</span></span>
- <span data-ttu-id="886bd-191">Gerir o RBAC</span><span class="sxs-lookup"><span data-stu-id="886bd-191">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="886bd-192">Subscrição</span><span class="sxs-lookup"><span data-stu-id="886bd-192">Subscription</span></span>
<span data-ttu-id="886bd-193">Versão de pré-visualização do módulo Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886bd-193">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="886bd-194">Este módulo fornece funcionalidade que permite aos Utilizadores:</span><span class="sxs-lookup"><span data-stu-id="886bd-194">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="886bd-195">Criar, Eliminar e Atualizar Subscrições</span><span class="sxs-lookup"><span data-stu-id="886bd-195">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="886bd-196">Atualizar</span><span class="sxs-lookup"><span data-stu-id="886bd-196">Update</span></span>
<span data-ttu-id="886bd-197">Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886bd-197">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="886bd-198">Neste módulo, os administradores podem:</span><span class="sxs-lookup"><span data-stu-id="886bd-198">In this module administrators can:</span></span>
- <span data-ttu-id="886bd-199">Listar e instalar atualizações disponíveis</span><span class="sxs-lookup"><span data-stu-id="886bd-199">List and install available updates</span></span>
- <span data-ttu-id="886bd-200">Retomar atualizações interrompidas</span><span class="sxs-lookup"><span data-stu-id="886bd-200">Resume interrupted updates</span></span>
- <span data-ttu-id="886bd-201">Ver atualizações instaladas</span><span class="sxs-lookup"><span data-stu-id="886bd-201">View installed updates</span></span>
