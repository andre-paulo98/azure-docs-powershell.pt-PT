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
ms.openlocfilehash: e9fa2d75c1c4e6ffaa2f7dd8e400f5b13dd4527d
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110488"
---
# <a name="release-notes"></a><span data-ttu-id="25660-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="25660-103">Release notes</span></span>

<span data-ttu-id="25660-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="25660-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="650---july-2018"></a><span data-ttu-id="25660-105">6.5.0 - Julho de 2018</span><span class="sxs-lookup"><span data-stu-id="25660-105">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="25660-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="25660-106">AzureRM.Profile</span></span>
* <span data-ttu-id="25660-107">Ajuda atualizada para "Get-AzureRmContextAutosaveSetting"</span><span class="sxs-lookup"><span data-stu-id="25660-107">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="25660-108">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="25660-108">Azure.Storage</span></span>
* <span data-ttu-id="25660-109">Suporte de Carregamento de Blob ou Ficheiro com token Sas apenas de escrita</span><span class="sxs-lookup"><span data-stu-id="25660-109">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="25660-110">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="25660-110">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="25660-111">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="25660-111">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="25660-112">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="25660-112">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="25660-113">Adicionar propriedade ResourceGroupName obrigatória ao AS.</span><span class="sxs-lookup"><span data-stu-id="25660-113">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="25660-114">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="25660-114">AzureRM.Automation</span></span>
* <span data-ttu-id="25660-115">Atualizar ajuda e adicionar exemplo a "New-AzureRMAutomationSchedule"</span><span class="sxs-lookup"><span data-stu-id="25660-115">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="25660-116">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="25660-116">AzureRM.Compute</span></span>
* <span data-ttu-id="25660-117">Adicionar parâmetro -Tag a Update/New-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="25660-117">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="25660-118">Adicionar exemplo a "Add-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="25660-118">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="25660-119">Adicionar exemplos a "Remove-AzureRmVmssExtension"</span><span class="sxs-lookup"><span data-stu-id="25660-119">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="25660-120">Atualizar ajuda para "Set-AzureRmVMAccessExtension"</span><span class="sxs-lookup"><span data-stu-id="25660-120">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="25660-121">Atualizar SimpleParameterSet para New-AzureRmVmss para definir SinglePlacementGroup como falso por predefinição e adicionar parâmetro do comutador "SinglePlacementGroup" que permite ao utilizador criar a VMSS num único grupo de posicionamento.</span><span class="sxs-lookup"><span data-stu-id="25660-121">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="25660-122">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="25660-122">AzureRM.EventHub</span></span>
* <span data-ttu-id="25660-123">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSEventHubDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="25660-123">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="25660-124">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="25660-124">AzureRM.KeyVault</span></span>
* <span data-ttu-id="25660-125">Atualizar mensagem de erro para Set-AzureRmKeyVaultAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="25660-125">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="25660-126">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="25660-126">AzureRM.LogicApp</span></span>
* <span data-ttu-id="25660-127">Erro "a definição do parâmetro não foi resolvida" corrigido no New-AzureRmLogicApp</span><span class="sxs-lookup"><span data-stu-id="25660-127">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="25660-128">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="25660-128">AzureRM.Network</span></span>
* <span data-ttu-id="25660-129">Ativar peering entre várias Redes Virtuais em vários Inquilinos para Set/Add-AzureRmVirtualNetworkPeering</span><span class="sxs-lookup"><span data-stu-id="25660-129">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="25660-130">Cmdlets abaixo atualizados para Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="25660-130">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="25660-131">New-AzureRmApplicationGateway: Sinalizador EnableFIPS e suporte de Zonas adicionados</span><span class="sxs-lookup"><span data-stu-id="25660-131">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="25660-132">New-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="25660-132">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="25660-133">Set-AzureRmApplicationGatewaySku: novos skus Standard_v2 e WAF_v2 adicionados</span><span class="sxs-lookup"><span data-stu-id="25660-133">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="25660-134">Cmdlets RouteTable regenerados com a versão do gerador mais recente</span><span class="sxs-lookup"><span data-stu-id="25660-134">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="25660-135">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="25660-135">AzureRM.Relay</span></span>
* <span data-ttu-id="25660-136">Ficheiros de marcação atualizados, correção para o problema do nome do parâmetro no exemplo</span><span class="sxs-lookup"><span data-stu-id="25660-136">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="25660-137">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="25660-137">AzureRM.Resources</span></span>
* <span data-ttu-id="25660-138">Cmdlets Roleassignment e roledefinition atualizados:</span><span class="sxs-lookup"><span data-stu-id="25660-138">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="25660-139">Remover chamadas de roledefinition extra feitas como parte da paginação.</span><span class="sxs-lookup"><span data-stu-id="25660-139">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="25660-140">Corrigir cmdlet Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25660-140">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="25660-141">Corrigir funcionalidade do parâmetro do comando -ExpandPrincipalGroups</span><span class="sxs-lookup"><span data-stu-id="25660-141">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="25660-142">Corrigir problema com "Get-AzureRmResource" em que o parâmetro "-ResourceType" era sensível a maiúsculas e minúsculas</span><span class="sxs-lookup"><span data-stu-id="25660-142">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="25660-143">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="25660-143">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="25660-144">Parâmetro top e skip adicionados para listar os cmdlets</span><span class="sxs-lookup"><span data-stu-id="25660-144">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="25660-145">Cmdlets de migração do Espaço de Nomes Standard a Premium:</span><span class="sxs-lookup"><span data-stu-id="25660-145">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="25660-146">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="25660-146">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="25660-147">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="25660-147">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="25660-148">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="25660-148">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="25660-149">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="25660-149">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="25660-150">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="25660-150">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="25660-151">Adicionada uma propriedade só de leitura "PendingReplicationOperationsCount" à classe PSServiceBusDRConfigurationAttributes, o que concede a contagem de operações de replicação pendente enquanto está em curso</span><span class="sxs-lookup"><span data-stu-id="25660-151">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="25660-152">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="25660-152">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="25660-153">Exemplo de atualização para "New-AzureRmServiceFabricCluster"</span><span class="sxs-lookup"><span data-stu-id="25660-153">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="25660-154">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="25660-154">AzureRM.Sql</span></span>
* <span data-ttu-id="25660-155">Adicionar novos Cmdlets ao Management.Sql para permitir aos clientes adicionarem o Certificado TDE à instância do Sql Server ou uma Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="25660-155">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="25660-156">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="25660-156">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="25660-157">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="25660-157">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="25660-158">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="25660-158">AzureRM.Websites</span></span>
* <span data-ttu-id="25660-159">`Set-AzureRmWebApp -AssignIdentity` e  `Set-AzureRmWebAppSlot -AssignIdentity` quando definidos como falso também irão agora remover a propriedade de Identidade da etiqueta de pré-visualização object.Removing do site.</span><span class="sxs-lookup"><span data-stu-id="25660-159">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="25660-160">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` exemplo atualizado</span><span class="sxs-lookup"><span data-stu-id="25660-160">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="25660-161">`Set-AzureRmWebApp -PhpVersion` suporta como uma versão válida do PHP</span><span class="sxs-lookup"><span data-stu-id="25660-161">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="25660-162">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="25660-162">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="25660-163">Geral</span><span class="sxs-lookup"><span data-stu-id="25660-163">General</span></span>
* <span data-ttu-id="25660-164">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="25660-164">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="25660-165">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="25660-165">AzureRM.Profile</span></span>
* <span data-ttu-id="25660-166">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="25660-166">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="25660-167">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="25660-167">AzureRM.Compute</span></span>
* <span data-ttu-id="25660-168">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="25660-168">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="25660-169">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="25660-169">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="25660-170">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="25660-170">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="25660-171">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="25660-171">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="25660-172">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="25660-172">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="25660-173">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="25660-173">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="25660-174">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="25660-174">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="25660-175">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="25660-175">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="25660-176">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="25660-176">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="25660-177">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="25660-177">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="25660-178">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="25660-178">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="25660-179">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="25660-179">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="25660-180">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="25660-180">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="25660-181">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="25660-181">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="25660-182">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="25660-182">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="25660-183">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="25660-183">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="25660-184">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="25660-184">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="25660-185">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="25660-185">AzureRM.EventHub</span></span>
* <span data-ttu-id="25660-186">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="25660-186">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="25660-187">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="25660-187">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="25660-188">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="25660-188">Provided Default Parameter set.</span></span>
* <span data-ttu-id="25660-189">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="25660-189">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="25660-190">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="25660-190">AzureRM.KeyVault</span></span>
* <span data-ttu-id="25660-191">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="25660-191">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="25660-192">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="25660-192">AzureRM.Network</span></span>
* <span data-ttu-id="25660-193">Apresentação de novos SKUs para VirtualNetworkGateways com redundância entre zonas</span><span class="sxs-lookup"><span data-stu-id="25660-193">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="25660-194">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="25660-194">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="25660-195">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="25660-195">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="25660-196">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="25660-196">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="25660-197">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="25660-197">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="25660-198">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="25660-198">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="25660-199">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="25660-199">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="25660-200">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="25660-200">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="25660-201">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="25660-201">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="25660-202">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="25660-202">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="25660-203">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="25660-203">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="25660-204">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="25660-204">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="25660-205">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="25660-205">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="25660-206">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="25660-206">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="25660-207">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="25660-207">AzureRM.Resources</span></span>
* <span data-ttu-id="25660-208">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="25660-208">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="25660-209">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="25660-209">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="25660-210">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="25660-210">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="25660-211">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="25660-211">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="25660-212">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="25660-212">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="25660-213">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="25660-213">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="25660-214">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="25660-214">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="25660-215">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="25660-215">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="25660-216">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="25660-216">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="25660-217">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="25660-217">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="25660-218">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="25660-218">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="25660-219">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="25660-219">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="25660-220">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="25660-220">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="25660-221">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="25660-221">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="25660-222">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="25660-222">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="25660-223">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="25660-223">AzureRM.Sql</span></span>
* <span data-ttu-id="25660-224">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="25660-224">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="25660-225">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="25660-225">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="25660-226">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="25660-226">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="25660-227">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="25660-227">AzureRM.Profile</span></span>
* <span data-ttu-id="25660-228">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="25660-228">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="25660-229">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="25660-229">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="25660-230">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="25660-230">Azure.Storage</span></span>
* <span data-ttu-id="25660-231">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="25660-231">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="25660-232">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="25660-232">AzureRM.Compute</span></span>
* <span data-ttu-id="25660-233">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="25660-233">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="25660-234">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="25660-234">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="25660-235">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="25660-235">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="25660-236">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="25660-236">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="25660-237">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="25660-237">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="25660-238">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="25660-238">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="25660-239">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="25660-239">Start-AzureRmVM</span></span>
    - <span data-ttu-id="25660-240">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="25660-240">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="25660-241">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="25660-241">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="25660-242">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="25660-242">Set-AzureRmVM</span></span>
    - <span data-ttu-id="25660-243">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="25660-243">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="25660-244">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="25660-244">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="25660-245">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="25660-245">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="25660-246">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="25660-246">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="25660-247">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="25660-247">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="25660-248">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="25660-248">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="25660-249">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="25660-249">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="25660-250">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="25660-250">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="25660-251">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="25660-251">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="25660-252">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="25660-252">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="25660-253">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="25660-253">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="25660-254">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="25660-254">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="25660-255">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="25660-255">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="25660-256">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="25660-256">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="25660-257">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="25660-257">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="25660-258">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="25660-258">AzureRM.EventGrid</span></span>
* <span data-ttu-id="25660-259">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="25660-259">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="25660-260">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="25660-260">AzureRM.KeyVault</span></span>
* <span data-ttu-id="25660-261">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="25660-261">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="25660-262">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="25660-262">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="25660-263">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="25660-263">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="25660-264">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="25660-264">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="25660-265">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="25660-265">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="25660-266">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="25660-266">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="25660-267">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="25660-267">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="25660-268">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="25660-268">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="25660-269">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="25660-269">AzureRM.Sql</span></span>
* <span data-ttu-id="25660-270">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="25660-270">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="25660-271">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="25660-271">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="25660-272">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="25660-272">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="25660-273">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="25660-273">AzureRM.Websites</span></span>
* <span data-ttu-id="25660-274">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="25660-274">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="25660-275">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="25660-275">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="25660-276">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="25660-276">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="25660-277">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="25660-277">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="25660-278">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="25660-278">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="25660-279">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="25660-279">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="25660-280">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="25660-280">AzureRM.Profile</span></span>
* <span data-ttu-id="25660-281">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="25660-281">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="25660-282">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="25660-282">AzureRM.Compute</span></span>
* <span data-ttu-id="25660-283">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="25660-283">VMSS VM Update feature</span></span>
    - <span data-ttu-id="25660-284">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="25660-284">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="25660-285">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="25660-285">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="25660-286">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="25660-286">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="25660-287">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="25660-287">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="25660-288">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="25660-288">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="25660-289">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="25660-289">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="25660-290">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="25660-290">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="25660-291">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="25660-291">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="25660-292">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="25660-292">AzureRM.KeyVault</span></span>
* <span data-ttu-id="25660-293">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="25660-293">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="25660-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="25660-294">AzureRM.Network</span></span>
* <span data-ttu-id="25660-295">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="25660-295">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="25660-296">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="25660-296">AzureRM.Resources</span></span>
* <span data-ttu-id="25660-297">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="25660-297">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="25660-298">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="25660-298">AzureRM.Scheduler</span></span>
* <span data-ttu-id="25660-299">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="25660-299">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="25660-300">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="25660-300">AzureRM.Sql</span></span>
* <span data-ttu-id="25660-301">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="25660-301">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="25660-302">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="25660-302">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="25660-303">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="25660-303">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="25660-304">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="25660-304">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="25660-305">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="25660-305">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="25660-306">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="25660-306">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="25660-307">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="25660-307">AzureRM.Websites</span></span>
* <span data-ttu-id="25660-308">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="25660-308">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="25660-309">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="25660-309">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="25660-310">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="25660-310">AzureRM.Profile</span></span>
* <span data-ttu-id="25660-311">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="25660-311">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="25660-312">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="25660-312">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="25660-313">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="25660-313">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="25660-314">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="25660-314">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="25660-315">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="25660-315">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="25660-316">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="25660-316">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="25660-317">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="25660-317">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="25660-318">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="25660-318">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="25660-319">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="25660-319">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="25660-320">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="25660-320">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="25660-321">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="25660-321">Added support for MSI identity</span></span>
* <span data-ttu-id="25660-322">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="25660-322">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="25660-323">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="25660-323">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="25660-324">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="25660-324">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="25660-325">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="25660-325">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="25660-326">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="25660-326">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="25660-327">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="25660-327">AzureRM.Batch</span></span>
* <span data-ttu-id="25660-328">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="25660-328">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="25660-329">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="25660-329">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="25660-330">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="25660-330">AzureRM.Consumption</span></span>
* <span data-ttu-id="25660-331">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="25660-331">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="25660-332">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="25660-332">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="25660-333">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="25660-333">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="25660-334">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="25660-334">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="25660-335">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="25660-335">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="25660-336">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="25660-336">AzureRM.Network</span></span>
* <span data-ttu-id="25660-337">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="25660-337">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="25660-338">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="25660-338">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="25660-339">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="25660-339">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="25660-340">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="25660-340">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="25660-341">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="25660-341">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="25660-342">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="25660-342">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="25660-343">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="25660-343">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="25660-344">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="25660-344">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="25660-345">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="25660-345">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="25660-346">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="25660-346">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="25660-347">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="25660-347">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="25660-348">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="25660-348">AzureRM.Sql</span></span>
* <span data-ttu-id="25660-349">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="25660-349">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="25660-350">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="25660-350">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="25660-351">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="25660-351">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="25660-352">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="25660-352">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="25660-353">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="25660-353">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="25660-354">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="25660-354">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="25660-355">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="25660-355">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="25660-356">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="25660-356">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="25660-357">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="25660-357">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="25660-358">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="25660-358">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="25660-359">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="25660-359">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="25660-360">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="25660-360">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>