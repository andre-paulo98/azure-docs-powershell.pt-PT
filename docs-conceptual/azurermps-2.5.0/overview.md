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
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: 4b72bbd1bda93767251e0ba3d488f798575d9115
ms.sourcegitcommit: 8b3126b5c79f453464d90669f0046ba86b7a3424
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 09/01/2020
ms.locfileid: "89244318"
---
# <a name="azurerm-module-250"></a><span data-ttu-id="5bfa2-103">Módulo AzureRM 2.5.0</span><span class="sxs-lookup"><span data-stu-id="5bfa2-103">AzureRM Module 2.5.0</span></span>

## <a name="requirements"></a><span data-ttu-id="5bfa2-104">Requisitos:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-104">Requirements:</span></span>
<span data-ttu-id="5bfa2-105">A versão mínima suportada do Azure Stack é a 1904.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="5bfa2-106">Nota: Se estiver a utilizar uma versão anterior, instale a versão 1.2.11</span><span class="sxs-lookup"><span data-stu-id="5bfa2-106">Note: If you are using an earlier version install version 1.2.11</span></span>


## <a name="install"></a><span data-ttu-id="5bfa2-107">Instalar</span><span class="sxs-lookup"><span data-stu-id="5bfa2-107">Install</span></span>
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

## <a name="release-notes"></a><span data-ttu-id="5bfa2-108">Notas de Versão</span><span class="sxs-lookup"><span data-stu-id="5bfa2-108">Release Notes</span></span>
* <span data-ttu-id="5bfa2-109">AzureRm.Resources</span><span class="sxs-lookup"><span data-stu-id="5bfa2-109">AzureRm.Resources</span></span>
    * <span data-ttu-id="5bfa2-110">Novo módulo de Recursos que suporta a versão de api 2018-05-01 com o perfil 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="5bfa2-110">New Resources module supporting 2018-05-01 api version with 2019-03-01-hybrid profile</span></span>
    * <span data-ttu-id="5bfa2-111">As operações PolicyDefinition(2016-12-01) e PolicyAssisgment(2017-06-01-preview) continuam com versões de api antigas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-111">PolicyDefinition(2016-12-01) and PolicyAssisgment(2017-06-01-preview) operations are still with old api versions</span></span>
* <span data-ttu-id="5bfa2-112">AzureRm.Compute</span><span class="sxs-lookup"><span data-stu-id="5bfa2-112">AzureRm.Compute</span></span>
    * <span data-ttu-id="5bfa2-113">Novo módulo de computação que suporta a versão de api 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-113">New compute module supporting 2017-12-01 api version.'</span></span>


* <span data-ttu-id="5bfa2-114">Esta versão corresponde ao perfil de api específico do azurestack 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="5bfa2-114">This release corresponds to the azurestack specific api profile 2019-03-01-hybrid</span></span>
* <span data-ttu-id="5bfa2-115">Todos os módulos têm uma dependência igual ou superior no módulo AzureRm.Profile</span><span class="sxs-lookup"><span data-stu-id="5bfa2-115">All the modules are taking greater than or equal to dependency on the AzureRm.Profile module.</span></span>
* <span data-ttu-id="5bfa2-116">A versão de api suportada por cada um dos módulos foi atualizada.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-116">Api version suppoerted by  each of the modules are updated.</span></span> 
    * <span data-ttu-id="5bfa2-117">Computação - 2017-12-30</span><span class="sxs-lookup"><span data-stu-id="5bfa2-117">Compute - 2017-12-30</span></span>
    * <span data-ttu-id="5bfa2-118">Rede - 2017-10-01</span><span class="sxs-lookup"><span data-stu-id="5bfa2-118">Network - 2017-10-01</span></span>
    * <span data-ttu-id="5bfa2-119">Armazenamento - 2016-01-01</span><span class="sxs-lookup"><span data-stu-id="5bfa2-119">Storage - 2016-01-01</span></span>
    * <span data-ttu-id="5bfa2-120">Recursos - 2018-02-01</span><span class="sxs-lookup"><span data-stu-id="5bfa2-120">Resources - 2018-02-01</span></span>
    * <span data-ttu-id="5bfa2-121">Key Vault - 2016-10-01</span><span class="sxs-lookup"><span data-stu-id="5bfa2-121">Keyvault - 2016-10-01</span></span>
    * <span data-ttu-id="5bfa2-122">DNS - 2016-04-01</span><span class="sxs-lookup"><span data-stu-id="5bfa2-122">Dns - 2016-04-01</span></span>
* <span data-ttu-id="5bfa2-123">O mapa das versões de api completo para cada um dos tipos de recursos está disponível em https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span><span class="sxs-lookup"><span data-stu-id="5bfa2-123">The complete api version map for each of the resource types can be found at https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json</span></span>

## <a name="content"></a><span data-ttu-id="5bfa2-124">Conteúdo:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-124">Content:</span></span>
### <a name="azure-bridge"></a><span data-ttu-id="5bfa2-125">Azure Bridge</span><span class="sxs-lookup"><span data-stu-id="5bfa2-125">Azure Bridge</span></span>
<span data-ttu-id="5bfa2-126">Versão de pré-visualização do módulo de administrador AzureBridge do Azure Stack que lhe permite sindicar imagens a partir do Azure.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-126">Preview release of the Azure Stack AzureBridge administrator module which allows you to syndicate images from Azure.</span></span>

### <a name="backup"></a><span data-ttu-id="5bfa2-127">Cópia de segurança</span><span class="sxs-lookup"><span data-stu-id="5bfa2-127">Backup</span></span>
<span data-ttu-id="5bfa2-128">Versão de pré-visualização do módulo de administrador Cópia de Segurança que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-128">Preview release of the Backup administrator module that allows administrators to:</span></span>
- <span data-ttu-id="5bfa2-129">Configurar em que local as cópias de segurança são armazenadas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-129">Configure where backups are stored</span></span>
- <span data-ttu-id="5bfa2-130">Fazer cópias de segurança</span><span class="sxs-lookup"><span data-stu-id="5bfa2-130">Perform backups</span></span>
- <span data-ttu-id="5bfa2-131">Listar e restaurar cópias de segurança concluídas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-131">List and restore completed backup</span></span>

### <a name="commerce"></a><span data-ttu-id="5bfa2-132">Comércio</span><span class="sxs-lookup"><span data-stu-id="5bfa2-132">Commerce</span></span>
<span data-ttu-id="5bfa2-133">Versão de pré-visualização do módulo de administrador Comércio do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-133">Preview release of the Azure Stack Commerce administrator module which provides a way to view aggregate data usage across your Azure Stack system.</span></span>

### <a name="compute"></a><span data-ttu-id="5bfa2-134">Computação</span><span class="sxs-lookup"><span data-stu-id="5bfa2-134">Compute</span></span>
<span data-ttu-id="5bfa2-135">Versão de pré-visualização do módulo de administrador Computação do Azure Stack, que fornece uma funcionalidade que permite gerir quotas de computação, imagens de plataformas, discos geridos e extensões de máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-135">Preview release of the Azure Stack Compute administrator module which provides functionality to manage compute quotas, platform images, managed disks and virtual machine extensions.</span></span>

### <a name="fabric"></a><span data-ttu-id="5bfa2-136">Recursos de infraestrutura</span><span class="sxs-lookup"><span data-stu-id="5bfa2-136">Fabric</span></span>
<span data-ttu-id="5bfa2-137">Versão de pré-visualização do módulo de administrador Recursos de infraestrutura do Azure Stack que permite ver a utilização de dados agregados em todo o sistema do Azure Stack:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-137">Preview release of the Azure Stack Fabric administrator module which allows administrators to view and manage infrastructure components:</span></span>
- <span data-ttu-id="5bfa2-138">Parar, Iniciar e Encerrar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="5bfa2-138">Stop, Start and Shutdown of scale unit nodes</span></span>
- <span data-ttu-id="5bfa2-139">Drenar e Retomar nós de unidade de escala para atividades relacionadas com FRU</span><span class="sxs-lookup"><span data-stu-id="5bfa2-139">Drain and Resume of scale unit nodes for FRU related activities</span></span>
- <span data-ttu-id="5bfa2-140">Reparar nós de unidade de escala</span><span class="sxs-lookup"><span data-stu-id="5bfa2-140">Repair of scale unit nodes</span></span>
- <span data-ttu-id="5bfa2-141">Reiniciar a função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="5bfa2-141">Restart of Infrastructure role</span></span>
- <span data-ttu-id="5bfa2-142">Parar, Iniciar e Encerrar instâncias de função Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="5bfa2-142">Stop, Start and Shutdown of Infrastructure role instances</span></span>
- <span data-ttu-id="5bfa2-143">Criar novos Conjuntos IP</span><span class="sxs-lookup"><span data-stu-id="5bfa2-143">Create new IP Pools</span></span>


### <a name="gallery"></a><span data-ttu-id="5bfa2-144">Galeria</span><span class="sxs-lookup"><span data-stu-id="5bfa2-144">Gallery</span></span>
<span data-ttu-id="5bfa2-145">Versão de pré-visualização do módulo de administrador Galeria do Azure Stack que fornece funcionalidade que permite gerir itens da galeria no marketplace do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-145">Preview release of the Azure Stack Gallery administrator module which provides functionality to manage gallery items in the Azure Stack marketplace.</span></span>

### <a name="infrastructure-insights"></a><span data-ttu-id="5bfa2-146">Informações de Infraestrutura</span><span class="sxs-lookup"><span data-stu-id="5bfa2-146">Infrastructure Insights</span></span>
<span data-ttu-id="5bfa2-147">Versão de pré-visualização do módulo de administrador Informações de Infraestrutura que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-147">Preview release of the Infrastructure Insights administrator module which allows administrators:</span></span>
- <span data-ttu-id="5bfa2-148">Ver o estado de funcionamento dos recursos de carimbo do Azure Stack</span><span class="sxs-lookup"><span data-stu-id="5bfa2-148">View the health of their Azure Stack stamp resources</span></span>
- <span data-ttu-id="5bfa2-149">Ver e gerir alertas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-149">View and manage alerts</span></span>

### <a name="keyvault"></a><span data-ttu-id="5bfa2-150">KeyVault</span><span class="sxs-lookup"><span data-stu-id="5bfa2-150">KeyVault</span></span>
<span data-ttu-id="5bfa2-151">Versão de pré-visualização do módulo de administrador KeyVault do Azure Stack que permite ao administrador ver as quotas do KeyVault.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-151">Preview release of the Azure Stack KeyVault administrator module which allows administrator to view KeyVault quotas.</span></span>

### <a name="network"></a><span data-ttu-id="5bfa2-152">Rede</span><span class="sxs-lookup"><span data-stu-id="5bfa2-152">Network</span></span>
<span data-ttu-id="5bfa2-153">Versão de pré-visualização do módulo de administrador Rede que permite:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-153">Preview release of the Network administrator module which allows:</span></span>
- <span data-ttu-id="5bfa2-154">Gerir quotas de rede</span><span class="sxs-lookup"><span data-stu-id="5bfa2-154">Management of network quotas</span></span>
- <span data-ttu-id="5bfa2-155">Ver recursos de rede alocados, como endereços IP públicos, redes virtuais, balanceadores de carga</span><span class="sxs-lookup"><span data-stu-id="5bfa2-155">View allocated network resources such as public IP addresses, virtual networks, load balancers</span></span>
- <span data-ttu-id="5bfa2-156">Fornece um cmdlet que apresenta uma descrição geral de administrador</span><span class="sxs-lookup"><span data-stu-id="5bfa2-156">Provides a cmdlet which displays an administrator overview</span></span>

### <a name="storage"></a><span data-ttu-id="5bfa2-157">Armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bfa2-157">Storage</span></span>
<span data-ttu-id="5bfa2-158">Versão de pré-visualização do módulo de administrador Armazenamento do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-158">Preview release of the Azure Stack Storage administrator module.</span></span>  <span data-ttu-id="5bfa2-159">Nesta versão, fornecemos funcionalidade para:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-159">In this release we provide the functionality to:</span></span>
- <span data-ttu-id="5bfa2-160">Gerir quotas de armazenamento</span><span class="sxs-lookup"><span data-stu-id="5bfa2-160">Manage storage quotas</span></span>
- <span data-ttu-id="5bfa2-161">Libertar memória de recursos de armazenamento eliminados</span><span class="sxs-lookup"><span data-stu-id="5bfa2-161">Garbage collect deleted storage resources</span></span>
- <span data-ttu-id="5bfa2-162">Restaurar contas de armazenamento eliminadas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-162">Restore deleted storage accounts</span></span>
- <span data-ttu-id="5bfa2-163">Migrar contentores de uma partilha para outra</span><span class="sxs-lookup"><span data-stu-id="5bfa2-163">Migrate containers from one share to another</span></span>
- <span data-ttu-id="5bfa2-164">Ver informações sobre os componentes de armazenamento individuais</span><span class="sxs-lookup"><span data-stu-id="5bfa2-164">View information about the individual storage components</span></span>
- <span data-ttu-id="5bfa2-165">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="5bfa2-165">View usage and performance information</span></span>

### <a name="subscription-admin"></a><span data-ttu-id="5bfa2-166">Administrador da Subscrição</span><span class="sxs-lookup"><span data-stu-id="5bfa2-166">Subscription Admin</span></span>
<span data-ttu-id="5bfa2-167">Versão de pré-visualização do módulo de administrador Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-167">Preview release of the Azure Stack Subscription administrator module.</span></span>  <span data-ttu-id="5bfa2-168">Este módulo fornece funcionalidade que permite aos administradores:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-168">This module provides functionality for administrators to:</span></span>
- <span data-ttu-id="5bfa2-169">Gerir planos e ofertas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-169">Manage plans and offers</span></span>
- <span data-ttu-id="5bfa2-170">Ver informações de utilização e desempenho</span><span class="sxs-lookup"><span data-stu-id="5bfa2-170">View usage and performance information</span></span>
- <span data-ttu-id="5bfa2-171">Gerir o RBAC</span><span class="sxs-lookup"><span data-stu-id="5bfa2-171">Manage RBAC</span></span>

### <a name="subscription"></a><span data-ttu-id="5bfa2-172">Subscrição</span><span class="sxs-lookup"><span data-stu-id="5bfa2-172">Subscription</span></span>
<span data-ttu-id="5bfa2-173">Versão de pré-visualização do módulo Subscrição do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-173">Preview release of the Azure Stack Subscription module.</span></span>  <span data-ttu-id="5bfa2-174">Este módulo fornece funcionalidade que permite aos Utilizadores:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-174">This module provides functionality for Users to:</span></span>
- <span data-ttu-id="5bfa2-175">Criar, Eliminar e Atualizar Subscrições</span><span class="sxs-lookup"><span data-stu-id="5bfa2-175">Create, Delete and Update Subscriptions</span></span>

### <a name="update"></a><span data-ttu-id="5bfa2-176">Atualizar</span><span class="sxs-lookup"><span data-stu-id="5bfa2-176">Update</span></span>
<span data-ttu-id="5bfa2-177">Versão de pré-visualização do módulo de administrador Atualizar do Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="5bfa2-177">Preview release of the Azure Stack Update administrator module.</span></span>  <span data-ttu-id="5bfa2-178">Neste módulo, os administradores podem:</span><span class="sxs-lookup"><span data-stu-id="5bfa2-178">In this module administrators can:</span></span>
- <span data-ttu-id="5bfa2-179">Listar e instalar atualizações disponíveis</span><span class="sxs-lookup"><span data-stu-id="5bfa2-179">List and install available updates</span></span>
- <span data-ttu-id="5bfa2-180">Retomar atualizações interrompidas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-180">Resume interrupted updates</span></span>
- <span data-ttu-id="5bfa2-181">Ver atualizações instaladas</span><span class="sxs-lookup"><span data-stu-id="5bfa2-181">View installed updates</span></span>
