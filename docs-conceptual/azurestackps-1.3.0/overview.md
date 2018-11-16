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
ms.openlocfilehash: fb892daeafb1365ea62324392ac806cf9f3d39cf
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 11/15/2018
ms.locfileid: "51575557"
---
# <a name="azure-stack-module-130"></a><span data-ttu-id="6f4ff-103">Módulo 1.3.0 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6f4ff-103">Azure Stack Module 1.3.0</span></span>

## <a name="requirements"></a><span data-ttu-id="6f4ff-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-104">Requirements:</span></span>
<span data-ttu-id="6f4ff-105">A versão mínima suportada do Azure Stack é a 1804.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-105">Minimum supported Azure Stack version is 1804.</span></span>

<span data-ttu-id="6f4ff-106">Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.2.11</span><span class="sxs-lookup"><span data-stu-id="6f4ff-106">Note: If you are using an earlier version install version 1.2.11</span></span>

## <a name="known-issues"></a><span data-ttu-id="6f4ff-107">Problemas conhecidos:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-107">Known issues:</span></span>

- <span data-ttu-id="6f4ff-108">Fechar Alerta requer a versão 1803 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6f4ff-108">Close Alert requires Azure Stack version 1803</span></span>
- <span data-ttu-id="6f4ff-109">Alguns cmdlets de Armazenamento requerem a versão 1804 do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6f4ff-109">Some Storage cmdlets do require Azure Stack version 1804</span></span>
- <span data-ttu-id="6f4ff-110">O New-AzsOffer não permite criar uma oferta com o estado público.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-110">New-AzsOffer does not allow to create an offer with state public.</span></span> <span data-ttu-id="6f4ff-111">O cmdlet Set-AzsOffer tem de ser chamado depois para alterar o estado.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-111">The Set-AzsOffer cmdlet needs to be called afterwards to change the state.</span></span>
- <span data-ttu-id="6f4ff-112">Não é possível remover um Conjunto IP sem uma reimplementação</span><span class="sxs-lookup"><span data-stu-id="6f4ff-112">An IP Pool cannot be removed without a redeployment</span></span>

## <a name="breaking-changes"></a><span data-ttu-id="6f4ff-113">Alterações Interruptivas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-113">Breaking Changes</span></span>
<span data-ttu-id="6f4ff-114">Todas as alterações interruptivas migradas da versão 1.2.11 estão documentadas aqui https://aka.ms/azspowershellmigration</span><span class="sxs-lookup"><span data-stu-id="6f4ff-114">All breaking changes migrating from 1.2.11 are documented here https://aka.ms/azspowershellmigration</span></span>

## <a name="install"></a><span data-ttu-id="6f4ff-115">Instalar</span><span class="sxs-lookup"><span data-stu-id="6f4ff-115">Install</span></span>
```
# Remove previous Versions
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Uninstall-Module -Name AzureStack -Force 


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.3.0
```
## <a name="content"></a><span data-ttu-id="6f4ff-116">Conteúdo:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-116">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="6f4ff-117">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="6f4ff-117">Azure Bridge</span></span>
<span data-ttu-id="6f4ff-118">Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-118">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="6f4ff-119">Cópia de segurança</span><span class="sxs-lookup"><span data-stu-id="6f4ff-119">Backup</span></span>
<span data-ttu-id="6f4ff-120">Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-120">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="6f4ff-121">Configurar em que local as cópias de segurança são armazenadas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-121">Configure where backups are stored</span></span>
- <span data-ttu-id="6f4ff-122">Fazer cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="6f4ff-122">Perform backups</span></span>
- <span data-ttu-id="6f4ff-123">Listar e restaurar cópias de segurança concluídas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-123">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="6f4ff-124">Comércio</span><span class="sxs-lookup"><span data-stu-id="6f4ff-124">Commerce</span></span>
<span data-ttu-id="6f4ff-125">Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-125">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="6f4ff-126">Computação</span><span class="sxs-lookup"><span data-stu-id="6f4ff-126">Compute</span></span>
<span data-ttu-id="6f4ff-127">Versão de pré-visualização do módulo de administrador Computação do Azure Stack que fornece funcionalidade que permite gerir quotas de computação, imagens de plataforma e extensões de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-127">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="6f4ff-128">Recursos de infraestrutura</span><span class="sxs-lookup"><span data-stu-id="6f4ff-128">Fabric</span></span>
<span data-ttu-id="6f4ff-129">Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-129">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="6f4ff-130">Parar, Iniciar e Encerrar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="6f4ff-130">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="6f4ff-131">Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU</span><span class="sxs-lookup"><span data-stu-id="6f4ff-131">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="6f4ff-132">Reparar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="6f4ff-132">Repair of scale unit nodes</span></span>
- <span data-ttu-id="6f4ff-133">Reiniciar a função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="6f4ff-133">Restart of Infrastructure role</span></span>
- <span data-ttu-id="6f4ff-134">Parar, Iniciar e Encerrar instâncias de função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="6f4ff-134">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="6f4ff-135">Criar novos Conjuntos IP</span><span class="sxs-lookup"><span data-stu-id="6f4ff-135">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="6f4ff-136">Galeria</span><span class="sxs-lookup"><span data-stu-id="6f4ff-136">Gallery</span></span>
<span data-ttu-id="6f4ff-137">Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-137">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="6f4ff-138">Informações de Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="6f4ff-138">Infrastructure Insights</span></span>
<span data-ttu-id="6f4ff-139">Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-139">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="6f4ff-140">Ver o estado de funcionamento dos recursos de carimbo do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="6f4ff-140">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="6f4ff-141">Ver e gerir alertas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-141">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="6f4ff-142">KeyVault</span><span class="sxs-lookup"><span data-stu-id="6f4ff-142">KeyVault</span></span>
<span data-ttu-id="6f4ff-143">Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-143">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="6f4ff-144">Rede</span><span class="sxs-lookup"><span data-stu-id="6f4ff-144">Network</span></span>
<span data-ttu-id="6f4ff-145">Versão de pré-visualização do módulo de administrador Rede que permite:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-145">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="6f4ff-146">Gerir quotas de rede</span><span class="sxs-lookup"><span data-stu-id="6f4ff-146">Management of network quotas</span></span>
- <span data-ttu-id="6f4ff-147">Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga</span><span class="sxs-lookup"><span data-stu-id="6f4ff-147">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="6f4ff-148">Fornece um cmdlet que apresenta uma descrição geral de administrador</span><span class="sxs-lookup"><span data-stu-id="6f4ff-148">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="6f4ff-149">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="6f4ff-149">Storage</span></span>
<span data-ttu-id="6f4ff-150">Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-150">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="6f4ff-151">Nesta versão, fornecemos funcionalidade para:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-151">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="6f4ff-152">Gerir quotas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="6f4ff-152">Manage storage quotas</span></span>
- <span data-ttu-id="6f4ff-153">Libertar memória de recursos de armazenamento eliminados</span><span class="sxs-lookup"><span data-stu-id="6f4ff-153">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="6f4ff-154">Restaurar contas de armazenamento eliminadas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-154">Restore deleted storage accounts</span></span>
- <span data-ttu-id="6f4ff-155">Migrar contentores de uma partilha para outra</span><span class="sxs-lookup"><span data-stu-id="6f4ff-155">Migrate containers from one share to another</span></span>
- <span data-ttu-id="6f4ff-156">Ver informações sobre os componentes de armazenamento individuais</span><span class="sxs-lookup"><span data-stu-id="6f4ff-156">View information about the individual storage components</span></span>
- <span data-ttu-id="6f4ff-157">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="6f4ff-157">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="6f4ff-158">Administrador da Subscrição</span><span class="sxs-lookup"><span data-stu-id="6f4ff-158">Subscription Admin</span></span>
<span data-ttu-id="6f4ff-159">Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-159">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="6f4ff-160">Este módulo fornece funcionalidade que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-160">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="6f4ff-161">Gerir planos e ofertas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-161">Manage plans and offers</span></span>
- <span data-ttu-id="6f4ff-162">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="6f4ff-162">View usage and performance information</span></span>
- <span data-ttu-id="6f4ff-163">Gerir o RBAC</span><span class="sxs-lookup"><span data-stu-id="6f4ff-163">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="6f4ff-164">Subscrição</span><span class="sxs-lookup"><span data-stu-id="6f4ff-164">Subscription</span></span>
<span data-ttu-id="6f4ff-165">Versão de pré-visualização do módulo Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-165">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="6f4ff-166">Este módulo fornece funcionalidade que permite aos Utilizadores:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-166">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="6f4ff-167">Criar, Eliminar e Atualizar Subscrições</span><span class="sxs-lookup"><span data-stu-id="6f4ff-167">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="6f4ff-168">Atualizar</span><span class="sxs-lookup"><span data-stu-id="6f4ff-168">Update</span></span>
<span data-ttu-id="6f4ff-169">Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="6f4ff-169">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="6f4ff-170">Neste módulo, os administradores podem:</span><span class="sxs-lookup"><span data-stu-id="6f4ff-170">In this module administrators can:</span></span>
- <span data-ttu-id="6f4ff-171">Listar e instalar atualizações disponíveis</span><span class="sxs-lookup"><span data-stu-id="6f4ff-171">List and install available updates</span></span>
- <span data-ttu-id="6f4ff-172">Retomar atualizações interrompidas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-172">Resume interrupted updates</span></span>
- <span data-ttu-id="6f4ff-173">Ver atualizações instaladas</span><span class="sxs-lookup"><span data-stu-id="6f4ff-173">View installed updates</span></span>
