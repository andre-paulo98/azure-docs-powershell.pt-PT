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
ms.openlocfilehash: 18861f0e5232e0b505767aa9609099afe88f9477
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/27/2018
ms.locfileid: "47178634"
---
# <a name="azure-stack-module-150"></a><span data-ttu-id="d5204-103">Módulo 1.5.0 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d5204-103">Azure Stack Module 1.5.0</span></span>

## <a name="requirements"></a><span data-ttu-id="d5204-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="d5204-104">Requirements:</span></span>
<span data-ttu-id="d5204-105">A versão mínima suportada do Azure Stack é a 1808.</span><span class="sxs-lookup"><span data-stu-id="d5204-105">Minimum supported Azure Stack version is 1808.</span></span>

<span data-ttu-id="d5204-106">Nota: se estiver a utilizar uma versão anterior, instale a versão 1.4.0.</span><span class="sxs-lookup"><span data-stu-id="d5204-106">Note: If you are using an earlier version install version 1.4.0</span></span>

## <a name="known-issues"></a><span data-ttu-id="d5204-107">Problemas conhecidos:</span><span class="sxs-lookup"><span data-stu-id="d5204-107">Known issues:</span></span>

- <span data-ttu-id="d5204-108">O New-AzsOffer não permite criar uma oferta com o estado público.</span><span class="sxs-lookup"><span data-stu-id="d5204-108">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="d5204-109">O cmdlet Set-AzsOffer tem de ser chamado depois para alterar o estado.</span><span class="sxs-lookup"><span data-stu-id="d5204-109">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="d5204-110">Não é possível remover um Conjunto IP sem uma reimplementação</span><span class="sxs-lookup"><span data-stu-id="d5204-110">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="install"></a><span data-ttu-id="d5204-111">Instalar</span><span class="sxs-lookup"><span data-stu-id="d5204-111">Install</span></span>
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

##<a name="release-notes"></a><span data-ttu-id="d5204-112">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="d5204-112">Release Notes</span></span>
* <span data-ttu-id="d5204-113">Todos os módulos do Azure Stack Admin foram atualizados para dependência igual ou superior no módulo AzureRm.Profile</span><span class="sxs-lookup"><span data-stu-id="d5204-113">All the Azure Stack Admin modules are updated for greater than or equal to dependency on the AzureRm.Profile module</span></span>
* <span data-ttu-id="d5204-114">Suporte para processar nomes de recursos aninhados em todos os módulos</span><span class="sxs-lookup"><span data-stu-id="d5204-114">Support for handling nested resource names in all the modules</span></span>
* <span data-ttu-id="d5204-115">Correção de erros em todos os módulos em que ErrorActionPreference são anulados e mudam para Parar</span><span class="sxs-lookup"><span data-stu-id="d5204-115">Bug fix in all the modules where ErrorActionPreference is being overridden to be Stop</span></span>
* <span data-ttu-id="d5204-116">Módulo Azs.Compute.Admin</span><span class="sxs-lookup"><span data-stu-id="d5204-116">Azs.Compute.Admin Module</span></span>
    * <span data-ttu-id="d5204-117">Novas quotas de propriedades adicionadas para suportar discos geridos</span><span class="sxs-lookup"><span data-stu-id="d5204-117">New quota properties added for the support of manged disk</span></span>
    * <span data-ttu-id="d5204-118">Adição de cmdlets relacionados com a migração de discos</span><span class="sxs-lookup"><span data-stu-id="d5204-118">Addition of disk migration related cmdlets</span></span>
    * <span data-ttu-id="d5204-119">Propriedades adicionais nos objetos Imagem da Plataforma e extensão da VM</span><span class="sxs-lookup"><span data-stu-id="d5204-119">Additional properties in the Platform Image and VM extesnion objects</span></span>
* <span data-ttu-id="d5204-120">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="d5204-120">Azs.Fabric.Admin</span></span> 
    * <span data-ttu-id="d5204-121">Novo cmdlet para adicionar o nó de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="d5204-121">New cmdlet for adding scale unit node</span></span>
* <span data-ttu-id="d5204-122">Azs.Backup.Admin</span><span class="sxs-lookup"><span data-stu-id="d5204-122">Azs.Backup.Admin</span></span>
    * <span data-ttu-id="d5204-123">Set-AzsBackupShare é agora um alias do cmdlet Set-AzsBackupConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5204-123">Set-AzsBackupShare is an alias now to the cmdlet Set-AzsBackupConfiguration</span></span>
    * <span data-ttu-id="d5204-124">Get-AzsBackupLocation é agora um alias do cmdlet Get-AzsBackupConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5204-124">Get-AzsBackupLocation is an alias now to the cmdlet Get-AzsBackupConfiguration</span></span>
    * <span data-ttu-id="d5204-125">Set-AzsBackupConfiguration, o parâmetro BackupShare é agora um alias do caminho do parâmetro</span><span class="sxs-lookup"><span data-stu-id="d5204-125">Set-AzsBackupConfiguration, the parameter BackupShare is an alias now for the parameter path</span></span>
* <span data-ttu-id="d5204-126">Azs.Subscriptions</span><span class="sxs-lookup"><span data-stu-id="d5204-126">Azs.Subscriptions</span></span>
    * <span data-ttu-id="d5204-127">Get-AzsDelegatedProviderOffer, o parâmetro OfferName é agora um alias de Offer</span><span class="sxs-lookup"><span data-stu-id="d5204-127">Get-AzsDelegatedProviderOffer, the parameter OfferName is now an alias for Offer</span></span>
* <span data-ttu-id="d5204-128">Azs.Subscriptions.Admin</span><span class="sxs-lookup"><span data-stu-id="d5204-128">Azs.Subscriptions.Admin</span></span>
    * <span data-ttu-id="d5204-129">Get-AzsDelegatedProviderOffer, o parâmetro OfferName é agora um alias de Offer</span><span class="sxs-lookup"><span data-stu-id="d5204-129">Get-AzsDelegatedProviderOffer, the parameter OfferName is now an alias for Offer</span></span>

## <a name="content"></a><span data-ttu-id="d5204-130">Conteúdo:</span><span class="sxs-lookup"><span data-stu-id="d5204-130">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="d5204-131">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="d5204-131">Azure Bridge</span></span>
<span data-ttu-id="d5204-132">Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.</span><span class="sxs-lookup"><span data-stu-id="d5204-132">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="d5204-133">Cópia de segurança</span><span class="sxs-lookup"><span data-stu-id="d5204-133">Backup</span></span>
<span data-ttu-id="d5204-134">Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="d5204-134">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="d5204-135">Configurar em que local as cópias de segurança são armazenadas</span><span class="sxs-lookup"><span data-stu-id="d5204-135">Configure where backups are stored</span></span>
- <span data-ttu-id="d5204-136">Fazer cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="d5204-136">Perform backups</span></span>
- <span data-ttu-id="d5204-137">Listar e restaurar cópias de segurança concluídas</span><span class="sxs-lookup"><span data-stu-id="d5204-137">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="d5204-138">Comércio</span><span class="sxs-lookup"><span data-stu-id="d5204-138">Commerce</span></span>
<span data-ttu-id="d5204-139">Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d5204-139">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="d5204-140">Computação</span><span class="sxs-lookup"><span data-stu-id="d5204-140">Compute</span></span>
<span data-ttu-id="d5204-141">Versão de pré-visualização do módulo de administrador Computação do Azure Stack, que fornece uma funcionalidade que permite gerir quotas de computação, imagens de plataformas, discos geridos e extensões de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="d5204-141">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="d5204-142">Recursos de infraestrutura</span><span class="sxs-lookup"><span data-stu-id="d5204-142">Fabric</span></span>
<span data-ttu-id="d5204-143">Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:</span><span class="sxs-lookup"><span data-stu-id="d5204-143">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="d5204-144">Parar, Iniciar e Encerrar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="d5204-144">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="d5204-145">Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU</span><span class="sxs-lookup"><span data-stu-id="d5204-145">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="d5204-146">Reparar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="d5204-146">Repair of scale unit nodes</span></span>
- <span data-ttu-id="d5204-147">Reiniciar a função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="d5204-147">Restart of Infrastructure role</span></span>
- <span data-ttu-id="d5204-148">Parar, Iniciar e Encerrar instâncias de função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="d5204-148">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="d5204-149">Criar novos Conjuntos IP</span><span class="sxs-lookup"><span data-stu-id="d5204-149">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="d5204-150">Galeria</span><span class="sxs-lookup"><span data-stu-id="d5204-150">Gallery</span></span>
<span data-ttu-id="d5204-151">Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d5204-151">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="d5204-152">Informações de Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="d5204-152">Infrastructure Insights</span></span>
<span data-ttu-id="d5204-153">Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="d5204-153">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="d5204-154">Ver o estado de funcionamento dos recursos de carimbo do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="d5204-154">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="d5204-155">Ver e gerir alertas</span><span class="sxs-lookup"><span data-stu-id="d5204-155">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="d5204-156">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d5204-156">KeyVault</span></span>
<span data-ttu-id="d5204-157">Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.</span><span class="sxs-lookup"><span data-stu-id="d5204-157">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="d5204-158">Rede</span><span class="sxs-lookup"><span data-stu-id="d5204-158">Network</span></span>
<span data-ttu-id="d5204-159">Versão de pré-visualização do módulo de administrador Rede que permite:</span><span class="sxs-lookup"><span data-stu-id="d5204-159">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="d5204-160">Gerir quotas de rede</span><span class="sxs-lookup"><span data-stu-id="d5204-160">Management of network quotas</span></span>
- <span data-ttu-id="d5204-161">Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga</span><span class="sxs-lookup"><span data-stu-id="d5204-161">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="d5204-162">Fornece um cmdlet que apresenta uma descrição geral de administrador</span><span class="sxs-lookup"><span data-stu-id="d5204-162">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="d5204-163">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="d5204-163">Storage</span></span>
<span data-ttu-id="d5204-164">Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d5204-164">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="d5204-165">Nesta versão, fornecemos funcionalidade para:</span><span class="sxs-lookup"><span data-stu-id="d5204-165">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="d5204-166">Gerir quotas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="d5204-166">Manage storage quotas</span></span>
- <span data-ttu-id="d5204-167">Libertar memória de recursos de armazenamento eliminados</span><span class="sxs-lookup"><span data-stu-id="d5204-167">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="d5204-168">Restaurar contas de armazenamento eliminadas</span><span class="sxs-lookup"><span data-stu-id="d5204-168">Restore deleted storage accounts</span></span>
- <span data-ttu-id="d5204-169">Migrar contentores de uma partilha para outra</span><span class="sxs-lookup"><span data-stu-id="d5204-169">Migrate containers from one share to another</span></span>
- <span data-ttu-id="d5204-170">Ver informações sobre os componentes de armazenamento individuais</span><span class="sxs-lookup"><span data-stu-id="d5204-170">View information about the individual storage components</span></span>
- <span data-ttu-id="d5204-171">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="d5204-171">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="d5204-172">Administrador da Subscrição</span><span class="sxs-lookup"><span data-stu-id="d5204-172">Subscription Admin</span></span>
<span data-ttu-id="d5204-173">Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d5204-173">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="d5204-174">Este módulo fornece funcionalidade que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="d5204-174">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="d5204-175">Gerir planos e ofertas</span><span class="sxs-lookup"><span data-stu-id="d5204-175">Manage plans and offers</span></span>
- <span data-ttu-id="d5204-176">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="d5204-176">View usage and performance information</span></span>
- <span data-ttu-id="d5204-177">Gerir o RBAC</span><span class="sxs-lookup"><span data-stu-id="d5204-177">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="d5204-178">Subscrição</span><span class="sxs-lookup"><span data-stu-id="d5204-178">Subscription</span></span>
<span data-ttu-id="d5204-179">Versão de pré-visualização do módulo Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d5204-179">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="d5204-180">Este módulo fornece funcionalidade que permite aos Utilizadores:</span><span class="sxs-lookup"><span data-stu-id="d5204-180">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="d5204-181">Criar, Eliminar e Atualizar Subscrições</span><span class="sxs-lookup"><span data-stu-id="d5204-181">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="d5204-182">Atualizar</span><span class="sxs-lookup"><span data-stu-id="d5204-182">Update</span></span>
<span data-ttu-id="d5204-183">Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="d5204-183">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="d5204-184">Neste módulo, os administradores podem:</span><span class="sxs-lookup"><span data-stu-id="d5204-184">In this module administrators can:</span></span>
- <span data-ttu-id="d5204-185">Listar e instalar atualizações disponíveis</span><span class="sxs-lookup"><span data-stu-id="d5204-185">List and install available updates</span></span>
- <span data-ttu-id="d5204-186">Retomar atualizações interrompidas</span><span class="sxs-lookup"><span data-stu-id="d5204-186">Resume interrupted updates</span></span>
- <span data-ttu-id="d5204-187">Ver atualizações instaladas</span><span class="sxs-lookup"><span data-stu-id="d5204-187">View installed updates</span></span>
