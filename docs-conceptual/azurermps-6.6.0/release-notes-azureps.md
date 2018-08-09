---
title: Registo de alterações do Azure PowerShell | Microsoft Docs
description: Este é um histórico das alterações realizadas no Azure PowerShell na versão mais recente.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 3961f5c37869d0dc877b85bad535f399181040db
ms.sourcegitcommit: fd11600079ee3844986552bccc4e274a231332b6
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 08/02/2018
ms.locfileid: "39368182"
---
# <a name="release-notes"></a><span data-ttu-id="9edcb-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="9edcb-103">Release notes</span></span>

<span data-ttu-id="9edcb-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="9edcb-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="660---july-2018"></a><span data-ttu-id="9edcb-105">6.6.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="9edcb-105">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9edcb-106">Geral</span><span class="sxs-lookup"><span data-stu-id="9edcb-106">General</span></span>
* <span data-ttu-id="9edcb-107">Foram atualizados todos os ficheiros de ajuda para incluir tipos de parâmetros inteiros e tipos de entrada/saída corretos.</span><span class="sxs-lookup"><span data-stu-id="9edcb-107">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9edcb-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9edcb-108">AzureRM.Profile</span></span>
* <span data-ttu-id="9edcb-109">A biblioteca Common.Strategy foi atualizada para poder validar que a configuração atual de um recurso é compatível com o recurso de destino.</span><span class="sxs-lookup"><span data-stu-id="9edcb-109">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span> <span data-ttu-id="9edcb-110">A predefinição é sempre “true”, recursos individuais e substituir a predefinição.</span><span class="sxs-lookup"><span data-stu-id="9edcb-110">Default is always true, individual resources and overridet the default.</span></span>
* <span data-ttu-id="9edcb-111">Foi adicionado ps1xml a Common.Storage</span><span class="sxs-lookup"><span data-stu-id="9edcb-111">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9edcb-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9edcb-112">Azure.Storage</span></span>
* <span data-ttu-id="9edcb-113">Suporte para get Storage Context a partir de DefaulfProfile</span><span class="sxs-lookup"><span data-stu-id="9edcb-113">Support get Storage Context from DefaulfProfile</span></span>
* <span data-ttu-id="9edcb-114">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets.</span><span class="sxs-lookup"><span data-stu-id="9edcb-114">Add Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9edcb-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9edcb-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9edcb-116">Problema https://github.com/Azure/azure-powershell/issues/6370 corrigido</span><span class="sxs-lookup"><span data-stu-id="9edcb-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="9edcb-117">Foi corrigido um erro no Automapper para traduzir PsApiManagementApi para ApiContract</span><span class="sxs-lookup"><span data-stu-id="9edcb-117">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="9edcb-118">Problema https://github.com/Azure/azure-powershell/issues/6515 corrigido</span><span class="sxs-lookup"><span data-stu-id="9edcb-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="9edcb-119">Foi corrigido um erro em File.Save para não sobrecarregar com Tipo de Codificação</span><span class="sxs-lookup"><span data-stu-id="9edcb-119">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="9edcb-120">Problema https://github.com/Azure/azure-powershell/issues/6560 corrigido</span><span class="sxs-lookup"><span data-stu-id="9edcb-120">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="9edcb-121">Atualizado para a versão 4.0.3 do Nuget, que corrige a exceção de padrão em apiId</span><span class="sxs-lookup"><span data-stu-id="9edcb-121">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9edcb-122">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9edcb-122">AzureRM.Compute</span></span>
* <span data-ttu-id="9edcb-123">Corrigido problema com a falha na criação de uma vm com DiskFileParameterSet em New-AzureRmVm devido a mudança de nome do tipo de conta de armazenamento PremiumLRS.</span><span class="sxs-lookup"><span data-stu-id="9edcb-123">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="9edcb-124">Foi corrigido o cmdlet Invoke-AzureRmVMRunCommand</span><span class="sxs-lookup"><span data-stu-id="9edcb-124">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="9edcb-125">Foi atualizado Get-AzureRmAvailabilitySet para permitir a listagem de todos os conjuntos de disponibilidade numa subscrição.</span><span class="sxs-lookup"><span data-stu-id="9edcb-125">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="9edcb-126">(O parâmetro ResouceGroupName é agora opcional.)</span><span class="sxs-lookup"><span data-stu-id="9edcb-126">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="9edcb-127">Atualização de SimpleParameterSet de “New-AzureRmVm” para permitir a Rede Acelerada em vms elegíveis.</span><span class="sxs-lookup"><span data-stu-id="9edcb-127">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="9edcb-128">Atualização do conjunto de parâmetros simples New-AzureRmVmss para falhar a criação de vms quando um LB especificado por um utilizador já existir.</span><span class="sxs-lookup"><span data-stu-id="9edcb-128">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="9edcb-129">Atualização de exemplo para New-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="9edcb-129">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="9edcb-130">Adição de exemplo para “New-AzureRmVM”</span><span class="sxs-lookup"><span data-stu-id="9edcb-130">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="9edcb-131">Atualização da descrição para Set-AzureRmVMOSDisk</span><span class="sxs-lookup"><span data-stu-id="9edcb-131">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="9edcb-132">Atualização do Exemplo 1 para Set-AzureRmVMBginfoExtension para corrigir a ortografia e o prefixo.</span><span class="sxs-lookup"><span data-stu-id="9edcb-132">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9edcb-133">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9edcb-133">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9edcb-134">Atualização da versão do SDK .NET do ADF para a 1.1.0.</span><span class="sxs-lookup"><span data-stu-id="9edcb-134">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="9edcb-135">Suporte para partilha de runtime de integração autoalojado em várias fábricas de dados</span><span class="sxs-lookup"><span data-stu-id="9edcb-135">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="9edcb-136">Adicionado parâmetro novo -SharedIntegrationRuntimeResourceId ao cmdlet Set-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="9edcb-136">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="9edcb-137">Adicionado o parâmetro opcional novo -LinkedDataFactoryName ao cmdlet Remove-AzureRmDataFactoryV2IntegrationRuntime.</span><span class="sxs-lookup"><span data-stu-id="9edcb-137">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9edcb-138">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9edcb-138">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9edcb-139">Atualizada a versão do SDK DataPlane (Microsoft.Azure.DataLake.Store) para a 1.1.9</span><span class="sxs-lookup"><span data-stu-id="9edcb-139">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9edcb-140">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9edcb-140">AzureRM.EventHub</span></span>
* <span data-ttu-id="9edcb-141">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="9edcb-141">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="9edcb-142">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9edcb-142">AzureRM.Insights</span></span>
* <span data-ttu-id="9edcb-143">Correção da formatação de OutputType nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="9edcb-143">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="9edcb-144">Utilização da pré-visualização do SDK Microsoft.Azure.Management.Monitor SDK 0.19.1</span><span class="sxs-lookup"><span data-stu-id="9edcb-144">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9edcb-145">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9edcb-145">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9edcb-146">Correção de problema em Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="9edcb-146">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9edcb-147">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9edcb-147">AzureRM.Network</span></span>
* <span data-ttu-id="9edcb-148">Adicionados exemplos para os cmdlets LoadBalancerInboundNatPoolConfig.</span><span class="sxs-lookup"><span data-stu-id="9edcb-148">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9edcb-149">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9edcb-149">AzureRM.Resources</span></span>
* <span data-ttu-id="9edcb-150">Corrigido problema ao fornecer o nome e o valor da etiqueta para “Get-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="9edcb-150">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="9edcb-151">Correção de cenário de piping com “Set-AzureRmResource”</span><span class="sxs-lookup"><span data-stu-id="9edcb-151">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9edcb-152">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9edcb-152">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9edcb-153">Atualização de piping para InputObject e ResourceId em cmdlets de remoção</span><span class="sxs-lookup"><span data-stu-id="9edcb-153">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="9edcb-154">corrigidos problemas novos</span><span class="sxs-lookup"><span data-stu-id="9edcb-154">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="9edcb-155">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9edcb-155">AzureRM.Sql</span></span>
* <span data-ttu-id="9edcb-156">Adição de suporte para Proteção Avançada contra Ameaças do Servidor com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9edcb-156">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="9edcb-157">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9edcb-157">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="9edcb-158">Adição de suporte para Avaliação de Vulnerabilidades com os seguintes cmdlets:</span><span class="sxs-lookup"><span data-stu-id="9edcb-158">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="9edcb-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="9edcb-159">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="9edcb-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="9edcb-160">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="9edcb-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="9edcb-161">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="9edcb-162">Corrigido exemplo em Remove-AzureRmSqlServerFirewallRule</span><span class="sxs-lookup"><span data-stu-id="9edcb-162">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="9edcb-163">Corrigido processamento incorreto de datetime para culturas base diferentes de eua em Get-AzureSqlSyncGroupLog</span><span class="sxs-lookup"><span data-stu-id="9edcb-163">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9edcb-164">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9edcb-164">AzureRM.Storage</span></span>
* <span data-ttu-id="9edcb-165">Adição de Ps1XmlAttribute para propriedades de tipos de saídas de cmdlets</span><span class="sxs-lookup"><span data-stu-id="9edcb-165">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="9edcb-166">Mostrar saída de cmdlet StorageAccount na vista de tabela</span><span class="sxs-lookup"><span data-stu-id="9edcb-166">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="9edcb-167">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9edcb-167">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="9edcb-168">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9edcb-168">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="9edcb-169">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9edcb-169">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="9edcb-170">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="9edcb-170">AzureRM.Tags</span></span>
* <span data-ttu-id="9edcb-171">Remoção de declaração incorreta da ajuda do cmdlet Tag</span><span class="sxs-lookup"><span data-stu-id="9edcb-171">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="9edcb-172">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="9edcb-172">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9edcb-173">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9edcb-173">AzureRM.Profile</span></span>
* <span data-ttu-id="9edcb-174">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="9edcb-174">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9edcb-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9edcb-175">Azure.Storage</span></span>
* <span data-ttu-id="9edcb-176">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="9edcb-176">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="9edcb-177">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="9edcb-177">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="9edcb-178">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="9edcb-178">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9edcb-179">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9edcb-179">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9edcb-180">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="9edcb-180">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="9edcb-181">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="9edcb-181">AzureRM.Automation</span></span>
* <span data-ttu-id="9edcb-182">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="9edcb-182">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9edcb-183">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9edcb-183">AzureRM.Compute</span></span>
* <span data-ttu-id="9edcb-184">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="9edcb-184">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="9edcb-185">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="9edcb-185">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="9edcb-186">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="9edcb-186">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="9edcb-187">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="9edcb-187">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="9edcb-188">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="9edcb-188">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9edcb-189">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9edcb-189">AzureRM.EventHub</span></span>
* <span data-ttu-id="9edcb-190">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="9edcb-190">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9edcb-191">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9edcb-191">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9edcb-192">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="9edcb-192">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="9edcb-193">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9edcb-193">AzureRM.LogicApp</span></span>
* <span data-ttu-id="9edcb-194">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="9edcb-194">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9edcb-195">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9edcb-195">AzureRM.Network</span></span>
* <span data-ttu-id="9edcb-196">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="9edcb-196">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="9edcb-197">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="9edcb-197">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="9edcb-198">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="9edcb-198">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="9edcb-199">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="9edcb-199">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="9edcb-200">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="9edcb-200">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="9edcb-201">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="9edcb-201">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="9edcb-202">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="9edcb-202">AzureRM.Relay</span></span>
* <span data-ttu-id="9edcb-203">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="9edcb-203">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9edcb-204">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9edcb-204">AzureRM.Resources</span></span>
* <span data-ttu-id="9edcb-205">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="9edcb-205">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="9edcb-206">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="9edcb-206">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="9edcb-207">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="9edcb-207">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="9edcb-208">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="9edcb-208">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="9edcb-209">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="9edcb-209">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9edcb-210">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9edcb-210">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9edcb-211">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="9edcb-211">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="9edcb-212">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="9edcb-212">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="9edcb-213">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9edcb-213">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9edcb-214">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9edcb-214">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9edcb-215">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9edcb-215">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9edcb-216">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9edcb-216">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9edcb-217">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9edcb-217">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="9edcb-218">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="9edcb-218">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9edcb-219">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9edcb-219">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9edcb-220">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="9edcb-220">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9edcb-221">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9edcb-221">AzureRM.Sql</span></span>
* <span data-ttu-id="9edcb-222">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="9edcb-222">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="9edcb-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="9edcb-223">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="9edcb-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="9edcb-224">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9edcb-225">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9edcb-225">AzureRM.Websites</span></span>
* <span data-ttu-id="9edcb-226">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="9edcb-226">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="9edcb-227">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="9edcb-227">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="9edcb-228">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="9edcb-228">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="9edcb-229">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="9edcb-229">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9edcb-230">Geral</span><span class="sxs-lookup"><span data-stu-id="9edcb-230">General</span></span>
* <span data-ttu-id="9edcb-231">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="9edcb-231">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9edcb-232">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9edcb-232">AzureRM.Profile</span></span>
* <span data-ttu-id="9edcb-233">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="9edcb-233">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9edcb-234">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9edcb-234">AzureRM.Compute</span></span>
* <span data-ttu-id="9edcb-235">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="9edcb-235">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="9edcb-236">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="9edcb-236">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="9edcb-237">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="9edcb-237">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="9edcb-238">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="9edcb-238">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="9edcb-239">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-239">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="9edcb-240">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-240">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="9edcb-241">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-241">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="9edcb-242">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="9edcb-242">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="9edcb-243">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="9edcb-243">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="9edcb-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9edcb-244">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9edcb-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9edcb-245">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9edcb-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9edcb-246">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9edcb-247">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9edcb-247">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9edcb-248">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="9edcb-248">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="9edcb-249">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="9edcb-249">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9edcb-250">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="9edcb-250">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="9edcb-251">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="9edcb-251">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9edcb-252">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9edcb-252">AzureRM.EventHub</span></span>
* <span data-ttu-id="9edcb-253">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="9edcb-253">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="9edcb-254">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="9edcb-254">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="9edcb-255">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="9edcb-255">Provided Default Parameter set.</span></span>
* <span data-ttu-id="9edcb-256">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="9edcb-256">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9edcb-257">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9edcb-257">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9edcb-258">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="9edcb-258">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9edcb-259">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9edcb-259">AzureRM.Network</span></span>
* <span data-ttu-id="9edcb-260">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="9edcb-260">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="9edcb-261">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="9edcb-261">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="9edcb-262">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="9edcb-262">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9edcb-263">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="9edcb-263">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9edcb-264">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9edcb-264">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9edcb-265">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9edcb-265">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9edcb-266">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9edcb-266">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9edcb-267">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="9edcb-267">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="9edcb-268">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="9edcb-268">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="9edcb-269">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="9edcb-269">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9edcb-270">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9edcb-270">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9edcb-271">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="9edcb-271">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="9edcb-272">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="9edcb-272">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="9edcb-273">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="9edcb-273">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9edcb-274">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9edcb-274">AzureRM.Resources</span></span>
* <span data-ttu-id="9edcb-275">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="9edcb-275">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="9edcb-276">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9edcb-276">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="9edcb-277">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9edcb-277">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="9edcb-278">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="9edcb-278">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="9edcb-279">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9edcb-279">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="9edcb-280">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9edcb-280">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9edcb-281">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="9edcb-281">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9edcb-282">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="9edcb-282">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="9edcb-283">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9edcb-283">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9edcb-284">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="9edcb-284">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9edcb-285">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="9edcb-285">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="9edcb-286">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="9edcb-286">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="9edcb-287">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="9edcb-287">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="9edcb-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9edcb-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9edcb-289">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="9edcb-289">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9edcb-290">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9edcb-290">AzureRM.Sql</span></span>
* <span data-ttu-id="9edcb-291">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="9edcb-291">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="9edcb-292">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="9edcb-292">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="9edcb-293">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9edcb-293">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9edcb-294">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9edcb-294">AzureRM.Profile</span></span>
* <span data-ttu-id="9edcb-295">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="9edcb-295">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="9edcb-296">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="9edcb-296">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9edcb-297">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9edcb-297">Azure.Storage</span></span>
* <span data-ttu-id="9edcb-298">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="9edcb-298">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9edcb-299">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9edcb-299">AzureRM.Compute</span></span>
* <span data-ttu-id="9edcb-300">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="9edcb-300">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="9edcb-301">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="9edcb-301">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="9edcb-302">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9edcb-302">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9edcb-303">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9edcb-303">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9edcb-304">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="9edcb-304">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="9edcb-305">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="9edcb-305">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="9edcb-306">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9edcb-306">Start-AzureRmVM</span></span>
    - <span data-ttu-id="9edcb-307">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9edcb-307">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="9edcb-308">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9edcb-308">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="9edcb-309">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9edcb-309">Set-AzureRmVM</span></span>
    - <span data-ttu-id="9edcb-310">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="9edcb-310">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="9edcb-311">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-311">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="9edcb-312">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="9edcb-312">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="9edcb-313">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="9edcb-313">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="9edcb-314">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-314">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="9edcb-315">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-315">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="9edcb-316">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-316">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="9edcb-317">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9edcb-317">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="9edcb-318">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="9edcb-318">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="9edcb-319">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9edcb-319">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9edcb-320">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="9edcb-320">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="9edcb-321">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9edcb-321">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9edcb-322">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="9edcb-322">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="9edcb-323">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="9edcb-323">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="9edcb-324">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="9edcb-324">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="9edcb-325">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="9edcb-325">AzureRM.EventGrid</span></span>
* <span data-ttu-id="9edcb-326">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="9edcb-326">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9edcb-327">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9edcb-327">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9edcb-328">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="9edcb-328">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="9edcb-329">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="9edcb-329">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="9edcb-330">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="9edcb-330">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="9edcb-331">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="9edcb-331">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="9edcb-332">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="9edcb-332">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9edcb-333">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9edcb-333">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9edcb-334">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="9edcb-334">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="9edcb-335">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="9edcb-335">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9edcb-336">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9edcb-336">AzureRM.Sql</span></span>
* <span data-ttu-id="9edcb-337">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="9edcb-337">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9edcb-338">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9edcb-338">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9edcb-339">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="9edcb-339">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9edcb-340">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9edcb-340">AzureRM.Websites</span></span>
* <span data-ttu-id="9edcb-341">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="9edcb-341">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="9edcb-342">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="9edcb-342">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="9edcb-343">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9edcb-343">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="9edcb-344">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9edcb-344">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="9edcb-345">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="9edcb-345">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="9edcb-346">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9edcb-346">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9edcb-347">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9edcb-347">AzureRM.Profile</span></span>
* <span data-ttu-id="9edcb-348">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="9edcb-348">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9edcb-349">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9edcb-349">AzureRM.Compute</span></span>
* <span data-ttu-id="9edcb-350">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="9edcb-350">VMSS VM Update feature</span></span>
    - <span data-ttu-id="9edcb-351">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="9edcb-351">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="9edcb-352">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="9edcb-352">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9edcb-353">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9edcb-353">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9edcb-354">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="9edcb-354">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="9edcb-355">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="9edcb-355">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="9edcb-356">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="9edcb-356">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="9edcb-357">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="9edcb-357">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="9edcb-358">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="9edcb-358">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="9edcb-359">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9edcb-359">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9edcb-360">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="9edcb-360">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="9edcb-361">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9edcb-361">AzureRM.Network</span></span>
* <span data-ttu-id="9edcb-362">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="9edcb-362">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9edcb-363">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9edcb-363">AzureRM.Resources</span></span>
* <span data-ttu-id="9edcb-364">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="9edcb-364">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="9edcb-365">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="9edcb-365">AzureRM.Scheduler</span></span>
* <span data-ttu-id="9edcb-366">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="9edcb-366">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="9edcb-367">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9edcb-367">AzureRM.Sql</span></span>
* <span data-ttu-id="9edcb-368">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="9edcb-368">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="9edcb-369">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9edcb-369">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9edcb-370">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9edcb-370">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9edcb-371">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9edcb-371">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9edcb-372">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9edcb-372">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9edcb-373">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9edcb-373">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9edcb-374">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9edcb-374">AzureRM.Websites</span></span>
* <span data-ttu-id="9edcb-375">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="9edcb-375">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="9edcb-376">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="9edcb-376">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9edcb-377">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9edcb-377">AzureRM.Profile</span></span>
* <span data-ttu-id="9edcb-378">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="9edcb-378">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9edcb-379">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9edcb-379">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9edcb-380">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="9edcb-380">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9edcb-381">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9edcb-381">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9edcb-382">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="9edcb-382">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="9edcb-383">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9edcb-383">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="9edcb-384">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="9edcb-384">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="9edcb-385">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="9edcb-385">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="9edcb-386">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="9edcb-386">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="9edcb-387">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="9edcb-387">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="9edcb-388">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="9edcb-388">Added support for MSI identity</span></span>
* <span data-ttu-id="9edcb-389">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="9edcb-389">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="9edcb-390">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="9edcb-390">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="9edcb-391">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="9edcb-391">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="9edcb-392">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="9edcb-392">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="9edcb-393">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="9edcb-393">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="9edcb-394">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="9edcb-394">AzureRM.Batch</span></span>
* <span data-ttu-id="9edcb-395">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="9edcb-395">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="9edcb-396">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="9edcb-396">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="9edcb-397">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9edcb-397">AzureRM.Consumption</span></span>
* <span data-ttu-id="9edcb-398">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="9edcb-398">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9edcb-399">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9edcb-399">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9edcb-400">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="9edcb-400">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9edcb-401">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9edcb-401">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="9edcb-402">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9edcb-402">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="9edcb-403">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9edcb-403">AzureRM.Network</span></span>
* <span data-ttu-id="9edcb-404">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="9edcb-404">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="9edcb-405">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="9edcb-405">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="9edcb-406">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="9edcb-406">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="9edcb-407">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9edcb-407">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="9edcb-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9edcb-408">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9edcb-409">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9edcb-409">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="9edcb-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9edcb-410">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9edcb-411">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="9edcb-411">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="9edcb-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9edcb-412">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9edcb-413">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9edcb-413">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9edcb-414">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="9edcb-414">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9edcb-415">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9edcb-415">AzureRM.Sql</span></span>
* <span data-ttu-id="9edcb-416">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="9edcb-416">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="9edcb-417">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="9edcb-417">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="9edcb-418">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="9edcb-418">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="9edcb-419">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="9edcb-419">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="9edcb-420">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="9edcb-420">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="9edcb-421">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9edcb-421">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9edcb-422">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9edcb-422">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9edcb-423">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9edcb-423">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9edcb-424">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9edcb-424">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9edcb-425">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9edcb-425">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9edcb-426">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9edcb-426">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9edcb-427">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="9edcb-427">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>