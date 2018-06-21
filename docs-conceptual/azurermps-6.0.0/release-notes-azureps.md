---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 8515a267e80e5d1f7bb97557efa72b9e86b7b45d
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 05/08/2018
ms.locfileid: "33912008"
---
# <a name="release-notes"></a><span data-ttu-id="3c643-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="3c643-103">Release notes</span></span>

<span data-ttu-id="3c643-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="3c643-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---

## <a name="600---may-2018"></a><span data-ttu-id="3c643-105">6.0.0 - maio 2018</span><span class="sxs-lookup"><span data-stu-id="3c643-105">6.0.0 - May 2018</span></span>

### <a name="general"></a><span data-ttu-id="3c643-106">Geral</span><span class="sxs-lookup"><span data-stu-id="3c643-106">General</span></span>
* <span data-ttu-id="3c643-107">Definir dependência mínima de módulos para o PowerShell 5.0</span><span class="sxs-lookup"><span data-stu-id="3c643-107">Set minimum dependency of modules to PowerShell 5.0</span></span>

### <a name="azurestorage"></a><span data-ttu-id="3c643-108">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="3c643-108">Azure.Storage</span></span>
* <span data-ttu-id="3c643-109">Suporte como nome de contentor do blob de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="3c643-109">Support  as Storage blob container name</span></span>
    - <span data-ttu-id="3c643-110">New-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="3c643-110">New-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="3c643-111">Remove-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="3c643-111">Remove-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="3c643-112">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="3c643-112">Set-AzureStorageBlobContent</span></span>
    - <span data-ttu-id="3c643-113">Get-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="3c643-113">Get-AzureStorageBlobContent</span></span>
* <span data-ttu-id="3c643-114">Correção do problema de alguns resultados de falha dos cmdlets de Armazenamento não conterem informações de falha de detalhe</span><span class="sxs-lookup"><span data-stu-id="3c643-114">Fix the issue that some Storage cmdlets failure output not contain detail failure information</span></span>

### <a name="azurermapimanagement"></a><span data-ttu-id="3c643-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="3c643-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="3c643-116">Introduzir várias alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="3c643-116">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-117">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-117">Please refer to the migration guide for more information</span></span>

### <a name="azurermautomation"></a><span data-ttu-id="3c643-118">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="3c643-118">AzureRM.Automation</span></span>
* <span data-ttu-id="3c643-119">Retirar alias de "Etiquetas" preteridas dos cmdlets</span><span class="sxs-lookup"><span data-stu-id="3c643-119">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="3c643-120">"Set-AzureRmAutomationRunbook"</span><span class="sxs-lookup"><span data-stu-id="3c643-120">'Set-AzureRmAutomationRunbook'</span></span>

### <a name="azurermbatch"></a><span data-ttu-id="3c643-121">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="3c643-121">AzureRM.Batch</span></span>
* <span data-ttu-id="3c643-122">Documentação do New-AzureBatchPool atualizada para remover exemplo preterido</span><span class="sxs-lookup"><span data-stu-id="3c643-122">Updated New-AzureBatchPool documentation to remove deprecated example</span></span>

### <a name="azurermcdn"></a><span data-ttu-id="3c643-123">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="3c643-123">AzureRM.Cdn</span></span>
* <span data-ttu-id="3c643-124">Introduzir várias alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="3c643-124">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-125">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-125">Please refer to the migration guide for more information</span></span>

### <a name="azurermcompute"></a><span data-ttu-id="3c643-126">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="3c643-126">AzureRM.Compute</span></span>
* <span data-ttu-id="3c643-127">O "New-AzureRmVm" e o "New-AzureRmVmss" suportam um resultado verboso de parâmetros</span><span class="sxs-lookup"><span data-stu-id="3c643-127">'New-AzureRmVm' and 'New-AzureRmVmss' support verbose output of parameters</span></span>
* <span data-ttu-id="3c643-128">O "New-AzureRmVm" e o "New-AzureRmVmss" (conjunto de parâmetros simples) suportam a atribuição de identidades definidas pelo sistema e (ou) definidas pelo utilizador para a(s) VM(s).</span><span class="sxs-lookup"><span data-stu-id="3c643-128">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support assigning user defined and(or) system defined identities to the VM(s).</span></span>
* <span data-ttu-id="3c643-129">Funcionalidade PerformMaintenance e Reimplementação do VMSS</span><span class="sxs-lookup"><span data-stu-id="3c643-129">VMSS Redeploy and PerformMaintenance feature</span></span>
    -  <span data-ttu-id="3c643-130">Adicionar novo parâmetro opcional -Redeploy e -PerformMaintenance to "Set-AzureRmVmss" e "Set-AzureRmVmssVM"</span><span class="sxs-lookup"><span data-stu-id="3c643-130">Add new switch parameter -Redeploy and -PerformMaintenance to 'Set-AzureRmVmss' and 'Set-AzureRmVmssVM'</span></span>
* <span data-ttu-id="3c643-131">Adicionar parâmetro opcional DisableVMAgent ao cmdlet "Set-AzureRmVMOperatingSystem"</span><span class="sxs-lookup"><span data-stu-id="3c643-131">Add DisableVMAgent switch parameter to 'Set-AzureRmVMOperatingSystem' cmdlet</span></span>
* <span data-ttu-id="3c643-132">"New-AzureRmVm" e "New-AzureRmVmss" (conjunto de parâmetros simples) suportam uma imagem do "Win10".</span><span class="sxs-lookup"><span data-stu-id="3c643-132">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support a 'Win10' image.</span></span>
* <span data-ttu-id="3c643-133">O cmdlet "Repair-AzureRmVmssServiceFabricUpdateDomain" foi adicionado.</span><span class="sxs-lookup"><span data-stu-id="3c643-133">'Repair-AzureRmVmssServiceFabricUpdateDomain' cmdlet is added.</span></span>
* <span data-ttu-id="3c643-134">Introduzir várias alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="3c643-134">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-135">Veja o guia de migração para mais detalhes</span><span class="sxs-lookup"><span data-stu-id="3c643-135">Please refer to the migration guide for more details</span></span>
* <span data-ttu-id="3c643-136">O "Set-AzureRmVmDiskEncryptionExtension" torna os parâmetros do AAD opcionais</span><span class="sxs-lookup"><span data-stu-id="3c643-136">'Set-AzureRmVmDiskEncryptionExtension' makes AAD parameters optional</span></span>

### <a name="azurermdatafactories"></a><span data-ttu-id="3c643-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="3c643-137">AzureRM.DataFactories</span></span>
* <span data-ttu-id="3c643-138">Retirar alias de "Etiquetas" preteridas dos cmdlets</span><span class="sxs-lookup"><span data-stu-id="3c643-138">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="3c643-139">New-AzureRmDataFactory</span><span class="sxs-lookup"><span data-stu-id="3c643-139">New-AzureRmDataFactory</span></span>

### <a name="azurermdatafactoryv2"></a><span data-ttu-id="3c643-140">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="3c643-140">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="3c643-141">FO SDK de .Net do ADF foi atualizado para a versão 0.7.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="3c643-141">Updated the ADF .Net SDK version to 0.7.0-preview containing following changes:</span></span>
    - <span data-ttu-id="3c643-142">Foram adicionados parâmetros de execução e propriedade de gestores de ligação na Atividade ExecuteSSISPackage</span><span class="sxs-lookup"><span data-stu-id="3c643-142">Added execution parameters and connection managers property on ExecuteSSISPackage Activity</span></span>
    - <span data-ttu-id="3c643-143">Serviço ligado atualizado PostgreSql MySql para utilizar a cadeia de ligação completa em vez do servidor, da base de dados, do esquema, do nome de utilizador e da palavra-passe</span><span class="sxs-lookup"><span data-stu-id="3c643-143">Updated PostgreSql, MySql llinked service to use full connection string instead of server, database, schema, username and password</span></span>
    - <span data-ttu-id="3c643-144">Esquema removido do serviço ligado DB2</span><span class="sxs-lookup"><span data-stu-id="3c643-144">Removed the schema from DB2 linked service</span></span>
    - <span data-ttu-id="3c643-145">Propriedade de esquema removida do serviço ligado Teradata</span><span class="sxs-lookup"><span data-stu-id="3c643-145">Removed schema property from Teradata linked service</span></span>
    - <span data-ttu-id="3c643-146">Foram adicionados o LinkedService, o Dataset e o CopySource ao Responsys</span><span class="sxs-lookup"><span data-stu-id="3c643-146">Added LinkedService, Dataset, CopySource for Responsys</span></span>

### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="3c643-147">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="3c643-147">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="3c643-148">Retirar alias de "Etiquetas" preteridas dos cmdlets</span><span class="sxs-lookup"><span data-stu-id="3c643-148">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="3c643-149">"New-AzureRmDataLakeAnalyticsAccount"</span><span class="sxs-lookup"><span data-stu-id="3c643-149">'New-AzureRmDataLakeAnalyticsAccount'</span></span>
    - <span data-ttu-id="3c643-150">"Set-AzureRmDataLakeAnalyticsAccount"</span><span class="sxs-lookup"><span data-stu-id="3c643-150">'Set-AzureRmDataLakeAnalyticsAccount'</span></span>

### <a name="azurermdatalakestore"></a><span data-ttu-id="3c643-151">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3c643-151">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="3c643-152">Adicionar nova funcionalidade da Alteração Acl recursiva a Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="3c643-152">Add new feature of recursive Acl Change to Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="3c643-153">Adicionar novo cmdlet para obter o resumo do conteúdo sob um diretório</span><span class="sxs-lookup"><span data-stu-id="3c643-153">Add new cmdlet for retrieving the content summary under a directory</span></span>
* <span data-ttu-id="3c643-154">Adicionar novo cmdlet para obter a utilização do disco e a informação de falha de sistema de Acl</span><span class="sxs-lookup"><span data-stu-id="3c643-154">Add new cmdlet for retrieving the disk usage and Acl dump</span></span>
* <span data-ttu-id="3c643-155">Corrigir tipo de devolução de AzureRmDataLakeStoreItemAcl bool para IEnumerable<DataLakeStoreItemAce></span><span class="sxs-lookup"><span data-stu-id="3c643-155">Correct return type of Set-AzureRmDataLakeStoreItemAcl bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="3c643-156">Corrigir tipo de devolução de AzureRmDataLakeStoreItemAclEntry bool para IEnumerable<DataLakeStoreItemAce></span><span class="sxs-lookup"><span data-stu-id="3c643-156">Correct return type of Set-AzureRmDataLakeStoreItemAclEntry bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="3c643-157">Alterações interruptivas no Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="3c643-157">Breaking changes in Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem</span></span>

### <a name="azurermdns"></a><span data-ttu-id="3c643-158">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="3c643-158">AzureRM.Dns</span></span>
* <span data-ttu-id="3c643-159">Introduzir várias alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="3c643-159">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-160">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-160">Please refer to the migration guide for more information</span></span>

### <a name="azurermeventhub"></a><span data-ttu-id="3c643-161">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="3c643-161">AzureRM.EventHub</span></span>
* <span data-ttu-id="3c643-162">Ajuda Atualizada para os cmdlets com exemplos em falta</span><span class="sxs-lookup"><span data-stu-id="3c643-162">Updated Help for cmdlets with missing examples</span></span>

### <a name="azurerminsights"></a><span data-ttu-id="3c643-163">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="3c643-163">AzureRM.Insights</span></span>
* <span data-ttu-id="3c643-164">Várias alterações interruptivas introduzidas</span><span class="sxs-lookup"><span data-stu-id="3c643-164">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-165">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-165">Please refer to the migration guide for more information</span></span>

### <a name="azurermiothub"></a><span data-ttu-id="3c643-166">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="3c643-166">AzureRM.IotHub</span></span>
* <span data-ttu-id="3c643-167">Ativar etiquetas e Sku Básico para o IotHub</span><span class="sxs-lookup"><span data-stu-id="3c643-167">Enable tags and Basic Sku to the IotHub</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="3c643-168">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="3c643-168">AzureRM.KeyVault</span></span>
* <span data-ttu-id="3c643-169">Alterações interruptivas para suportar cenários de piping</span><span class="sxs-lookup"><span data-stu-id="3c643-169">Breaking changes to support piping scenarios</span></span>
* <span data-ttu-id="3c643-170">Novos cmdlets adicionados: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval e Undo-AzureKeyVaultManagedStorageAccountRemoval</span><span class="sxs-lookup"><span data-stu-id="3c643-170">Added new cmdlets: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval, and Undo-AzureKeyVaultManagedStorageAccountRemoval</span></span>

### <a name="azurermmachinelearning"></a><span data-ttu-id="3c643-171">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="3c643-171">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="3c643-172">Retirar alias de "Etiquetas" preteridas dos cmdlets</span><span class="sxs-lookup"><span data-stu-id="3c643-172">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="3c643-173">Update-AzureRmMlCommitmentPlan</span><span class="sxs-lookup"><span data-stu-id="3c643-173">Update-AzureRmMlCommitmentPlan</span></span>

### <a name="azurermmedia"></a><span data-ttu-id="3c643-174">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="3c643-174">AzureRM.Media</span></span>
* <span data-ttu-id="3c643-175">Retirar alias de "Etiquetas" preteridas dos cmdlets</span><span class="sxs-lookup"><span data-stu-id="3c643-175">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="3c643-176">"Set-AzureRmMediaService"</span><span class="sxs-lookup"><span data-stu-id="3c643-176">'Set-AzureRmMediaService'</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="3c643-177">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="3c643-177">AzureRM.Network</span></span>
* <span data-ttu-id="3c643-178">Adicionar suporte ao recurso de plano de proteção contra DDoS</span><span class="sxs-lookup"><span data-stu-id="3c643-178">Add support for DDoS protection plan resource</span></span>
* <span data-ttu-id="3c643-179">Várias alterações interruptivas introduzidas</span><span class="sxs-lookup"><span data-stu-id="3c643-179">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-180">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-180">Please refer to the migration guide for more information</span></span>

### <a name="azurermnotificationhubs"></a><span data-ttu-id="3c643-181">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="3c643-181">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="3c643-182">Introduzir várias alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="3c643-182">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-183">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-183">Please refer to the migration guide for more information</span></span>

### <a name="azurermoperationalinsights"></a><span data-ttu-id="3c643-184">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="3c643-184">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="3c643-185">Introduzir várias alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="3c643-185">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-186">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-186">Please refer to the migration guide for more information</span></span>

### <a name="azurermprofile"></a><span data-ttu-id="3c643-187">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="3c643-187">AzureRM.Profile</span></span>
* <span data-ttu-id="3c643-188">Ativar gravação automática do contexto por predefinição</span><span class="sxs-lookup"><span data-stu-id="3c643-188">Enable context autosave by default</span></span>
* <span data-ttu-id="3c643-189">Adicionar propriedades USGovernmentOperationalInsightsEndpoint e USGovernmentOperationalInsightsEndpointResourceId ao ambiente do Azure para US Gov.</span><span class="sxs-lookup"><span data-stu-id="3c643-189">Add USGovernmentOperationalInsightsEndpoint and USGovernmentOperationalInsightsEndpointResourceId properties to Azure environment for US Gov.</span></span>

### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="3c643-190">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="3c643-190">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="3c643-191">Cabeçalho de Autenticação corrigida em cenários de SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="3c643-191">Fixed Authentication Header in SiteRecovery scenarios</span></span>

### <a name="azurermrediscache"></a><span data-ttu-id="3c643-192">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="3c643-192">AzureRM.RedisCache</span></span>
* <span data-ttu-id="3c643-193">Várias alterações interruptivas introduzidas</span><span class="sxs-lookup"><span data-stu-id="3c643-193">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-194">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-194">Please refer to the migration guide for more information</span></span>

### <a name="azurermresources"></a><span data-ttu-id="3c643-195">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="3c643-195">AzureRM.Resources</span></span>
* <span data-ttu-id="3c643-196">Remova o parâmetro obsoleto -AtScopeAndBelow da chamada Get-AzureRmRoledefinition</span><span class="sxs-lookup"><span data-stu-id="3c643-196">Remove obsolete parameter -AtScopeAndBelow from Get-AzureRmRoledefinition call</span></span>
* <span data-ttu-id="3c643-197">Incluir atribuições a Utilizadores/Grupos/ServicePrincipals eliminados no resultado do Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="3c643-197">Include assignments to deleted USers/Groups/ServicePrincipals in Get-AzureRmRoleAssignment result</span></span>
* <span data-ttu-id="3c643-198">Adicionar completadores de Separador de Âmbito e ResourceType</span><span class="sxs-lookup"><span data-stu-id="3c643-198">Add Tab completers for Scope and ResourceType</span></span>
* <span data-ttu-id="3c643-199">Adicionar cmdlet de conveniência para criar ServicePrincipals</span><span class="sxs-lookup"><span data-stu-id="3c643-199">Add convenience cmdlet for creating ServicePrincipals</span></span>
* <span data-ttu-id="3c643-200">Unir funcionalidade Get- e Find- no Get-AzureRmResource</span><span class="sxs-lookup"><span data-stu-id="3c643-200">Merge Get- and Find- functionality in Get-AzureRmResource</span></span>
* <span data-ttu-id="3c643-201">Adicionar Cmdlets do AD:</span><span class="sxs-lookup"><span data-stu-id="3c643-201">Add AD Cmdlets:</span></span>
  - <span data-ttu-id="3c643-202">Remove-AzureRmADGroupMember</span><span class="sxs-lookup"><span data-stu-id="3c643-202">Remove-AzureRmADGroupMember</span></span>
  - <span data-ttu-id="3c643-203">Get-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="3c643-203">Get-AzureRmADGroup</span></span>
  - <span data-ttu-id="3c643-204">New-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="3c643-204">New-AzureRmADGroup</span></span>
  - <span data-ttu-id="3c643-205">Remove-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="3c643-205">Remove-AzureRmADGroup</span></span>
  - <span data-ttu-id="3c643-206">Remove-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="3c643-206">Remove-AzureRmADUser</span></span>
  - <span data-ttu-id="3c643-207">Update-AzureRmADApplication</span><span class="sxs-lookup"><span data-stu-id="3c643-207">Update-AzureRmADApplication</span></span>
  - <span data-ttu-id="3c643-208">Update-AzureRmADServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="3c643-208">Update-AzureRmADServicePrincipal</span></span>
  - <span data-ttu-id="3c643-209">Update-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="3c643-209">Update-AzureRmADUser</span></span>

### <a name="azurermservicefabric"></a><span data-ttu-id="3c643-210">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3c643-210">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="3c643-211">Atualizar sku de versão de imagem do Linux predefinido</span><span class="sxs-lookup"><span data-stu-id="3c643-211">Update default Linux image version sku</span></span>
  - <span data-ttu-id="3c643-212">Atualização do Sku UbuntuServer1604 predefinido do NewAzureServiceFabricCluster.cs</span><span class="sxs-lookup"><span data-stu-id="3c643-212">NewAzureServiceFabricCluster.cs default UbuntuServer1604 Sku update</span></span>

### <a name="azurermstorage"></a><span data-ttu-id="3c643-213">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="3c643-213">AzureRM.Storage</span></span>
* <span data-ttu-id="3c643-214">Várias alterações interruptivas introduzidas</span><span class="sxs-lookup"><span data-stu-id="3c643-214">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="3c643-215">Veja o guia de migração para mais informações</span><span class="sxs-lookup"><span data-stu-id="3c643-215">Please refer to the migration guide for more information</span></span>

### <a name="azurermwebsites"></a><span data-ttu-id="3c643-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="3c643-216">AzureRM.Websites</span></span>
* <span data-ttu-id="3c643-217">Atualizar para a versão mais recente do SDK de Sites</span><span class="sxs-lookup"><span data-stu-id="3c643-217">Upgrade to latest version of the Websites SDK</span></span>
* <span data-ttu-id="3c643-218">Propriedades -AssignIdentity e -Httpsonly adicionadas a Set-AzureRmWebApp e a Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="3c643-218">Added -AssignIdentity & -Httpsonly properties for Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
* <span data-ttu-id="3c643-219">Dois novos cmdlets adicionados: Get-AzureRmWebAppSnapshots e Restore-AzureRmWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="3c643-219">Added two new cmdlets: Get-AzureRmWebAppSnapshots and Restore-AzureRmWebAppSnapshot</span></span>
