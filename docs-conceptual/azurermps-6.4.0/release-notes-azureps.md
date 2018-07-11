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
ms.openlocfilehash: 255e26aea5ea3cea866faa0d095cdf643c8ef0a8
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406488"
---
# <a name="release-notes"></a><span data-ttu-id="9a171-103">Notas de versão</span><span class="sxs-lookup"><span data-stu-id="9a171-103">Release notes</span></span>

<span data-ttu-id="9a171-104">Esta é a lista de alterações feitas ao Azure PowerShell nesta versão.</span><span class="sxs-lookup"><span data-stu-id="9a171-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="640---july-2018"></a><span data-ttu-id="9a171-105">6.4.0 - julho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a171-105">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9a171-106">Geral</span><span class="sxs-lookup"><span data-stu-id="9a171-106">General</span></span>
* <span data-ttu-id="9a171-107">Correção da formatação de OutputType nos ficheiros de ajuda para a maioria dos módulos</span><span class="sxs-lookup"><span data-stu-id="9a171-107">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9a171-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a171-108">AzureRM.Profile</span></span>
* <span data-ttu-id="9a171-109">Foi adicionado o atributo Ps1Xml aos tipos de saída básicos</span><span class="sxs-lookup"><span data-stu-id="9a171-109">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a171-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a171-110">AzureRM.Compute</span></span>
* <span data-ttu-id="9a171-111">Funcionalidade de Etiqueta IP para VMSS</span><span class="sxs-lookup"><span data-stu-id="9a171-111">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="9a171-112">Foi adicionado o cmdlet "New-AzureRmVmssIpTagConfig"</span><span class="sxs-lookup"><span data-stu-id="9a171-112">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="9a171-113">Foi adicionado o parâmetro IpTag a New-AzureRmVmssIpConfig</span><span class="sxs-lookup"><span data-stu-id="9a171-113">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="9a171-114">Funcionalidade de Reversão do SO automática para VMSS</span><span class="sxs-lookup"><span data-stu-id="9a171-114">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="9a171-115">Foram adicionados parâmetros DisableAutoRollback a New-AzureRmVmssConfig e Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a171-115">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="9a171-116">Funcionalidade de Histórico de Atualização do SO para Vmss</span><span class="sxs-lookup"><span data-stu-id="9a171-116">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="9a171-117">Foi adicionado o parâmetro OSUpgradeHistory a Get-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a171-117">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="9a171-118">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="9a171-118">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="9a171-119">Adição de suporte para ACLs de Catálogo através dos seguintes comandos:</span><span class="sxs-lookup"><span data-stu-id="9a171-119">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="9a171-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a171-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9a171-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a171-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9a171-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a171-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9a171-123">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9a171-123">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9a171-124">Adição de suporte ao cancelamento e de controlo do progresso para Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry e Set-AzureRmDataLakeStoreItemAcl</span><span class="sxs-lookup"><span data-stu-id="9a171-124">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="9a171-125">Adição de suporte ao cancelamento para Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="9a171-125">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9a171-126">Correção da remoção de mensagens de depuração para cmdlets que realizam operações recursivas</span><span class="sxs-lookup"><span data-stu-id="9a171-126">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="9a171-127">Correção da localização de teste de cmdlets do DataLake</span><span class="sxs-lookup"><span data-stu-id="9a171-127">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9a171-128">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9a171-128">AzureRM.EventHub</span></span>
* <span data-ttu-id="9a171-129">Adição do parâmetro Optional MaxCount aos cmdlets Get-AzureRmEventHub e Get-AzureRmEventHubConsumerGroup de List Operations</span><span class="sxs-lookup"><span data-stu-id="9a171-129">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="9a171-130">Correção de problema no cmdlet New-AzureRmEventHub, no qual era necessário, pelo menos, um parâmetro durante a criação de um novo EventHub.</span><span class="sxs-lookup"><span data-stu-id="9a171-130">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="9a171-131">Conjunto de Parâmetros Predefinidos fornecido.</span><span class="sxs-lookup"><span data-stu-id="9a171-131">Provided Default Parameter set.</span></span>
* <span data-ttu-id="9a171-132">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmEventHubKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="9a171-132">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9a171-133">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a171-133">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a171-134">Correção de problema no qual todos os recursos eram devolvidos por Get-AzureRmKeyVault -Tag</span><span class="sxs-lookup"><span data-stu-id="9a171-134">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9a171-135">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a171-135">AzureRM.Network</span></span>
* <span data-ttu-id="9a171-136">Apresentação de novos SKUs para VirtualNetworkGateways com redundância de zona</span><span class="sxs-lookup"><span data-stu-id="9a171-136">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="9a171-137">Adição de novos comandos para a funcionalidade: APIs de Parceiro do ExpressRoute via ARM</span><span class="sxs-lookup"><span data-stu-id="9a171-137">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="9a171-138">Adição de Get-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="9a171-138">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9a171-139">Adição de Set-AzureRmExpressRouteCrossConnection</span><span class="sxs-lookup"><span data-stu-id="9a171-139">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9a171-140">Adição de Add-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9a171-140">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9a171-141">Adição de Get-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9a171-141">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9a171-142">Adição de Remove-AzureRmExpressRouteCrossConnectionPeering</span><span class="sxs-lookup"><span data-stu-id="9a171-142">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9a171-143">Adição de Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="9a171-143">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="9a171-144">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="9a171-144">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="9a171-145">Adição de Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="9a171-145">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9a171-146">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9a171-146">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9a171-147">Adição do cmdlet Get-AzureRmRecoveryServicesBackupStatus.</span><span class="sxs-lookup"><span data-stu-id="9a171-147">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="9a171-148">Este cmdlet vai buscar um ID da VM e verifica se a VM está protegida por algum cofre na subscrição.</span><span class="sxs-lookup"><span data-stu-id="9a171-148">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="9a171-149">Se o cofre existir, o cmdlet devolve os detalhes do cofre.</span><span class="sxs-lookup"><span data-stu-id="9a171-149">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a171-150">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a171-150">AzureRM.Resources</span></span>
* <span data-ttu-id="9a171-151">Atualização de cmdlets Get-AzureRmPolicyAssignment:</span><span class="sxs-lookup"><span data-stu-id="9a171-151">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="9a171-152">Adição de suporte para a listagem de valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a171-152">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="9a171-153">Adição de suporte para a obtenção de atribuições individuais com valores -Scope ao nível do grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a171-153">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="9a171-154">Adição de parâmetros -Effective e -All ao parâmetro de controlo</span><span class="sxs-lookup"><span data-stu-id="9a171-154">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="9a171-155">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="9a171-155">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="9a171-156">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a171-156">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9a171-157">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="9a171-157">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9a171-158">Atualização dos cmdlets Get/New/Remove/Set-AzureRmPolicySetDefinition</span><span class="sxs-lookup"><span data-stu-id="9a171-158">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="9a171-159">Adição do parâmetro -ManagementGroupName para aplicar operações a um determinado grupo de gestão</span><span class="sxs-lookup"><span data-stu-id="9a171-159">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9a171-160">Adição do parâmetro -SubscriptionId para aplicar operações a uma determinada subscrição</span><span class="sxs-lookup"><span data-stu-id="9a171-160">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9a171-161">Adição de suporte de referência de segredo do KeyVault nos parâmetros ao utilizar "TemplateParameterObject" em "New-AzureRmResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="9a171-161">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="9a171-162">Correção de problema em que o parâmetro "-EndDate" era ignorado para "New-AzureRmADAppCredential"</span><span class="sxs-lookup"><span data-stu-id="9a171-162">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="9a171-163">Correção de problema em que "Add-AzureRmADGroupMember" utilizava o URL incorreto para fazer o pedido</span><span class="sxs-lookup"><span data-stu-id="9a171-163">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="9a171-164">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9a171-164">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9a171-165">Adição de Parâmetro opcional -KeyValue ao cmdlet New-AzureRmServiceBusKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="9a171-165">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a171-166">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a171-166">AzureRM.Sql</span></span>
* <span data-ttu-id="9a171-167">Esclarecimento dos Pontos de Restauro Definidos pelo Utilizador para SQLDW na ajuda de New-AzureRmSqlDatabaseRestorePoint</span><span class="sxs-lookup"><span data-stu-id="9a171-167">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="9a171-168">Atualização da documentação do parâmetro -ComputeGeneration em vários cmdlets</span><span class="sxs-lookup"><span data-stu-id="9a171-168">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="9a171-169">6.3.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a171-169">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a171-170">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a171-170">AzureRM.Profile</span></span>
* <span data-ttu-id="9a171-171">Atualização das mensagens de erro de Enable-AzureRmContextAutoSave</span><span class="sxs-lookup"><span data-stu-id="9a171-171">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="9a171-172">Criação de contexto para cada subscrição ao executar "Connect-AzureRmAccount" sem contexto anterior</span><span class="sxs-lookup"><span data-stu-id="9a171-172">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9a171-173">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9a171-173">Azure.Storage</span></span>
* <span data-ttu-id="9a171-174">Adição de outras informações sobre o parâmetro -Permissions nos ficheiros de ajuda.</span><span class="sxs-lookup"><span data-stu-id="9a171-174">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a171-175">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a171-175">AzureRM.Compute</span></span>
* <span data-ttu-id="9a171-176">"Get-AzureRmVmDiskEncryptionStatus" corrige um problema observado em VMs sem discos de dados</span><span class="sxs-lookup"><span data-stu-id="9a171-176">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="9a171-177">Atualização da versão da biblioteca de cliente de Computação para corrigir os seguintes cmdlets</span><span class="sxs-lookup"><span data-stu-id="9a171-177">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="9a171-178">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9a171-178">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9a171-179">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9a171-179">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9a171-180">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="9a171-180">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="9a171-181">Correção dos seguintes cmdlets para mostrar o "ID da operação" e o "estado da operação" corretamente:</span><span class="sxs-lookup"><span data-stu-id="9a171-181">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="9a171-182">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a171-182">Start-AzureRmVM</span></span>
    - <span data-ttu-id="9a171-183">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a171-183">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="9a171-184">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a171-184">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="9a171-185">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9a171-185">Set-AzureRmVM</span></span>
    - <span data-ttu-id="9a171-186">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="9a171-186">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="9a171-187">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a171-187">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="9a171-188">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="9a171-188">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="9a171-189">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="9a171-189">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="9a171-190">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a171-190">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="9a171-191">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a171-191">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="9a171-192">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a171-192">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="9a171-193">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9a171-193">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="9a171-194">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="9a171-194">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="9a171-195">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9a171-195">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9a171-196">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="9a171-196">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="9a171-197">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9a171-197">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9a171-198">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="9a171-198">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="9a171-199">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="9a171-199">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="9a171-200">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="9a171-200">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="9a171-201">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="9a171-201">AzureRM.EventGrid</span></span>
* <span data-ttu-id="9a171-202">Remoção das condições de validação ValidateNotNullOrEmpty para SubjectBeginsWith/SubjectEndsWith no cmdlet Update-AzureRmEventGridSubscription para permitir a alteração destes parâmetros para uma cadeia vazia, se necessário.</span><span class="sxs-lookup"><span data-stu-id="9a171-202">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9a171-203">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a171-203">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a171-204">Correção de problema em que não são devolvidas Etiquetas quando Get-AzureRmKeyVault -Tag é executado</span><span class="sxs-lookup"><span data-stu-id="9a171-204">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="9a171-205">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="9a171-205">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="9a171-206">Disponibilização pública de cmdlets de Informações de Política</span><span class="sxs-lookup"><span data-stu-id="9a171-206">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="9a171-207">Utilização da versão da API 2018-04-04</span><span class="sxs-lookup"><span data-stu-id="9a171-207">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="9a171-208">Adição de PolicyDefinitionReferenceId aos resultados de Get-AzureRmPolicyStateSummary</span><span class="sxs-lookup"><span data-stu-id="9a171-208">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9a171-209">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9a171-209">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9a171-210">Adição do parâmetro -Vault a cmdlets RecoveryServices.Backup.</span><span class="sxs-lookup"><span data-stu-id="9a171-210">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="9a171-211">Ao ser transmitido, substitui o cmdlet Set-AzureRmRecoveryServicesContext.</span><span class="sxs-lookup"><span data-stu-id="9a171-211">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a171-212">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a171-212">AzureRM.Sql</span></span>
* <span data-ttu-id="9a171-213">Atualização de exemplo no ficheiro de ajuda para Get-AzureRmSqlDatabaseExpanded</span><span class="sxs-lookup"><span data-stu-id="9a171-213">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9a171-214">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9a171-214">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9a171-215">Atualização do ficheiro de ajuda para Add-AzureRmTrafficManagerEndpointConfig</span><span class="sxs-lookup"><span data-stu-id="9a171-215">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a171-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a171-216">AzureRM.Websites</span></span>
* <span data-ttu-id="9a171-217">Atualização de "Set-AzureRmWebApp" de modo a não substituir AppSettings quando -AssignIdentity é utilizado</span><span class="sxs-lookup"><span data-stu-id="9a171-217">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="9a171-218">Atualização de "New-AzureRmWebAppSlot" de modo a honrar AppServicePlan como um parâmetro opcional</span><span class="sxs-lookup"><span data-stu-id="9a171-218">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="9a171-219">6.2.1 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a171-219">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="9a171-220">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9a171-220">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="9a171-221">Atualização do modelo de PSWorkspace para permitir que a Rede utilize o tipo como um parâmetro</span><span class="sxs-lookup"><span data-stu-id="9a171-221">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="9a171-222">6.2.0 - junho de 2018</span><span class="sxs-lookup"><span data-stu-id="9a171-222">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a171-223">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a171-223">AzureRM.Profile</span></span>
* <span data-ttu-id="9a171-224">Corrija o problema onde a versão 10.0.3 de Newtonsoft.Json não foi carregada na importação do módulo</span><span class="sxs-lookup"><span data-stu-id="9a171-224">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9a171-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9a171-225">AzureRM.Compute</span></span>
* <span data-ttu-id="9a171-226">Funcionalidade Atualização da VM VMSS</span><span class="sxs-lookup"><span data-stu-id="9a171-226">VMSS VM Update feature</span></span>
    - <span data-ttu-id="9a171-227">Cmdlets "Update-AzureRmVmssVM" e "New-AzureRmVMDataDisk" adicionados</span><span class="sxs-lookup"><span data-stu-id="9a171-227">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="9a171-228">Adicione o parâmetro VirtualMachineScaleSetVM ao cmdlet "Add-AzureRmVMDataDisk" para suportar a adição de um disco de dados à VM Vmss.</span><span class="sxs-lookup"><span data-stu-id="9a171-228">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9a171-229">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9a171-229">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9a171-230">O SDK de .Net do ADF foi atualizado para a versão 0.8.0-preview que contém as seguintes alterações:</span><span class="sxs-lookup"><span data-stu-id="9a171-230">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="9a171-231">Foi adicionada a operação de Configuração de fábrica do repositório</span><span class="sxs-lookup"><span data-stu-id="9a171-231">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="9a171-232">QuickBooks LinkedService atualizado para expor as propriedades consumerKey e consumerSecret</span><span class="sxs-lookup"><span data-stu-id="9a171-232">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="9a171-233">Vários tipos de modelos Atualizados de SecretBase para Object</span><span class="sxs-lookup"><span data-stu-id="9a171-233">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="9a171-234">Acionador de Eventos de Blob adicionado</span><span class="sxs-lookup"><span data-stu-id="9a171-234">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="9a171-235">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9a171-235">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9a171-236">Documentação de atualização com resultado de exemplo</span><span class="sxs-lookup"><span data-stu-id="9a171-236">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="9a171-237">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a171-237">AzureRM.Network</span></span>
* <span data-ttu-id="9a171-238">Ativar parâmetros da Análise de Tráfego em cmdlets do Observador de Rede</span><span class="sxs-lookup"><span data-stu-id="9a171-238">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9a171-239">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9a171-239">AzureRM.Resources</span></span>
* <span data-ttu-id="9a171-240">Corrija o problema com a propriedade "Propriedades" do(s) objeto(s) "PSResource" devolvidos por "Get-AzureRmResource"</span><span class="sxs-lookup"><span data-stu-id="9a171-240">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="9a171-241">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="9a171-241">AzureRM.Scheduler</span></span>
* <span data-ttu-id="9a171-242">Corrija o problema com a atualização ServiceBusQueueJob sem definir novos valores de Autenticação</span><span class="sxs-lookup"><span data-stu-id="9a171-242">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="9a171-243">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a171-243">AzureRM.Sql</span></span>
* <span data-ttu-id="9a171-244">Cmdlets seguintes atualizados com parâmetro opcional LicenseType</span><span class="sxs-lookup"><span data-stu-id="9a171-244">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="9a171-245">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a171-245">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9a171-246">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9a171-246">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9a171-247">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9a171-247">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9a171-248">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9a171-248">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9a171-249">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a171-249">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9a171-250">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9a171-250">AzureRM.Websites</span></span>
* <span data-ttu-id="9a171-251">"New-AzureRMWebApp" está atualizado para utilizar algoritmos comuns da biblioteca Estratégia.</span><span class="sxs-lookup"><span data-stu-id="9a171-251">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="9a171-252">6.1.0 - Maio de 2018</span><span class="sxs-lookup"><span data-stu-id="9a171-252">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9a171-253">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9a171-253">AzureRM.Profile</span></span>
* <span data-ttu-id="9a171-254">Correção do problema em que a execução de "Clear-AzureRmContext" mantinha um contexto vazio com o nome do contexto predefinido anterior, o que impedia o utilizador de criar um novo contexto com o nome antigo</span><span class="sxs-lookup"><span data-stu-id="9a171-254">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9a171-255">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9a171-255">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9a171-256">Permitir operações de associação/desassociação do Gateway no AS.</span><span class="sxs-lookup"><span data-stu-id="9a171-256">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9a171-257">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9a171-257">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9a171-258">Foi adicionado suporte para ApiVersions, ApiReleases e ApiRevisions</span><span class="sxs-lookup"><span data-stu-id="9a171-258">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="9a171-259">Foi adicionado suporte para o Back-end do ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9a171-259">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="9a171-260">Foi adicionado suporte para o Logger do Application Insights</span><span class="sxs-lookup"><span data-stu-id="9a171-260">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="9a171-261">Foi adicionado suporte para reconhecer o SKU "Básico" como um SKU válido do serviço Gestão de API</span><span class="sxs-lookup"><span data-stu-id="9a171-261">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="9a171-262">Foi adicionado suporte para instalar Certificados emitidos por AC privadas como Raiz ou AC</span><span class="sxs-lookup"><span data-stu-id="9a171-262">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="9a171-263">Foi adicionado suporte para aceitar Certificados SSL personalizados através do KeyVault e de vários nomes de anfitrião de proxy</span><span class="sxs-lookup"><span data-stu-id="9a171-263">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="9a171-264">Foi adicionado suporte para a identidade MSI</span><span class="sxs-lookup"><span data-stu-id="9a171-264">Added support for MSI identity</span></span>
* <span data-ttu-id="9a171-265">Foi adicionado suporte para aceitar políticas através de Url. NOTA: Os cmdlets seguintes serão preteridos numa versão futura</span><span class="sxs-lookup"><span data-stu-id="9a171-265">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="9a171-266">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="9a171-266">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="9a171-267">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a171-267">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="9a171-268">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="9a171-268">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="9a171-269">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="9a171-269">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="9a171-270">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="9a171-270">AzureRM.Batch</span></span>
* <span data-ttu-id="9a171-271">Lançamento do novo cmdlet Get-AzureBatchPoolNodeCounts</span><span class="sxs-lookup"><span data-stu-id="9a171-271">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="9a171-272">Lançamento do novo cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span><span class="sxs-lookup"><span data-stu-id="9a171-272">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="9a171-273">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9a171-273">AzureRM.Consumption</span></span>
* <span data-ttu-id="9a171-274">Adição dos novos parâmetros Expand, ResourceGroup, InstanceName, InstanceId, Tags e Top no Cmdlet Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="9a171-274">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9a171-275">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9a171-275">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9a171-276">Correção do exemplo de Export-AzureRmDataLakeStoreChildItemProperties</span><span class="sxs-lookup"><span data-stu-id="9a171-276">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9a171-277">Correção da exceção do parâmetro nulo do caso Recursivo em Set-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a171-277">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="9a171-278">Correção dos ficheiros de ajuda de Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9a171-278">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="9a171-279">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9a171-279">AzureRM.Network</span></span>
* <span data-ttu-id="9a171-280">Aumento da versão do SDK de Rede de 18.0.0-preview para 19.0.0-preview</span><span class="sxs-lookup"><span data-stu-id="9a171-280">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="9a171-281">Foi adicionado um cmdlet para criar a configuração de protocolo</span><span class="sxs-lookup"><span data-stu-id="9a171-281">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="9a171-282">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="9a171-282">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="9a171-283">Foi adicionado um cmdlet para adicionar uma nova ligação de circuito a um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9a171-283">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="9a171-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9a171-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9a171-285">Foi adicionado um cmdlet para remover uma ligação de circuito de um circuito existente do ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="9a171-285">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="9a171-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9a171-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9a171-287">Foi adicionado um cmdlet para obter uma ligação de circuito</span><span class="sxs-lookup"><span data-stu-id="9a171-287">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="9a171-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9a171-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9a171-289">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9a171-289">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9a171-290">Correção da utilização da autenticação de servidor com certificados gerados (Problema #5998)</span><span class="sxs-lookup"><span data-stu-id="9a171-290">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9a171-291">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9a171-291">AzureRM.Sql</span></span>
* <span data-ttu-id="9a171-292">Atualização dos cmdlets de Auditoria para permitir a remoção de AuditActions ou AuditActionGroups</span><span class="sxs-lookup"><span data-stu-id="9a171-292">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="9a171-293">Correção do problema de Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy ao definir uma nova política de retenção flexível em que o comando falhava com "Configurar a política de retenção de longo-prazo com o cofre e a política do serviço de recuperação do Azure já não é suportado.</span><span class="sxs-lookup"><span data-stu-id="9a171-293">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="9a171-294">Submeta um pedido com a nova política de retenção flexível".</span><span class="sxs-lookup"><span data-stu-id="9a171-294">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="9a171-295">Atualize todos os cmdlets relacionados com as Bases de Dados SQL do Azure/Criação de Conjuntos Elásticos/Atualização para utilizar a nova API de Base de Dados, que suporta a propriedade SKU para propriedades relacionadas com dimensionamento e escalão.</span><span class="sxs-lookup"><span data-stu-id="9a171-295">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="9a171-296">Os cmdlets atualizados, incluindo:</span><span class="sxs-lookup"><span data-stu-id="9a171-296">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="9a171-297">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a171-297">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9a171-298">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9a171-298">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9a171-299">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9a171-299">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9a171-300">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9a171-300">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9a171-301">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9a171-301">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9a171-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9a171-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9a171-303">Atualize os parâmetros de "Get-AzureRmTrafficManagerProfile" para que o parâmetro -ResourceGroupName seja necessário ao utilizar o parâmetro -Name.</span><span class="sxs-lookup"><span data-stu-id="9a171-303">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>