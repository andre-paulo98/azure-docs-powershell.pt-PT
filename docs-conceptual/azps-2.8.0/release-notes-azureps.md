---
title: Notas de versão do Azure PowerShell
description: Saiba mais sobre todas as atualizações mais recentes para os módulos do Azure PowerShell.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: 83e6039153bcc2b8ccb7ceddfa91609f0d6c7b3f
ms.sourcegitcommit: b4ee3fbaaa2a329ea28308bd1902ae83a34db698
ms.translationtype: HT
ms.contentlocale: pt-PT
ms.lasthandoff: 10/16/2019
ms.locfileid: "72380189"
---
## <a name="280---october-2019"></a><span data-ttu-id="ec939-103">2.8.0 - Outubro de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-103">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="ec939-104">Geral</span><span class="sxs-lookup"><span data-stu-id="ec939-104">General</span></span>
* <span data-ttu-id="ec939-105">Versão Az.HealthcareApis 1.0.0</span><span class="sxs-lookup"><span data-stu-id="ec939-105">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ec939-106">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-106">Az.Accounts</span></span>
* <span data-ttu-id="ec939-107">Atualização da telemetria e reescrita de URL para módulos gerados; correção de testes de unidades do Windows.</span><span class="sxs-lookup"><span data-stu-id="ec939-107">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ec939-108">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-108">Az.ApiManagement</span></span>
* <span data-ttu-id="ec939-109">**Set-AzApiManagementApi** - Suporte adicionado para Atualizar a API para ApiVersionSet</span><span class="sxs-lookup"><span data-stu-id="ec939-109">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="ec939-110">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="ec939-110">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-111">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-111">Az.Automation</span></span>
* <span data-ttu-id="ec939-112">Cmdlet New-AzureAutomationSoftwareUpdateConfiguration corrigido para o parâmetro de definição de reinício do Linux.</span><span class="sxs-lookup"><span data-stu-id="ec939-112">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="ec939-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ec939-113">Az.Batch</span></span>
* <span data-ttu-id="ec939-114">**Get-AzBatchNodeAgentSku** foi preterido e será substituído por **Get-AzBatchSupportImage** na versão 2.0.0.</span><span class="sxs-lookup"><span data-stu-id="ec939-114">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-115">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-115">Az.Compute</span></span>
* <span data-ttu-id="ec939-116">Adição dos parâmetros Priority, EvictionPolicy e MaxPrice aos cmdlets New-AzVM e New-AzVmss</span><span class="sxs-lookup"><span data-stu-id="ec939-116">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="ec939-117">Correção da mensagem de aviso e do documento de ajuda para os cmdlets Add-AzVMAdditionalUnattendContent e Add-AzVMSshPublicKey</span><span class="sxs-lookup"><span data-stu-id="ec939-117">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="ec939-118">Correção da exceção -skipVmBackup para VMs do Linux com discos geridos para Set-AzVMDiskEncryptionExtension.</span><span class="sxs-lookup"><span data-stu-id="ec939-118">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="ec939-119">Correção de erro na atualização de definições de encriptação em Set-AzVMDiskEncryptionExtension, cenário de dois passos.</span><span class="sxs-lookup"><span data-stu-id="ec939-119">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-120">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-120">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-121">Adição de comandos CRUD para o fluxo de dados do ADF V2: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow e Get-AzDataFactoryV2DataFlow.</span><span class="sxs-lookup"><span data-stu-id="ec939-121">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="ec939-122">Adição de comandos de ação para a Sessão de depuração de fluxo de dados do ADF V2: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand e Stop-AzDataFactoryV2DataFlowDebugSession.</span><span class="sxs-lookup"><span data-stu-id="ec939-122">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="ec939-123">Atualização da versão do SDK .Net do ADF para 4.2.0</span><span class="sxs-lookup"><span data-stu-id="ec939-123">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-124">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-124">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-125">Correção da validação de contas, para que as contas com "-" possam ser transmitidas sem domínio</span><span class="sxs-lookup"><span data-stu-id="ec939-125">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="ec939-126">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="ec939-126">Az.HealthcareApis</span></span>
* <span data-ttu-id="ec939-127">Atualização da versão do PowerShell para 1.0.0</span><span class="sxs-lookup"><span data-stu-id="ec939-127">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="ec939-128">Atualização da versão do SDK para 1.0.2</span><span class="sxs-lookup"><span data-stu-id="ec939-128">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="ec939-129">Atualização em testes para mencionarem a nova versão do SDK</span><span class="sxs-lookup"><span data-stu-id="ec939-129">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="ec939-130">Atualização da estrutura de saída de aninhada para bidimensional.</span><span class="sxs-lookup"><span data-stu-id="ec939-130">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ec939-131">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ec939-131">Az.IotHub</span></span>
* <span data-ttu-id="ec939-132">Adição de nova origem de encaminhamento: DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="ec939-132">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="ec939-133">Correção de pequeno erro: Get-AzIothub não devolvia subscriptionId</span><span class="sxs-lookup"><span data-stu-id="ec939-133">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="ec939-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-134">Az.Monitor</span></span>
* <span data-ttu-id="ec939-135">Novos recetores de grupo de ações adicionados para o grupo de ações   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="ec939-135">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="ec939-136">Utilização do esquema de alerta comum ativada para os recetores.</span><span class="sxs-lookup"><span data-stu-id="ec939-136">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="ec939-137">Não é aplicável aos recetores de SMS, emissão de Aplicação do Azure, ITSM e Voz</span><span class="sxs-lookup"><span data-stu-id="ec939-137">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="ec939-138">Os Webhooks suportam agora a autenticação do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ec939-138">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-139">Az.Network</span></span>
* <span data-ttu-id="ec939-140">Adição do novo cmdlet Get-AzAvailableServiceAlias, que pode ser chamado para obter os aliases que podem ser utilizados para Políticas de Ponto Final de Serviço.</span><span class="sxs-lookup"><span data-stu-id="ec939-140">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="ec939-141">Foi adicionado suporte para os seletores de adição de tráfego às Ligações de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="ec939-141">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="ec939-142">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="ec939-142">New cmdlets added:</span></span>
        - <span data-ttu-id="ec939-143">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-143">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="ec939-144">Cmdlets atualizados com o parâmetro opcional -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-144">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ec939-145">Adição de suporte para os protocolos ESP e AH nas configurações de regras de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="ec939-145">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="ec939-146">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="ec939-146">Updated cmdlets:</span></span>
        - <span data-ttu-id="ec939-147">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-147">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ec939-148">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-148">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ec939-149">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-149">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="ec939-150">Melhoria do processamento de exceções em cmdlets Cortex</span><span class="sxs-lookup"><span data-stu-id="ec939-150">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="ec939-151">Novas Gerações e SKUs para VirtualNetworkGateways</span><span class="sxs-lookup"><span data-stu-id="ec939-151">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="ec939-152">Introdução de novas Gerações para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="ec939-152">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="ec939-153">Introdução de novas SKUs de débito elevado para VirtualNetworkGateways.</span><span class="sxs-lookup"><span data-stu-id="ec939-153">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ec939-154">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ec939-154">Az.RedisCache</span></span>
* <span data-ttu-id="ec939-155">Atualização da documentação de referência "Set-AzRedisCache" para incluir valores em falta para o parâmetro "-Size"</span><span class="sxs-lookup"><span data-stu-id="ec939-155">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-156">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-156">Az.Sql</span></span>
* <span data-ttu-id="ec939-157">Adição de suporte para a definição do Administrador do Active Directory na Instância Gerida</span><span class="sxs-lookup"><span data-stu-id="ec939-157">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-158">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-158">Az.Storage</span></span>
* <span data-ttu-id="ec939-159">Atualização da Biblioteca de Clientes de Armazenamento para a versão 11.1.0</span><span class="sxs-lookup"><span data-stu-id="ec939-159">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="ec939-160">A listagem de contentores com a API de plano de gestão será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="ec939-160">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="ec939-161">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="ec939-161">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="ec939-162">A listagem de contas de armazenamento da subscrição será feita com NextPageLink</span><span class="sxs-lookup"><span data-stu-id="ec939-162">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="ec939-163">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-163">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ec939-164">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ec939-164">Az.StorageSync</span></span>
* <span data-ttu-id="ec939-165">Correção do Problema 9810 em Reset-AzStorageSyncServerCertificate.</span><span class="sxs-lookup"><span data-stu-id="ec939-165">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-166">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-166">Az.Websites</span></span>
* <span data-ttu-id="ec939-167">Set-AzWebApp ao atualizar o ASP de uma aplicação estava a falhar</span><span class="sxs-lookup"><span data-stu-id="ec939-167">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="ec939-168">2.7.0 - Setembro de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-168">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="ec939-169">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-169">Az.ApiManagement</span></span>
* <span data-ttu-id="ec939-170">Atualização da descrição do parâmetro "-Format" na documentação de referência "Set-AzApiManagementPolicy"</span><span class="sxs-lookup"><span data-stu-id="ec939-170">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="ec939-171">Remoção de referências do cmdlet preterido "Update-AzApiManagementDeployment" da documentação de referência.</span><span class="sxs-lookup"><span data-stu-id="ec939-171">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="ec939-172">Em alternativa, foi utilizado "Set-AzApiManagement".</span><span class="sxs-lookup"><span data-stu-id="ec939-172">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-173">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-173">Az.Automation</span></span>
* <span data-ttu-id="ec939-174">Correção de erro de digitação no exemplo na documentação de referência para "Register-AzAutomationDscNode"</span><span class="sxs-lookup"><span data-stu-id="ec939-174">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="ec939-175">Adição de esclarecimento sobre a restrição do sistema operativo a Register-AzAutomationDSCNode</span><span class="sxs-lookup"><span data-stu-id="ec939-175">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="ec939-176">Correção da exceção de referência Nula do cmdlet Start-AzAutomationRunbook para a opção -Wait.</span><span class="sxs-lookup"><span data-stu-id="ec939-176">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-177">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-177">Az.Compute</span></span>
* <span data-ttu-id="ec939-178">Adição do parâmetro UploadSizeInBytes a New-AzDiskConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-178">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="ec939-179">Adição do parâmetro Incremental a New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-179">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="ec939-180">Adição de uma funcionalidade de máquina virtual de baixa prioridade:</span><span class="sxs-lookup"><span data-stu-id="ec939-180">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="ec939-181">Os parâmetros MaxPrice, EvictionPolicy e Priority foram adicionados a New-AzVMConfig.</span><span class="sxs-lookup"><span data-stu-id="ec939-181">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="ec939-182">O parâmetro MaxPrice foi adicionado aos cmdlets New-AzVmssConfig, Update-AzVM e Update-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="ec939-182">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="ec939-183">Correção do problema de referência de VM para o cmdlet Get-AzAvailabilitySet quando lista todos os conjuntos de disponibilidade na subscrição.</span><span class="sxs-lookup"><span data-stu-id="ec939-183">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="ec939-184">Correção da exceção numa para Get-AzRemoteDesktopFile.</span><span class="sxs-lookup"><span data-stu-id="ec939-184">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="ec939-185">Correção do método VHD Seek para a posição end-relative.</span><span class="sxs-lookup"><span data-stu-id="ec939-185">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="ec939-186">Correção do problema de UltraSSD para New-AzVM e Update-AzVM.</span><span class="sxs-lookup"><span data-stu-id="ec939-186">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-187">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-187">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-188">Adição de 3 novos comandos para o ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription e Get-AzDataFactoryV2TriggerSubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="ec939-188">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="ec939-189">Atualização da versão do SDK .Net do ADF para 4.1.3</span><span class="sxs-lookup"><span data-stu-id="ec939-189">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="ec939-190">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec939-190">Az.HDInsight</span></span>
* <span data-ttu-id="ec939-191">Chamada de alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="ec939-191">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ec939-192">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ec939-192">Az.IotHub</span></span>
* <span data-ttu-id="ec939-193">Adição de suporte para invocar a ativação pós-falha de um IotHub para a região de recuperação após desastre geograficamente emparelhada.</span><span class="sxs-lookup"><span data-stu-id="ec939-193">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="ec939-194">Adição de suporte para gerir o melhoramento de mensagens para um IotHub.</span><span class="sxs-lookup"><span data-stu-id="ec939-194">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="ec939-195">Os novos cmdlets são:</span><span class="sxs-lookup"><span data-stu-id="ec939-195">New cmdlets are:</span></span>
    - <span data-ttu-id="ec939-196">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ec939-196">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ec939-197">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ec939-197">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ec939-198">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ec939-198">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="ec939-199">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="ec939-199">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ec939-200">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-200">Az.Monitor</span></span>
* <span data-ttu-id="ec939-201">Indicação do Monitor SDK mais recente, ou seja, 0.24.1-preview</span><span class="sxs-lookup"><span data-stu-id="ec939-201">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="ec939-202">Adição de alterações sem quebra aos cmdlets de Métricas, ou seja, a enumeração de unidades suporta vários valores novos.</span><span class="sxs-lookup"><span data-stu-id="ec939-202">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="ec939-203">Estes cmdlets são só de leitura, pelo que não haverá qualquer alteração na introdução dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="ec939-203">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="ec939-204">A versão da API dos pedidos de **ActionGroups** é agora **2019-06-01**. Anteriormente, era **2018-03-01**.</span><span class="sxs-lookup"><span data-stu-id="ec939-204">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="ec939-205">Os testes de cenário foram atualizados para acomodar esta alteração.</span><span class="sxs-lookup"><span data-stu-id="ec939-205">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="ec939-206">Os construtores para as classes **EmailReceiver** e **WebhookReceiver** adicionaram um novo argumento obrigatório, ou seja, um valor booleano chamado **useCommonAlertSchema**.</span><span class="sxs-lookup"><span data-stu-id="ec939-206">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="ec939-207">Atualmente, o valor foi corrigido para **false** para ocultar esta alteração interruptiva dos cmdlets.</span><span class="sxs-lookup"><span data-stu-id="ec939-207">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="ec939-208">**NOTA**: esta é uma alteração temporária que tem de ser validada pela equipa de Alertas.</span><span class="sxs-lookup"><span data-stu-id="ec939-208">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="ec939-209">A ordem dos argumentos para o construtor da classe **Source** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="ec939-209">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="ec939-210">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="ec939-210">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="ec939-211">A ordem dos argumentos para o construtor da classe **AlertingAction** (relacionada com a classe **ScheduledQueryRuleSource**) foi alterada em relação ao SDK anterior.</span><span class="sxs-lookup"><span data-stu-id="ec939-211">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="ec939-212">Esta alteração exigia a correção de dois testes de unidade: foram compilados, mas não passaram nos testes.</span><span class="sxs-lookup"><span data-stu-id="ec939-212">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="ec939-213">Suporte de critérios de Limiar Dinâmico para o alerta de métrica V2</span><span class="sxs-lookup"><span data-stu-id="ec939-213">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="ec939-214">New-AzMetricAlertRuleV2Criteria: agora também cria critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="ec939-214">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="ec939-215">Add-AzMetricAlertRuleV2: agora também aceita critérios de limiar dinâmico</span><span class="sxs-lookup"><span data-stu-id="ec939-215">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="ec939-216">Melhorias nos cmdlets de Regra de Consulta Agendada (SQR)</span><span class="sxs-lookup"><span data-stu-id="ec939-216">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="ec939-217">Os cmdlets aceitarão o parâmetro "Location" em ambos os formatos, ou seja, a localização (por exemplo, eastus) ou o nome a apresentar da localização (por exemplo, E.U.A. Leste)</span><span class="sxs-lookup"><span data-stu-id="ec939-217">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="ec939-218">O parâmetro “Enabled” foi ilustrado corretamente nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="ec939-218">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="ec939-219">Foram adicionados exemplos para o parâmetro opcional "ActionGroup"</span><span class="sxs-lookup"><span data-stu-id="ec939-219">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="ec939-220">Melhoria geral dos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="ec939-220">Overall improved help files</span></span>
* <span data-ttu-id="ec939-221">Correção de erro na determinação do tipo de âmbito para "Set-AzActionRule"</span><span class="sxs-lookup"><span data-stu-id="ec939-221">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-222">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-222">Az.Network</span></span>
* <span data-ttu-id="ec939-223">Correção de um exemplo incorreto na documentação de referência de "New-AzApplicationGateway"</span><span class="sxs-lookup"><span data-stu-id="ec939-223">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="ec939-224">Adição de nota da documentação de referência de "Get-AzNetworkWatcherPacketCapture" sobre a obtenção de todas as propriedades para uma captura de pacote</span><span class="sxs-lookup"><span data-stu-id="ec939-224">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="ec939-225">Exemplo corrigido na documentação de referência de "Test-AzNetworkWatcherIPFlow" para enumerar corretamente as NICs</span><span class="sxs-lookup"><span data-stu-id="ec939-225">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="ec939-226">Melhoria da análise de exceção de cloud para apresentar detalhes adicionais, caso estejam presentes</span><span class="sxs-lookup"><span data-stu-id="ec939-226">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="ec939-227">Melhoria da análise de exceção de cloud para processar um tipo adicional do SDK</span><span class="sxs-lookup"><span data-stu-id="ec939-227">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="ec939-228">Correção do mapeamento incorreto de modelos de Regra de Segurança</span><span class="sxs-lookup"><span data-stu-id="ec939-228">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="ec939-229">Adição de propriedades à interface de rede para a funcionalidade de IP privado</span><span class="sxs-lookup"><span data-stu-id="ec939-229">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="ec939-230">Adição da propriedade "PrivateEndpoint" como tipo de PSResourceId a PSNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="ec939-230">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="ec939-231">Adição da propriedade "PrivateLinkConnectionProperties" como tipo de PSIpConfigurationConnectivityInformation a PSNetworkInterfaceIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-231">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="ec939-232">Adição da nova classe de modelo PSIpConfigurationConnectivityInformation</span><span class="sxs-lookup"><span data-stu-id="ec939-232">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="ec939-233">Adição do novo ApplicationRuleProtocolType "mssql" para o recurso Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="ec939-233">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="ec939-234">Suporte de Multiligação na WAN Virtual</span><span class="sxs-lookup"><span data-stu-id="ec939-234">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="ec939-235">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-235">New cmdlets</span></span>
        - <span data-ttu-id="ec939-236">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="ec939-236">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="ec939-237">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-237">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="ec939-238">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="ec939-238">Updated cmdlet:</span></span>
        - <span data-ttu-id="ec939-239">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="ec939-239">New-VpnSite</span></span>
        - <span data-ttu-id="ec939-240">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="ec939-240">Update-VpnSite</span></span>
        - <span data-ttu-id="ec939-241">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-241">New-VpnConnection</span></span>
        - <span data-ttu-id="ec939-242">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-242">Update-VpnConnection</span></span>
* <span data-ttu-id="ec939-243">Correção de documentos para alguns exemplos do PowerShell para utilizar cmdlets Az em vez de cmdlets AzureRM</span><span class="sxs-lookup"><span data-stu-id="ec939-243">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-244">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-244">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-245">Atualização do Objeto AzureVMpolicy com o Atributo ProtectedItemsCount</span><span class="sxs-lookup"><span data-stu-id="ec939-245">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="ec939-246">Adição de Testes para a política de VM e Restauro de Conta de Armazenamento Original</span><span class="sxs-lookup"><span data-stu-id="ec939-246">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-247">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-247">Az.Resources</span></span>
* <span data-ttu-id="ec939-248">Correção de erro em que não era possível chamar New-AzRoleAssignment sem o parâmetro Scope.</span><span class="sxs-lookup"><span data-stu-id="ec939-248">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ec939-249">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-249">Az.ServiceFabric</span></span>
* <span data-ttu-id="ec939-250">Correção de erro de digitação no exemplo para a documentação de referência "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="ec939-250">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="ec939-251">Adição de novos cmdlets para a gestão de aplicações e serviços:</span><span class="sxs-lookup"><span data-stu-id="ec939-251">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="ec939-252">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ec939-252">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ec939-253">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ec939-253">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ec939-254">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ec939-254">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ec939-255">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="ec939-255">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="ec939-256">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ec939-256">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ec939-257">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ec939-257">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ec939-258">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ec939-258">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ec939-259">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ec939-259">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ec939-260">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="ec939-260">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="ec939-261">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="ec939-261">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="ec939-262">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="ec939-262">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="ec939-263">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="ec939-263">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="ec939-264">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="ec939-264">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="ec939-265">Atualização do Service Fabric SDK para a versão 1.2.0, que utiliza a versão de API do fornecedor de serviços do Service Fabric 2019-03-01.</span><span class="sxs-lookup"><span data-stu-id="ec939-265">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ec939-266">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ec939-266">Az.SignalR</span></span>
* <span data-ttu-id="ec939-267">Adição dos Cmdlets Update, Restart, CheckNameAvailability, GetUsage</span><span class="sxs-lookup"><span data-stu-id="ec939-267">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-268">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-268">Az.Sql</span></span>
* <span data-ttu-id="ec939-269">Atualização do exemplo na documentação de referência para "Get-AzSqlElasticPool"</span><span class="sxs-lookup"><span data-stu-id="ec939-269">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="ec939-270">Adição de exemplo de vCore para a criação de um conjunto elástico (New-AzSqlElasticPool).</span><span class="sxs-lookup"><span data-stu-id="ec939-270">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="ec939-271">Remoção da validação de EmailAddresses e da verificação de que EmailAdmins não é falso no caso de EmailAddresses estar vazio em Set-AzSqlServerAdvancedThreatProtectionPolicy e Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-271">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="ec939-272">Ativação da remoção das definições de auditoria de servidor/base de dados quando existem várias definições de diagnóstico que ativam a categoria de auditoria.</span><span class="sxs-lookup"><span data-stu-id="ec939-272">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="ec939-273">Correção da validação de endereço de e-mail em vários cmdlets de Avaliação de Vulnerabilidades de SQL (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting e Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span><span class="sxs-lookup"><span data-stu-id="ec939-273">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-274">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-274">Az.Storage</span></span>
* <span data-ttu-id="ec939-275">Atualização do exemplo na documentação de referência para "Get-AzStorageAccountKey"</span><span class="sxs-lookup"><span data-stu-id="ec939-275">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="ec939-276">Na opção Carregar/Descarregar Ficheiro do Azure, o suporte preserva as propriedades SMB de Ficheiro (Atributos de Ficheiro, Hora de Criação do Ficheiro, Hora da Última Escrita no Ficheiro) no ficheiro de destino</span><span class="sxs-lookup"><span data-stu-id="ec939-276">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="ec939-277">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ec939-277">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="ec939-278">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ec939-278">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="ec939-279">Correção da falha de carregamento de blob de blocos com propriedades/metadados em ImmutabilityPolicy ativada em contentores.</span><span class="sxs-lookup"><span data-stu-id="ec939-279">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="ec939-280">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ec939-280">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="ec939-281">Suporte da gestão de partilhas de Ficheiros do Azure com a API do Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="ec939-281">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="ec939-282">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ec939-282">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ec939-283">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ec939-283">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ec939-284">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ec939-284">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="ec939-285">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="ec939-285">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-286">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-286">Az.Websites</span></span>
* <span data-ttu-id="ec939-287">Correção do problema em que as Etiquetas webapp eram eliminadas ao migrar a Aplicação para o novo ASP</span><span class="sxs-lookup"><span data-stu-id="ec939-287">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="ec939-288">Correção de Publish-AzureWebapp para funcionar no Linux e no Windows</span><span class="sxs-lookup"><span data-stu-id="ec939-288">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="ec939-289">Atualização do exemplo na documentação de referência de "Get-AzWebAppPublishingProfile"</span><span class="sxs-lookup"><span data-stu-id="ec939-289">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="ec939-290">2.6.0 - Agosto de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-290">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="ec939-291">Geral</span><span class="sxs-lookup"><span data-stu-id="ec939-291">General</span></span>
* <span data-ttu-id="ec939-292">Correção de diversos erros de digitação em vários módulos</span><span class="sxs-lookup"><span data-stu-id="ec939-292">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ec939-293">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-293">Az.Accounts</span></span>
* <span data-ttu-id="ec939-294">Suporte de MSI atribuído pelo utilizador na Autenticação de Funções do Azure (#9479)</span><span class="sxs-lookup"><span data-stu-id="ec939-294">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="ec939-295">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="ec939-295">Az.Aks</span></span>
* <span data-ttu-id="ec939-296">Correção do problema com a saída "Get-AzAks"</span><span class="sxs-lookup"><span data-stu-id="ec939-296">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="ec939-297">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="ec939-297">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ec939-298">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-298">Az.ApiManagement</span></span>
* <span data-ttu-id="ec939-299">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="ec939-299">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="ec939-300">Atualização da versão nuget .net, que não impõe restrições a productId, apiId, groupId e userId</span><span class="sxs-lookup"><span data-stu-id="ec939-300">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="ec939-301">**Get-AzApiManagementProduct** - Suporte adicionado para consultar produtos com a API.</span><span class="sxs-lookup"><span data-stu-id="ec939-301">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="ec939-302">**New-AzApiManagementApiRevision** - Correção do problema em que ApiRevisionDescription não estava a ser definido ao criar uma nova revisão da API https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="ec939-302">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="ec939-303">Correção do erro de digitação no modelo "PsApiManagementOAuth2AuthrozationServer" para "PsApiManagementOAuth2AuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="ec939-303">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="ec939-304">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ec939-304">Az.Batch</span></span>
* <span data-ttu-id="ec939-305">Correção de erro de digitação na mensagem de ajuda e na documentação para capitalizar Windows</span><span class="sxs-lookup"><span data-stu-id="ec939-305">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ec939-306">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ec939-306">Az.Cdn</span></span>
* <span data-ttu-id="ec939-307">Correção de um erro de digitação no programa auxiliar de conversão do módulo CDN</span><span class="sxs-lookup"><span data-stu-id="ec939-307">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-308">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-308">Az.Compute</span></span>
* <span data-ttu-id="ec939-309">VmssId adicionado ao cmdlet New-AzVMConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-309">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="ec939-310">Parâmetros TerminateScheduledEvents e TerminateScheduledEventNotBeforeTimeoutInMinutes adicionados a New-AzVmssConfig e Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="ec939-310">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="ec939-311">Propriedade HyperVGeneration adicionada ao objeto de imagem da VM</span><span class="sxs-lookup"><span data-stu-id="ec939-311">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="ec939-312">Funcionalidades Host e HostGroup adicionadas</span><span class="sxs-lookup"><span data-stu-id="ec939-312">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="ec939-313">Novos cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="ec939-313">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="ec939-314">O parâmetro HostId foi adicionado a New-AzVMConfig e New-AzVM</span><span class="sxs-lookup"><span data-stu-id="ec939-314">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="ec939-315">Exemplo atualizado na documentação "Invoke-AzVMRunCommand" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="ec939-315">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="ec939-316">Descrição '-VolumeType' atualizada na documentação de referência "Set-AzVMDiskEncryptionExtension" e "Set-AzVmssDiskEncryptionExtension"</span><span class="sxs-lookup"><span data-stu-id="ec939-316">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-317">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-317">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-318">Erro de digitação corrigido para capitalizar "Windows" na documentação "New-AzDataFactoryEncryptValue"</span><span class="sxs-lookup"><span data-stu-id="ec939-318">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="ec939-319">Atualização da versão do SDK .Net do ADF para 4.1.2</span><span class="sxs-lookup"><span data-stu-id="ec939-319">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="ec939-320">Parâmetros "DataProxyIntegrationRuntimeName", "DataProxyStagingLinkedServiceName" e "DataProxyStagingPath" adicionados para o cmd "Set-AzureRmDataFactoryV2IntegrationRuntime" para permitir a configuração do Runtime de Integração Autoalojado como proxy para o Azure-SSIS Integration Runtime</span><span class="sxs-lookup"><span data-stu-id="ec939-320">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="ec939-321">PSTriggerRun atualizado para mostrar os pipelines acionados, a mensagem e as propriedades, e PSActivityRun para mostrar o tipo de atividade</span><span class="sxs-lookup"><span data-stu-id="ec939-321">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-322">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-322">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-323">Correção de Get-DataLakeStoreDeletedItem para erros ou exceções remotas.</span><span class="sxs-lookup"><span data-stu-id="ec939-323">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ec939-324">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ec939-324">Az.EventHub</span></span>
* <span data-ttu-id="ec939-325">Correção do problema n.º 9658: Erro de digitação no parâmetro VirtualNteworkRule em Set-AzEventHubNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-325">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="ec939-326">Correção do problema n.º 9558: Set-AzEventHubNamespace está a utilizar PATCH em vez de PUT</span><span class="sxs-lookup"><span data-stu-id="ec939-326">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="ec939-327">Parâmetro EnableKafka adicionado ao cmdlet Set-AzEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="ec939-327">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="ec939-328">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="ec939-328">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="ec939-329">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="ec939-329">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="ec939-330">Correção do erro de digitação na documentação em que "Azure" estava em minúsculas</span><span class="sxs-lookup"><span data-stu-id="ec939-330">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ec939-331">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-331">Az.Monitor</span></span>
* <span data-ttu-id="ec939-332">Foi corrigido nome de parâmetro incorreto na documentação de ajuda</span><span class="sxs-lookup"><span data-stu-id="ec939-332">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-333">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-333">Az.Network</span></span>
* <span data-ttu-id="ec939-334">New-AzPrivateLinkServiceIpConfig atualizado</span><span class="sxs-lookup"><span data-stu-id="ec939-334">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="ec939-335">O parâmetro "PublicIpAddress" foi preterido por nunca ser utilizado no lado do servidor.</span><span class="sxs-lookup"><span data-stu-id="ec939-335">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="ec939-336">Foi adicionado um parâmetro opcional "Primary" que indica se a configuração IP atual é ou não primária.</span><span class="sxs-lookup"><span data-stu-id="ec939-336">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="ec939-337">Processamento melhorado da exceção de erros dos pedidos do SDK – Correção do problema em que as exceções do SDK anteriores não eram processadas corretamente, o que fazia com que os principais detalhes de erro não fossem apresentados</span><span class="sxs-lookup"><span data-stu-id="ec939-337">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="ec939-338">Foi ajustada a lógica de validação do prefixo IPv6 para verificar o comprimento correto do prefixo IPv6.</span><span class="sxs-lookup"><span data-stu-id="ec939-338">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="ec939-339">Get-AzVirtualNetworkSubnetConfig atualizado: Conjunto de parâmetros adicionado para obtenção por ID de recurso da sub-rede.</span><span class="sxs-lookup"><span data-stu-id="ec939-339">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="ec939-340">Descrição atualizada do parâmetro Location para AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="ec939-340">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ec939-341">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-341">Az.OperationalInsights</span></span>
* <span data-ttu-id="ec939-342">Documentação atualizada para "New-AzOperationalInsightsLinuxSyslogDataSource"</span><span class="sxs-lookup"><span data-stu-id="ec939-342">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="ec939-343">Exemplo adicionado</span><span class="sxs-lookup"><span data-stu-id="ec939-343">Added example</span></span>
    - <span data-ttu-id="ec939-344">Descrição atualizada para o parâmetro "-Name"</span><span class="sxs-lookup"><span data-stu-id="ec939-344">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="ec939-345">Exemplo adicionado para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="ec939-345">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="ec939-346">Alteração da descrição do parâmetro -Name para New-AzOperationalInsightsWindowsEventDataSource</span><span class="sxs-lookup"><span data-stu-id="ec939-346">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-347">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-347">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-348">Atualização de "Get-AzRecoveryServicesBackupJobDetail.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-348">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-349">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-349">Az.Resources</span></span>
* <span data-ttu-id="ec939-350">Suporte adicionado para a nova versão da API de 2019-05-10 para Microsoft.Resource</span><span class="sxs-lookup"><span data-stu-id="ec939-350">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="ec939-351">Suporte adicionado para "copy.count = 0" para variáveis, recursos e propriedades</span><span class="sxs-lookup"><span data-stu-id="ec939-351">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="ec939-352">Os recursos com "condition = false" ou "copy.count = 0" serão eliminados no modo completo</span><span class="sxs-lookup"><span data-stu-id="ec939-352">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="ec939-353">Exemplo de atribuição de política adicionado ao nível de subscrição no documento de ajuda</span><span class="sxs-lookup"><span data-stu-id="ec939-353">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ec939-354">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ec939-354">Az.ServiceBus</span></span>
* <span data-ttu-id="ec939-355">Correção do problema n.º 9658: Parâmetro VirtualNetworkRule com erro de digitação em Set-AzServiceBusNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-355">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="ec939-356">Correção do problema n.º 9786: não é possível criar uma regra com direitos apenas de escuta</span><span class="sxs-lookup"><span data-stu-id="ec939-356">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="ec939-357">Novo comando "test-AzServiceBusNameAvailability" adicionado para verificar a disponibilidade do nome da fila e do tópico</span><span class="sxs-lookup"><span data-stu-id="ec939-357">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="ec939-358">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-358">Az.ServiceFabric</span></span>
* <span data-ttu-id="ec939-359">Correção de erros no cmdlet de tipo de nó:</span><span class="sxs-lookup"><span data-stu-id="ec939-359">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="ec939-360">Erro de NullReferenceException quando o grupo de recursos tinha outros vmss não relacionados com o cluster do service fabric.</span><span class="sxs-lookup"><span data-stu-id="ec939-360">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="ec939-361">Correção do problema: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="ec939-361">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="ec939-362">Correção do erro em que ocorre a falha do cmdlet quando virtualNetwork está num grupo de recursos diferente do cluster.</span><span class="sxs-lookup"><span data-stu-id="ec939-362">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="ec939-363">Correção do problema: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="ec939-363">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="ec939-364">Descontinuação do cmdlet Add-AzServiceFabricApplicationCertificate</span><span class="sxs-lookup"><span data-stu-id="ec939-364">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-365">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-365">Az.Sql</span></span>
* <span data-ttu-id="ec939-366">Documentação dos cmdlets de Auditoria antigos atualizada.</span><span class="sxs-lookup"><span data-stu-id="ec939-366">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-367">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-367">Az.Storage</span></span>
* <span data-ttu-id="ec939-368">Ajuda atualizada para Get/Close-AzStorageFileHandle, ao adicionar mais cenários aos exemplos do cmdlet e descrições de parâmetros atualizadas</span><span class="sxs-lookup"><span data-stu-id="ec939-368">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="ec939-369">Suporte de StandardBlobTier no blob de carregamento e de cópia</span><span class="sxs-lookup"><span data-stu-id="ec939-369">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="ec939-370">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ec939-370">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="ec939-371">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ec939-371">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="ec939-372">Suporte de Rehydrate Priority no blob de cópia</span><span class="sxs-lookup"><span data-stu-id="ec939-372">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="ec939-373">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ec939-373">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-374">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-374">Az.Websites</span></span>
* <span data-ttu-id="ec939-375">Esclarecimento adicionado ao parâmetro -AppSettings em Set-AzWebApp e Set-AzWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="ec939-375">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="ec939-376">2.5.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-376">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-377">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-377">Az.Accounts</span></span>
* <span data-ttu-id="ec939-378">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="ec939-378">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="ec939-379">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-379">Az.ApplicationInsights</span></span>
* <span data-ttu-id="ec939-380">Correção do erro de digitação na documentação de "Remove-AzApplicationInsightsApiKey"</span><span class="sxs-lookup"><span data-stu-id="ec939-380">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="ec939-381">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-381">Az.Automation</span></span>
* <span data-ttu-id="ec939-382">Correção do erro de digitação na cadeia de recursos</span><span class="sxs-lookup"><span data-stu-id="ec939-382">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="ec939-383">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ec939-383">Az.CognitiveServices</span></span>
* <span data-ttu-id="ec939-384">Adicionado suporte de NetworkRuleSet.</span><span class="sxs-lookup"><span data-stu-id="ec939-384">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-385">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-385">Az.Compute</span></span>
* <span data-ttu-id="ec939-386">Adicionadas as propriedades em falta (ComputerName, OsName, OsVersion e HyperVGeneration) do objeto de vista da instância de VM.</span><span class="sxs-lookup"><span data-stu-id="ec939-386">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="ec939-387">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="ec939-387">Az.ContainerRegistry</span></span>
* <span data-ttu-id="ec939-388">Correção do erro de digitação em Remove-AzContainerRegistryReplication para o parâmetro de Replicação</span><span class="sxs-lookup"><span data-stu-id="ec939-388">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="ec939-389">Mais informações aqui https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="ec939-389">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-390">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-390">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-391">Atualização da versão do SDK .Net do ADF para 4.1.0</span><span class="sxs-lookup"><span data-stu-id="ec939-391">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="ec939-392">Correção do erro de digitação na documentação de "Get-AzDataFactoryV2PipelineRun"</span><span class="sxs-lookup"><span data-stu-id="ec939-392">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ec939-393">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ec939-393">Az.EventHub</span></span>
* <span data-ttu-id="ec939-394">Adicionado novo cmdlet para gerar um token de SAS: New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="ec939-394">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="ec939-395">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="ec939-395">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ec939-396">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec939-396">Az.KeyVault</span></span>
* <span data-ttu-id="ec939-397">Adicionado suporte para especificar o KeySize das Políticas de Certificado</span><span class="sxs-lookup"><span data-stu-id="ec939-397">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ec939-398">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ec939-398">Az.LogicApp</span></span>
* <span data-ttu-id="ec939-399">Correção para Get-AzIntegrationAccountMap para listar todos os tipos de mapa</span><span class="sxs-lookup"><span data-stu-id="ec939-399">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="ec939-400">Adicionado novo parâmetro MapType para filtragem</span><span class="sxs-lookup"><span data-stu-id="ec939-400">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="ec939-401">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="ec939-401">Az.ManagedServices</span></span>
* <span data-ttu-id="ec939-402">Adicionado suporte para a versão de API 2019-06-01 (GA)</span><span class="sxs-lookup"><span data-stu-id="ec939-402">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-403">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-403">Az.Network</span></span>
* <span data-ttu-id="ec939-404">Adicionado suporte para ponto final privado e serviço de ligação privada</span><span class="sxs-lookup"><span data-stu-id="ec939-404">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="ec939-405">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-405">New cmdlets</span></span>
        - <span data-ttu-id="ec939-406">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ec939-406">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ec939-407">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ec939-407">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ec939-408">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-408">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ec939-409">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-409">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ec939-410">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-410">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ec939-411">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-411">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="ec939-412">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="ec939-412">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="ec939-413">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ec939-413">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="ec939-414">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies na Sub-rede em Virtualnetwork</span><span class="sxs-lookup"><span data-stu-id="ec939-414">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="ec939-415">Atualização de New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-415">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="ec939-416">Foi adicionado o parâmetro opcional -PrivateEndpointNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no ponto final privado nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="ec939-416">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="ec939-417">Foi adicionado o parâmetro opcional -PrivateLinkServiceNetworkPoliciesFlag que configura se as políticas de rede devem ser aplicadas no serviço de ligação privada nesta sub-rede.</span><span class="sxs-lookup"><span data-stu-id="ec939-417">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="ec939-418">O nome do parâmetro de cmdlet "ServiceName" de AzPrivateLinkService foi alterado para "Name" com um alias "ServiceName" para retrocompatibilidade</span><span class="sxs-lookup"><span data-stu-id="ec939-418">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="ec939-419">Ativação do protocolo ICMP para configurações de regra de segurança de rede</span><span class="sxs-lookup"><span data-stu-id="ec939-419">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="ec939-420">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="ec939-420">Updated cmdlets</span></span>
        - <span data-ttu-id="ec939-421">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-421">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ec939-422">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-422">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="ec939-423">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-423">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="ec939-424">Adicionado ConnectionProtocolType (Ikev1/Ikev2) como parâmetro configurável de New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-424">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="ec939-425">Adicionado PrivateIpAddressVersion em LoadBalancerFrontendIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-425">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="ec939-426">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="ec939-426">Updated cmdlet:</span></span>
        - <span data-ttu-id="ec939-427">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-427">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="ec939-428">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-428">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="ec939-429">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-429">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="ec939-430">Atualização do comando New-AzApplicationGatewayProbeConfig do Gateway de Aplicação para suportar a porta personalizada na Sonda</span><span class="sxs-lookup"><span data-stu-id="ec939-430">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="ec939-431">Atualização de New-AzApplicationGatewayProbeConfig: Adicionada Porta de parâmetro opcional utilizada para sondar o servidor de back-end.</span><span class="sxs-lookup"><span data-stu-id="ec939-431">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="ec939-432">Este parâmetro é aplicável ao SKU Standard_V2 e WAF_V2.</span><span class="sxs-lookup"><span data-stu-id="ec939-432">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ec939-433">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-433">Az.OperationalInsights</span></span>
* <span data-ttu-id="ec939-434">Atualização da versão predefinida das pesquisas guardadas como 1.</span><span class="sxs-lookup"><span data-stu-id="ec939-434">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="ec939-435">Correção do processamento de regex nula de registo personalizado</span><span class="sxs-lookup"><span data-stu-id="ec939-435">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-436">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-436">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-437">Atualização de "Get-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-437">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="ec939-438">Atualização de "Get-AzRecoveryServicesBackupContainer.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-438">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="ec939-439">Atualização de "Get-AzRecoveryServicesVault.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-439">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="ec939-440">Atualização de "Wait-AzRecoveryServicesBackupJob.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-440">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="ec939-441">Atualização de "Set-AzRecoveryServicesVaultContext.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-441">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="ec939-442">Atualização de "Get-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-442">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="ec939-443">Atualização de "Get-AzRecoveryServicesBackupRecoveryPoint.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-443">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="ec939-444">Atualização de "Restore-AzRecoveryServicesBackupItem.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-444">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="ec939-445">Atualização da chamada de serviço para Anular o registo na Partilha de Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-445">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="ec939-446">Atualização de "Set-AzRecoveryServicesAsrAlertSetting.md"</span><span class="sxs-lookup"><span data-stu-id="ec939-446">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-447">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-447">Az.Resources</span></span>
- <span data-ttu-id="ec939-448">Remoção do cmdlet em falta referenciado na documentação de "New-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="ec939-448">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="ec939-449">Atualização dos cmdlets de política para utilizar a nova versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="ec939-449">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ec939-450">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ec939-450">Az.ServiceBus</span></span>
* <span data-ttu-id="ec939-451">Adicionado novo cmdlet para gerar um token de SAS: New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="ec939-451">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="ec939-452">Adicionada a verificação e mensagem de erro para os direitos de AuthorizationRules se apenas "Manage" estiver atribuído</span><span class="sxs-lookup"><span data-stu-id="ec939-452">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-453">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-453">Az.Sql</span></span>
* <span data-ttu-id="ec939-454">Correção de exemplos em falta para o cmdlet Set-AzSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="ec939-454">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="ec939-455">Correção da definição de análises recorrentes de Avaliação de Vulnerabilidades sem fornecer nenhum endereço de e-mail</span><span class="sxs-lookup"><span data-stu-id="ec939-455">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="ec939-456">Correção de um pequeno erro de digitação numa mensagem de aviso.</span><span class="sxs-lookup"><span data-stu-id="ec939-456">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-457">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-457">Az.Storage</span></span>
* <span data-ttu-id="ec939-458">Atualização do exemplo na documentação de referência de "Get-AzStorageAccount" para utilizar o nome de parâmetro correto</span><span class="sxs-lookup"><span data-stu-id="ec939-458">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ec939-459">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ec939-459">Az.StorageSync</span></span>
* <span data-ttu-id="ec939-460">A adicionar o cmdlet Invoke-AzStorageSyncChangeDetection.</span><span class="sxs-lookup"><span data-stu-id="ec939-460">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="ec939-461">Correção do Problema 9551 referente a TierFilesOlderThanDays</span><span class="sxs-lookup"><span data-stu-id="ec939-461">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-462">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-462">Az.Websites</span></span>
* <span data-ttu-id="ec939-463">Correção de um erro em que algumas propriedades SiteConfig não eram devolvidas por Get-AzWebApp e Set-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="ec939-463">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="ec939-464">Adiciona um novo parâmetro de Localização a Get-AzDeletedWebApp e Restore-AzDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="ec939-464">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="ec939-465">Corrige um erro de clonagem de blocos de aplicação Web com -IncludeSourceWebAppSlots de New-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="ec939-465">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="ec939-466">2.4.0 - Julho de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-466">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-467">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-467">Az.Accounts</span></span>
* <span data-ttu-id="ec939-468">Adicionar suporte para cmdlets de perfil</span><span class="sxs-lookup"><span data-stu-id="ec939-468">Add support for profile cmdlets</span></span>
* <span data-ttu-id="ec939-469">Adicionar suporte para ambientes e planos de dados nos cmdlets gerados</span><span class="sxs-lookup"><span data-stu-id="ec939-469">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="ec939-470">Corrigir erro quando o ponto final incorreto estava a ser utilizado em alguns casos para cmdlets do plano de dados no Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="ec939-470">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="ec939-471">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="ec939-471">Az.Advisor</span></span>
* <span data-ttu-id="ec939-472">Versão GA do Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="ec939-472">GA release of Az.Advisor</span></span>
* <span data-ttu-id="ec939-473">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="ec939-473">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="ec939-474">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-474">Az.ApiManagement</span></span>
* <span data-ttu-id="ec939-475">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="ec939-475">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="ec939-476">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="ec939-476">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="ec939-477">Foi adicionado suporte para consultar subscrições por Utilizador e Produto</span><span class="sxs-lookup"><span data-stu-id="ec939-477">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="ec939-478">Foi adicionado suporte para consultar com o Âmbito "/", "/apis", "/apis/eco-api"</span><span class="sxs-lookup"><span data-stu-id="ec939-478">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="ec939-479">Correção para o problema https://github.com/Azure/azure-powershell/issues/9307 e https://github.com/Azure/azure-powershell/issues/8432</span><span class="sxs-lookup"><span data-stu-id="ec939-479">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="ec939-480">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="ec939-480">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="ec939-481">Foi adicionado suporte para especificar "ApiVersion" e "ApiVersionSetId" ao importar Apis</span><span class="sxs-lookup"><span data-stu-id="ec939-481">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-482">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-482">Az.Automation</span></span>
* <span data-ttu-id="ec939-483">Foi corrigido o erro do cmdlet Set-AzAutomationConnectionFieldValue para lidar com o valor da cadeia (de carateres).</span><span class="sxs-lookup"><span data-stu-id="ec939-483">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-484">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-484">Az.Compute</span></span>
* <span data-ttu-id="ec939-485">Adicionar parâmetro HyperVGeneration a New-AzImageConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-485">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-486">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-486">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-487">A atualizar a saída para obter execuções de atividades, do pipeline e do acionador de cmdlets ADF para suportar o pipe Select-Object.</span><span class="sxs-lookup"><span data-stu-id="ec939-487">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ec939-488">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ec939-488">Az.EventGrid</span></span>
* <span data-ttu-id="ec939-489">Corrigir erro de digitação na documentação "New-AzEventGridSubscription"</span><span class="sxs-lookup"><span data-stu-id="ec939-489">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ec939-490">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ec939-490">Az.IotHub</span></span>
* <span data-ttu-id="ec939-491">Adicione suporte para regenerar chaves de política de autorização.</span><span class="sxs-lookup"><span data-stu-id="ec939-491">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-492">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-492">Az.Network</span></span>
* <span data-ttu-id="ec939-493">Foi adicionado "RoutingPreference" para etiquetas de IP público</span><span class="sxs-lookup"><span data-stu-id="ec939-493">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="ec939-494">Melhorar exemplos para documentação de referência "Get-AzNetworkServiceTag"</span><span class="sxs-lookup"><span data-stu-id="ec939-494">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ec939-495">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-495">Az.PolicyInsights</span></span>
* <span data-ttu-id="ec939-496">Corrigir problema de referência nula em Get-AzPolicyState</span><span class="sxs-lookup"><span data-stu-id="ec939-496">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="ec939-497">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="ec939-497">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ec939-498">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-498">Az.OperationalInsights</span></span>
* <span data-ttu-id="ec939-499">Modelo de origem de dados CustomLog corrigido devolvido em Get-AzOperationalInsightsDataSource</span><span class="sxs-lookup"><span data-stu-id="ec939-499">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-500">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-500">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-501">Corrigir para o comando get-policy para IaaSVMs</span><span class="sxs-lookup"><span data-stu-id="ec939-501">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-502">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-502">Az.Resources</span></span>
    - <span data-ttu-id="ec939-503">Corrigir texto de ajuda para o parâmetro Get-AzPolicyState- Top</span><span class="sxs-lookup"><span data-stu-id="ec939-503">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="ec939-504">Adicionar suporte de paginação do lado do cliente para Get-AzPolicyAlias</span><span class="sxs-lookup"><span data-stu-id="ec939-504">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="ec939-505">Adicionar novos parâmetros para Set-AzPolicyAssignment, -PolicyParameters e -PolicyParametersObject</span><span class="sxs-lookup"><span data-stu-id="ec939-505">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="ec939-506">Várias atualizações de documento e exemplo para cmdlets de Política</span><span class="sxs-lookup"><span data-stu-id="ec939-506">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ec939-507">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ec939-507">Az.ServiceBus</span></span>
* <span data-ttu-id="ec939-508">Correção do problema n.º 4938 - New-AzureRmServiceBusQueue devolve BadRequest ao definir MaxSizeInMegabytes</span><span class="sxs-lookup"><span data-stu-id="ec939-508">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-509">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-509">Az.Sql</span></span>
* <span data-ttu-id="ec939-510">Adicionar cmdlets de Grupo de Ativação Pós-falha de Instância da versão de pré-visualização para a versão pública</span><span class="sxs-lookup"><span data-stu-id="ec939-510">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="ec939-511">Suporta SQL Server do Azure\Auditoria de Base de Dados com cmdlets novos.</span><span class="sxs-lookup"><span data-stu-id="ec939-511">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="ec939-512">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ec939-512">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ec939-513">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ec939-513">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ec939-514">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="ec939-514">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="ec939-515">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ec939-515">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="ec939-516">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ec939-516">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="ec939-517">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="ec939-517">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="ec939-518">Remover restrições de e-mail das definições de Avaliação de Vulnerabilidades</span><span class="sxs-lookup"><span data-stu-id="ec939-518">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-519">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-519">Az.Storage</span></span>
* <span data-ttu-id="ec939-520">Alterar dois parâmetros "-IndexDocument" e "-ErrorDocument404Path" de obrigatório para opcional no cmdlet:</span><span class="sxs-lookup"><span data-stu-id="ec939-520">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="ec939-521">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ec939-521">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="ec939-522">Ajuda de atualização de Get-AzStorageBlobContent ao adicionar um exemplo</span><span class="sxs-lookup"><span data-stu-id="ec939-522">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="ec939-523">Mostrar mais informações de erro quando o cmdlet falhou com o StorageException</span><span class="sxs-lookup"><span data-stu-id="ec939-523">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="ec939-524">Suporte de criação ou atualização da conta de Armazenamento com Autenticação de DS do AAD dos Ficheiros do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-524">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="ec939-525">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-525">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="ec939-526">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-526">Set-AzStorageAccount</span></span>
* <span data-ttu-id="ec939-527">Suportar lista ou fechar identificadores de ficheiro de uma partilha de ficheiros, diretório do ficheiro ou um ficheiro</span><span class="sxs-lookup"><span data-stu-id="ec939-527">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="ec939-528">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ec939-528">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="ec939-529">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="ec939-529">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="ec939-530">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="ec939-530">Az.StorageSync</span></span>
* <span data-ttu-id="ec939-531">Este módulo está agora incluído como parte do módulo `Az` de rollup</span><span class="sxs-lookup"><span data-stu-id="ec939-531">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="ec939-532">2.3.2 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-532">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-533">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-533">Az.Accounts</span></span>
* <span data-ttu-id="ec939-534">Correção do erro de utilização do URL incorreto em alguns casos para chamadas de Funções</span><span class="sxs-lookup"><span data-stu-id="ec939-534">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="ec939-535">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="ec939-535">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="ec939-536">Correção de problema em aliases de cmdlets do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="ec939-536">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="ec939-537">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="ec939-537">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="ec939-538">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="ec939-538">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-539">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-539">Az.Compute</span></span>
* <span data-ttu-id="ec939-540">Os conjuntos de parâmetros simples New-AzVm e New-AzVmss aceitam agora o parâmetro "ProximityPlacementGroup".</span><span class="sxs-lookup"><span data-stu-id="ec939-540">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="ec939-541">Correção de erro de digitação na documentação de referência "New-AzVM"</span><span class="sxs-lookup"><span data-stu-id="ec939-541">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="ec939-542">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="ec939-542">Az.Dns</span></span>
* <span data-ttu-id="ec939-543">Foi corrigido um erro de digitação nos exemplos de ajuda "Set-AzDnsZone".</span><span class="sxs-lookup"><span data-stu-id="ec939-543">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ec939-544">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ec939-544">Az.EventGrid</span></span>
* <span data-ttu-id="ec939-545">Atualizado para utilizar a versão de API 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="ec939-545">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="ec939-546">Novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="ec939-546">New cmdlets:</span></span>
    - <span data-ttu-id="ec939-547">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ec939-547">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ec939-548">Cria um novo Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="ec939-548">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ec939-549">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ec939-549">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ec939-550">Obtém os detalhes de um Domínio do Event Grid ou obtém uma lista de todos os Domínios do Event Grid na atual subscrição do Azure.</span><span class="sxs-lookup"><span data-stu-id="ec939-550">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="ec939-551">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="ec939-551">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="ec939-552">Remove um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="ec939-552">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ec939-553">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="ec939-553">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="ec939-554">Regenera a chave de acesso partilhado para um Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="ec939-554">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="ec939-555">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="ec939-555">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="ec939-556">Obtém as chaves de acesso partilhado utilizadas para publicar eventos num Domínio do Event Grid.</span><span class="sxs-lookup"><span data-stu-id="ec939-556">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="ec939-557">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="ec939-557">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="ec939-558">Cria um novo Tópico de Domínio do Azure Event Grid.</span><span class="sxs-lookup"><span data-stu-id="ec939-558">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="ec939-559">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="ec939-559">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="ec939-560">Obtém os detalhes de um Tópico de Domínio do Event Grid ou obtém uma lista de todos os Tópicos de Domínio do Event Grid no Domínio específico do Event Grid no Azure atual</span><span class="sxs-lookup"><span data-stu-id="ec939-560">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="ec939-561">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="ec939-561">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="ec939-562">Remove um Tópico de Domínio do Azure Event Grid existente.</span><span class="sxs-lookup"><span data-stu-id="ec939-562">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="ec939-563">cmdlets atualizados:</span><span class="sxs-lookup"><span data-stu-id="ec939-563">Updated cmdlets:</span></span>
    - <span data-ttu-id="ec939-564">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="ec939-564">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="ec939-565">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o novo Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="ec939-565">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="ec939-566">Adição de novos parâmetros obrigatórios para especificar o novo nome de Domínio do Event Grid e/ou nome de Tópico de Domínio do Event Grid, para permitir a criação de uma nova subscrição de evento nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="ec939-566">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="ec939-567">Adição de novos Conjuntos de parâmetros para domínios e tópicos de domínio, para permitir a reutilização de parâmetros existentes (p. ex., EndPointType, SubjectBeginsWith, etc.).</span><span class="sxs-lookup"><span data-stu-id="ec939-567">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="ec939-568">Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="ec939-568">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="ec939-569">Data de expiração da subscrição de eventos,</span><span class="sxs-lookup"><span data-stu-id="ec939-569">Event subscription expiration date,</span></span>
            - <span data-ttu-id="ec939-570">Parâmetros de filtragem avançada.</span><span class="sxs-lookup"><span data-stu-id="ec939-570">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="ec939-571">Adição de uma nova enumeração para servicebusqueue como destino.</span><span class="sxs-lookup"><span data-stu-id="ec939-571">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="ec939-572">Deixou de ser permitida a utilização de "All" na opção -IncludedEventType e foi substituída por</span><span class="sxs-lookup"><span data-stu-id="ec939-572">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="ec939-573">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="ec939-573">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="ec939-574">Adição de novos parâmetros opcionais (Top, ODataQuery e NextLink) para suportar a paginação e filtragem de resultados.</span><span class="sxs-lookup"><span data-stu-id="ec939-574">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="ec939-575">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="ec939-575">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="ec939-576">Adição de novos parâmetros obrigatórios para suportar o encaminhamento para o Domínio do Event Grid e Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="ec939-576">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="ec939-577">Adição de novos parâmetros obrigatórios para especificar o nome do Domínio do Event Grid e/ou nome do Tópico de Domínio do Event Grid, para permitir a remoção de uma subscrição de evento existente nestes recursos.</span><span class="sxs-lookup"><span data-stu-id="ec939-577">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="ec939-578">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ec939-578">Az.FrontDoor</span></span>
* <span data-ttu-id="ec939-579">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="ec939-579">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="ec939-580">Adição de suporte de transformações e do novo valor de preenchimento automático de operador (RegEx)</span><span class="sxs-lookup"><span data-stu-id="ec939-580">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="ec939-581">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="ec939-581">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="ec939-582">Adição de novos valores de preenchimento automático</span><span class="sxs-lookup"><span data-stu-id="ec939-582">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-583">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-583">Az.Network</span></span>
* <span data-ttu-id="ec939-584">Adição de suporte para o Recurso de Gateway de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="ec939-584">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="ec939-585">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-585">New cmdlets</span></span>
        - <span data-ttu-id="ec939-586">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="ec939-586">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="ec939-587">Adição de AvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="ec939-587">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="ec939-588">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-588">New cmdlets</span></span> 
        - <span data-ttu-id="ec939-589">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="ec939-589">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="ec939-590">Adição de PrivatePrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ec939-590">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="ec939-591">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-591">New cmdlets</span></span> 
        - <span data-ttu-id="ec939-592">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ec939-592">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="ec939-593">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ec939-593">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ec939-594">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="ec939-594">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="ec939-595">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-595">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="ec939-596">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-596">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="ec939-597">Adição de PrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ec939-597">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="ec939-598">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-598">New cmdlets</span></span>
        - <span data-ttu-id="ec939-599">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ec939-599">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ec939-600">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ec939-600">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ec939-601">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="ec939-601">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="ec939-602">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-602">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="ec939-603">Foram atualizados os seguintes comandos para a funcionalidade: Sinalizador UseLocalAzureIpAddress em VpnConnection</span><span class="sxs-lookup"><span data-stu-id="ec939-603">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="ec939-604">New-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve ser utilizado como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="ec939-604">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="ec939-605">Set-AzVpnConnection atualizado: Foi adicionado o parâmetro opcional -UseLocalAzureIpAddress para indicar que o endereço ip do azure local deve servir como endereço de origem ao iniciar a ligação.</span><span class="sxs-lookup"><span data-stu-id="ec939-605">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="ec939-606">Foi adicionado o campo só de leitura PeeredConnections no peering de ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ec939-606">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="ec939-607">Foi adicionado o campo só de leitura GlobalReachEnabled no ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ec939-607">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="ec939-608">Foi adicionado o atributo de alteração interruptiva para chamar a descontinuação do campo AllowGlobalReach no modelo ExpressRouteCircuit</span><span class="sxs-lookup"><span data-stu-id="ec939-608">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="ec939-609">Foi corrigido o Problema 8756 Erro ao utilizar TargetListenerID com os cmdlets AzApplicationGatewayRedirectConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-609">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="ec939-610">Foi corrigido o erro em New-AzApplicationGatewayPathRuleConfig que impedia a definição do conjunto de regras de rescrita.</span><span class="sxs-lookup"><span data-stu-id="ec939-610">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="ec939-611">Foi corrigida a apresentação de VirtualNetworkTaps em NetworkInterfaceIpConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-611">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="ec939-612">Foram corrigidos os cmdlets Get do Cortex para listagem de todas as peças</span><span class="sxs-lookup"><span data-stu-id="ec939-612">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="ec939-613">Foi corrigida a criação da referência VirtualHub para ExpressRouteGateways, VpnGateway</span><span class="sxs-lookup"><span data-stu-id="ec939-613">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="ec939-614">Foi adicionado suporte para Zonas de Disponibilidade no AzureFirewall e NatGateway</span><span class="sxs-lookup"><span data-stu-id="ec939-614">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="ec939-615">Foi adicionado o cmdlet Get-AzNetworkServiceTag</span><span class="sxs-lookup"><span data-stu-id="ec939-615">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="ec939-616">Adição de suporte para vários endereços IP públicos para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="ec939-616">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="ec939-617">cmdlet New-AzFirewall atualizado:</span><span class="sxs-lookup"><span data-stu-id="ec939-617">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="ec939-618">Foi adicionado o parâmetro -PublicIpAddress que aceita um ou mais objetos de Endereço IP Público</span><span class="sxs-lookup"><span data-stu-id="ec939-618">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="ec939-619">Foi adicionado o parâmetro -VirtualNetwork que aceita um objeto de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="ec939-619">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="ec939-620">Foram adicionados os métodos AddPublicIpAddress e RemovePublicIpAddress no objeto de firewall - estes métodos aceitam um objeto de Endereço IP Público como entrada</span><span class="sxs-lookup"><span data-stu-id="ec939-620">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="ec939-621">Foram preteridos os parâmetros -PublicIpName e -VirtualNetworkName</span><span class="sxs-lookup"><span data-stu-id="ec939-621">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="ec939-622">Foram atualizados os seguintes comandos para a funcionalidade: Definição de opções de autenticação do AAD de VpnClient para o recurso de gateway de rede Virtual.</span><span class="sxs-lookup"><span data-stu-id="ec939-622">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="ec939-623">New-AzVirtualNetworkGateway atualizado: Foram adicionados os parâmetros opcionais AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="ec939-623">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="ec939-624">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional AadTenantUri,AadAudienceId,AadIssuerUri para definir opções de autenticação do AAD de VpnClient no Gateway.</span><span class="sxs-lookup"><span data-stu-id="ec939-624">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="ec939-625">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional RemoveAadAuthentication para remover as opções de autenticação do AAD de VpnClient AAD do Gateway.</span><span class="sxs-lookup"><span data-stu-id="ec939-625">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ec939-626">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-626">Az.OperationalInsights</span></span>
* <span data-ttu-id="ec939-627">Ativar escalão de preço **pergb2018** no comando "New-AzureRmOperationalInsightsWorkspace"</span><span class="sxs-lookup"><span data-stu-id="ec939-627">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-628">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-628">Az.Resources</span></span>
* <span data-ttu-id="ec939-629">Suporte para opções adicionais de Exportação de Modelo</span><span class="sxs-lookup"><span data-stu-id="ec939-629">Support for additional Template Export options</span></span>
    - <span data-ttu-id="ec939-630">Adicionar parâmetro "-SkipResourceNameParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="ec939-630">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="ec939-631">Adicionar parâmetro "-SkipAllParameterization" a Export-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="ec939-631">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="ec939-632">Adicionar parâmetro "-Resource" a Export-AzResourceGroup para filtragem de recursos exportados</span><span class="sxs-lookup"><span data-stu-id="ec939-632">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ec939-633">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-633">Az.ServiceFabric</span></span>
* <span data-ttu-id="ec939-634">Corrigir adição do certificado ByExistingKeyVault que obtinha o thumbprint incorreto em alguns casos</span><span class="sxs-lookup"><span data-stu-id="ec939-634">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-635">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-635">Az.Sql</span></span>
* <span data-ttu-id="ec939-636">Corrigir sufixo do ponto final de armazenamento do Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="ec939-636">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="ec939-637">Corrigir ativação do Advanced Data Security que substitui a política Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="ec939-637">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="ec939-638">Novos Cmdlets para Management.Sql para permitir que os clientes adicionem chaves de Encriptação de Dados Transparente (TDE) e definam o protetor de Encriptação de Dados Transparente (TDE) para instâncias geridas</span><span class="sxs-lookup"><span data-stu-id="ec939-638">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="ec939-639">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ec939-639">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ec939-640">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ec939-640">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ec939-641">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="ec939-641">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="ec939-642">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="ec939-642">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="ec939-643">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="ec939-643">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-644">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-644">Az.Storage</span></span>
* <span data-ttu-id="ec939-645">Suporte de Kind FileStorage e SkuName Premium_ZRS ao criar a conta de armazenamento</span><span class="sxs-lookup"><span data-stu-id="ec939-645">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="ec939-646">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-646">New-AzStorageAccount</span></span>
* <span data-ttu-id="ec939-647">Foi clarificada a descrição do cmdlet de imutabilidade do blob</span><span class="sxs-lookup"><span data-stu-id="ec939-647">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="ec939-648">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-648">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-649">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-649">Az.Websites</span></span>
* <span data-ttu-id="ec939-650">Otimiza Get-AzWebAppCertificate para filtrar por grupo de recursos no servidor em vez do cliente</span><span class="sxs-lookup"><span data-stu-id="ec939-650">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="ec939-651">Adiciona o parâmetro opcional -UseDisasterRecovery a Get-AzWebAppSnapshot</span><span class="sxs-lookup"><span data-stu-id="ec939-651">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="ec939-652">2.2.0 - Junho de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-652">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="ec939-653">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ec939-653">Az.Cdn</span></span>
* <span data-ttu-id="ec939-654">Cmdlets atualizados para suportar a funcionalidade rulesEngine com base na versão de API de 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="ec939-654">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-655">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-655">Az.Compute</span></span>
* <span data-ttu-id="ec939-656">Foi adicionado o parâmetro `NoWait` que inicia a operação e devolve imediatamente, antes da conclusão da operação.</span><span class="sxs-lookup"><span data-stu-id="ec939-656">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="ec939-657">cmdlets atualizados:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="ec939-657">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ec939-658">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ec939-658">Az.EventHub</span></span>
* <span data-ttu-id="ec939-659">Correção para #9231 - Get-AzEventHubNamespace não devolve etiquetas</span><span class="sxs-lookup"><span data-stu-id="ec939-659">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="ec939-660">Correção para #9230 - Get-AzEventHubNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="ec939-660">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-661">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-661">Az.Network</span></span>
* <span data-ttu-id="ec939-662">Atualização de ResourceId e InputObject para o NAT Gateway</span><span class="sxs-lookup"><span data-stu-id="ec939-662">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="ec939-663">Adição do alias para ResourceId e InputObject</span><span class="sxs-lookup"><span data-stu-id="ec939-663">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ec939-664">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-664">Az.PolicyInsights</span></span>
* <span data-ttu-id="ec939-665">Correção do problema de referência Null em Get-AzPolicyEvent</span><span class="sxs-lookup"><span data-stu-id="ec939-665">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-666">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-666">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-667">Retenção mínima da política IaaSVM em dias alterada de 1 para 7</span><span class="sxs-lookup"><span data-stu-id="ec939-667">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ec939-668">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ec939-668">Az.ServiceBus</span></span>
* <span data-ttu-id="ec939-669">Correção do problema #9182 - Get-AzServiceBusNamespace devolve ResourceGroup em vez de ResourceGroupName</span><span class="sxs-lookup"><span data-stu-id="ec939-669">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ec939-670">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-670">Az.ServiceFabric</span></span>
* <span data-ttu-id="ec939-671">Correção da mensagem de erro para "Update-AzServiceFabricReliability"</span><span class="sxs-lookup"><span data-stu-id="ec939-671">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="ec939-672">Correção do caráter em falta nos cmdlines do Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ec939-672">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-673">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-673">Az.Sql</span></span>
* <span data-ttu-id="ec939-674">Adição do parâmetro DnsZonePartner para o cmdlet New-AzureSqlInstance para suportar AutoDr para a Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="ec939-674">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="ec939-675">Descontinuação do cmdlet Get-AzSqlDatabaseSecureConnectionPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-675">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="ec939-676">Mudança do nome dos cmdlets para o Advanced Threat Protection</span><span class="sxs-lookup"><span data-stu-id="ec939-676">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="ec939-677">Os parâmetros New-AzSqlInstance -StorageSizeInGB e -LicenseType são agora opcionais.</span><span class="sxs-lookup"><span data-stu-id="ec939-677">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-678">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-678">Az.Websites</span></span>
* <span data-ttu-id="ec939-679">corrige o problema em que a utilização de Set-AzWebApp e Set-AzWebAppSlot com a propriedade -WebApp remove as etiquetas</span><span class="sxs-lookup"><span data-stu-id="ec939-679">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="ec939-680">2.1.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-680">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="ec939-681">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-681">Az.ApiManagement</span></span>
* <span data-ttu-id="ec939-682">Foram criados novos Cmdlets para gerir diagnósticos no âmbito global e da API</span><span class="sxs-lookup"><span data-stu-id="ec939-682">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="ec939-683">**Get-AzApiManagementDiagnostic** - permite obter um âmbito global ou da API para o diagnóstico configurado</span><span class="sxs-lookup"><span data-stu-id="ec939-683">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="ec939-684">**New-AzApiManagementDiagnostic** - permite criar um novo diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="ec939-684">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="ec939-685">**New-AzApiManagementHttpMessageDiagnostic** - permite criar a definição de diagnóstico para os Cabeçalhos a registar e o tamanho de Bytes do Corpo</span><span class="sxs-lookup"><span data-stu-id="ec939-685">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="ec939-686">**New-AzApiManagementPipelineDiagnosticSetting** - permite criar definições de diagnóstico para mensagens HTTP de entrada/saída para o Gateway.</span><span class="sxs-lookup"><span data-stu-id="ec939-686">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="ec939-687">**New-AzApiManagementSamplingSetting** - permite criar a Definição de Amostragem para os pedidos/resposta de um diagnóstico</span><span class="sxs-lookup"><span data-stu-id="ec939-687">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="ec939-688">**Remove-AzApiManagementDiagnostic** - permite remover uma entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="ec939-688">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="ec939-689">**Set-AzApiManagementDiagnostic** - permite atualizar uma Entidade de diagnóstico no âmbito global ou da API</span><span class="sxs-lookup"><span data-stu-id="ec939-689">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="ec939-690">Foram criados novos Cmdlets para gerir a Cache no serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-690">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="ec939-691">**Get-AzApiManagementCache** - permite obter os detalhes da Cache especificada pelo identificador ou todas as caches</span><span class="sxs-lookup"><span data-stu-id="ec939-691">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="ec939-692">**New-AzApiManagementCache** - permite criar uma nova Cache predefinida ou numa região do Azure específica</span><span class="sxs-lookup"><span data-stu-id="ec939-692">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="ec939-693">**Remove-AzApiManagementCache** - permite remover uma cache</span><span class="sxs-lookup"><span data-stu-id="ec939-693">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="ec939-694">**Update-AzApiManagementCache** - permite atualizar uma cache</span><span class="sxs-lookup"><span data-stu-id="ec939-694">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="ec939-695">Foram criados novos Cmdlets para gerir o Esquema da API</span><span class="sxs-lookup"><span data-stu-id="ec939-695">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="ec939-696">**New-AzApiManagementSchema** - permite criar um novo Esquema para uma API</span><span class="sxs-lookup"><span data-stu-id="ec939-696">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="ec939-697">**Get-AzApiManagementSchema** - permite obter os esquemas configurados na API</span><span class="sxs-lookup"><span data-stu-id="ec939-697">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="ec939-698">**Remove-AzApiManagementSchema** - permite remover o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="ec939-698">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="ec939-699">**Set-AzApiManagementSchema** - permite atualizar o esquema configurado na API</span><span class="sxs-lookup"><span data-stu-id="ec939-699">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="ec939-700">Foi criado o novo Cmdlet para gerar um Token de Utilizador.</span><span class="sxs-lookup"><span data-stu-id="ec939-700">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="ec939-701">**New-AzApiManagementUserToken** - permite gerar um novo Token de Utilizador válido por 8 horas por predefinição. O Token para o utilizador "GIT" pode ser gerado com este cmdlet./</span><span class="sxs-lookup"><span data-stu-id="ec939-701">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="ec939-702">Foi criado um novo cmdlet para obter o Estado da Rede</span><span class="sxs-lookup"><span data-stu-id="ec939-702">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="ec939-703">**Get-AzApiManagementNetworkStatus** - permite obter a conectividade de recursos do estado da rede da qual depende a Gestão de API.</span><span class="sxs-lookup"><span data-stu-id="ec939-703">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="ec939-704">Isto é útil ao implementar o serviço ApiManagement numa Rede Virtual e ao validar se qualquer uma das dependências está quebrada.</span><span class="sxs-lookup"><span data-stu-id="ec939-704">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="ec939-705">Foi atualizado o cmdlet **New-AzApiManagement** para gerir o serviço ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-705">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="ec939-706">Foi adicionado suporte para o novo SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="ec939-706">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="ec939-707">Foi adicionado suporte para ativar o sinalizador "EnableClientCertificate" para o SKU "Consumption"</span><span class="sxs-lookup"><span data-stu-id="ec939-707">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="ec939-708">O novo cmdlet **New-AzApiManagementSslSetting** permite configurar a definição "TLS/SSL" no "Back-end" e "Front-end".</span><span class="sxs-lookup"><span data-stu-id="ec939-708">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="ec939-709">Isto também pode ser utilizado para configurar "Cifras" como "3DES" e "ServerProtocols" como "Http2" no "Front-end"de um serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="ec939-709">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="ec939-710">Foi adicionado suporte para configurar o nome de anfitrião "DeveloperPortal" no serviço ApiManagement.</span><span class="sxs-lookup"><span data-stu-id="ec939-710">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="ec939-711">Foram atualizados os cmdlets **Get-AzApiManagementSsoToken** para assumir o objeto "PsApiManagement" como entrada</span><span class="sxs-lookup"><span data-stu-id="ec939-711">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="ec939-712">Foi atualizado o cmdlet para apresentar Mensagens de Erro inline</span><span class="sxs-lookup"><span data-stu-id="ec939-712">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="ec939-713">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy: Código de Erro: Mensagem de Erro ValidationError: Um ou mais campos contêm valores incorretos: Detalhes do Erro:    [Code=ValidationError, Message=Error no elemento 'log-to-eventhub' na linha 3, coluna 10: O logger não foi encontrado, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="ec939-713">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="ec939-714">Foi atualizado o cmdlet **Export-AzApiManagementApi** para exportar APIs no formato "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="ec939-714">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="ec939-715">Foi atualizado o cmdlet **Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="ec939-715">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="ec939-716">Para importar a API da especificação de documento "OpenApi 3.0"</span><span class="sxs-lookup"><span data-stu-id="ec939-716">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="ec939-717">Para substituir a propriedade "PsApiManagementSchema" especificada em qualquer documento ("Swagger", "Wadl", "Wsdl", "OpenApi").</span><span class="sxs-lookup"><span data-stu-id="ec939-717">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="ec939-718">Para substituir a propriedade "ServiceUrl" especificada em qualquer documento.</span><span class="sxs-lookup"><span data-stu-id="ec939-718">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="ec939-719">Foi atualizado o cmdlet **Get-AzApiManagementPolicy** para devolver a política num "formato" sem escape de XML com "rawxml"</span><span class="sxs-lookup"><span data-stu-id="ec939-719">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="ec939-720">Foi atualizado o cmdlet **Set-AzApiManagementPolicy** para aceitar a política num "formato" com e sem escape de XML com "xml"</span><span class="sxs-lookup"><span data-stu-id="ec939-720">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="ec939-721">Foi atualizado o cmdlet **New-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="ec939-721">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="ec939-722">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="ec939-722">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="ec939-723">Para criar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="ec939-723">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="ec939-724">Para clonar uma API com "SourceApiId" e "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="ec939-724">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="ec939-725">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="ec939-725">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="ec939-726">Foi atualizado o cmdlet **Set-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="ec939-726">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="ec939-727">Para configurar a API com o servidor de autorização "OpenId".</span><span class="sxs-lookup"><span data-stu-id="ec939-727">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="ec939-728">Para atualizar uma API num "ApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="ec939-728">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="ec939-729">Capacidade de configurar "SubscriptionRequired" no âmbito da API.</span><span class="sxs-lookup"><span data-stu-id="ec939-729">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="ec939-730">Foi atualizado o cmdlet **New-AzApiManagementRevision**</span><span class="sxs-lookup"><span data-stu-id="ec939-730">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="ec939-731">Para clonar (etiquetas de cópia, produtos, operações e políticas) uma revisão existente com "SourceApiRevision".</span><span class="sxs-lookup"><span data-stu-id="ec939-731">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="ec939-732">A nova Revisão assume o "ApiId" do elemento principal.</span><span class="sxs-lookup"><span data-stu-id="ec939-732">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="ec939-733">Para fornecer uma "ApiRevisionDescription"</span><span class="sxs-lookup"><span data-stu-id="ec939-733">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="ec939-734">Para substituir o "ServiceUrl" ao clonar uma API.</span><span class="sxs-lookup"><span data-stu-id="ec939-734">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="ec939-735">Foi atualizado o cmdlet **New-AzApiManagementIdentityProvider**</span><span class="sxs-lookup"><span data-stu-id="ec939-735">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="ec939-736">Para configurar "AAD" ou "AADB2C" com uma "Autoridade"</span><span class="sxs-lookup"><span data-stu-id="ec939-736">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="ec939-737">Para configurar "SignupPolicy", "SigninPolicy", "ProfileEditingPolicy" e "PasswordResetPolicy"</span><span class="sxs-lookup"><span data-stu-id="ec939-737">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="ec939-738">Foi atualizado o cmdlet **New-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="ec939-738">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="ec939-739">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="ec939-739">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="ec939-740">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="ec939-740">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="ec939-741">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="ec939-741">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="ec939-742">Foi atualizado o cmdlet **Set-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="ec939-742">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="ec939-743">Para considerar o novo SubscriptonModel com "Scope" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="ec939-743">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="ec939-744">Para considerar o antigo modelo de subscrição com "ProductId" e "UserId"</span><span class="sxs-lookup"><span data-stu-id="ec939-744">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="ec939-745">Adição do suporte para ativar "AllowTracing" ao nível da subscrição.</span><span class="sxs-lookup"><span data-stu-id="ec939-745">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="ec939-746">Foram atualizados os seguintes cmdlets para aceitar "ResourceId" como entrada</span><span class="sxs-lookup"><span data-stu-id="ec939-746">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="ec939-747">"New-AzApiManagementContext"</span><span class="sxs-lookup"><span data-stu-id="ec939-747">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="ec939-748">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="ec939-748">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="ec939-749">"Get-AzApiManagementApiRelease"</span><span class="sxs-lookup"><span data-stu-id="ec939-749">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="ec939-750">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="ec939-750">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="ec939-751">"Get-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="ec939-751">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="ec939-752">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="ec939-752">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="ec939-753">"Get-AzApiManagementAuthorizationServer"</span><span class="sxs-lookup"><span data-stu-id="ec939-753">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="ec939-754">"Get-AzApiManagementBackend"</span><span class="sxs-lookup"><span data-stu-id="ec939-754">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="ec939-755">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="ec939-755">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="ec939-756">"Get-AzApiManagementCertificate"</span><span class="sxs-lookup"><span data-stu-id="ec939-756">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="ec939-757">"Remove-AzApiManagementApiVersionSet"</span><span class="sxs-lookup"><span data-stu-id="ec939-757">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="ec939-758">"Remove-AzApiManagementSubscription"</span><span class="sxs-lookup"><span data-stu-id="ec939-758">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-759">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-759">Az.Automation</span></span>
* <span data-ttu-id="ec939-760">Foi atualizado Get-AzAutomationJobOutputRecord para processar valores de registo de texto e JSON.</span><span class="sxs-lookup"><span data-stu-id="ec939-760">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="ec939-761">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="ec939-761">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="ec939-762">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="ec939-762">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="ec939-763">Foi alterado o comportamento de Start-AzAutomationDscCompilationJob para iniciar apenas a tarefa em vez de aguardar pela sua conclusão.</span><span class="sxs-lookup"><span data-stu-id="ec939-763">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="ec939-764">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="ec939-764">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="ec939-765">Correção para Get-AzAutomationDscNode quando utilizar -Name para devolver todos os nós.</span><span class="sxs-lookup"><span data-stu-id="ec939-765">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="ec939-766">Agora devolve apenas o nó correspondente.</span><span class="sxs-lookup"><span data-stu-id="ec939-766">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-767">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-767">Az.Compute</span></span>
* <span data-ttu-id="ec939-768">Adição dos parâmetros ProtectFromScaleIn e ProtectFromScaleSetAction ao cmdlet Update-AzVmssVM.</span><span class="sxs-lookup"><span data-stu-id="ec939-768">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="ec939-769">O parâmetro New-AzVM wimple definido utiliza agora por predefinição uma localização disponível se "E.U.A. Leste" não for suportado</span><span class="sxs-lookup"><span data-stu-id="ec939-769">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-770">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-770">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-771">Atualização do SDK do ADLS para utilizar httpclient e integrar os testes do plano de dados na arquitetura do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-771">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ec939-772">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-772">Az.Monitor</span></span>
* <span data-ttu-id="ec939-773">Foram corrigidos nomes de parâmetros incorretos nos exemplos de ajuda</span><span class="sxs-lookup"><span data-stu-id="ec939-773">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-774">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-774">Az.Network</span></span>
* <span data-ttu-id="ec939-775">Adição do sinalizador DisableBgpRoutePropagation à saída da Tabela de Rotas Efetivas</span><span class="sxs-lookup"><span data-stu-id="ec939-775">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="ec939-776">Cmdlet atualizado:</span><span class="sxs-lookup"><span data-stu-id="ec939-776">Updated cmdlet:</span></span>
        - <span data-ttu-id="ec939-777">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="ec939-777">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="ec939-778">Correção do traço duplo na documentação New-AzApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="ec939-778">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-779">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-779">Az.Resources</span></span>
* <span data-ttu-id="ec939-780">Adição do novo cmdlet Get-AzureRmDenyAssignment para obter atribuições de negação</span><span class="sxs-lookup"><span data-stu-id="ec939-780">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-781">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-781">Az.Sql</span></span>
* <span data-ttu-id="ec939-782">Mudança do nome dos cmdlets do Advanced Threat Protection para o Advanced Data Security e ativação da Avaliação de Vulnerabilidade por predefinição</span><span class="sxs-lookup"><span data-stu-id="ec939-782">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="ec939-783">2.0.0 - Maio de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-783">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-784">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-784">Az.Accounts</span></span>
* <span data-ttu-id="ec939-785">Atualização da Biblioteca de Autenticação para corrigir problemas do AD FS de autenticação com nome de utilizador/palavra-passe</span><span class="sxs-lookup"><span data-stu-id="ec939-785">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ec939-786">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ec939-786">Az.CognitiveServices</span></span>
* <span data-ttu-id="ec939-787">Apenas apresenta a exclusão de responsabilidade dos Serviços de Pesquisa do Bing.</span><span class="sxs-lookup"><span data-stu-id="ec939-787">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="ec939-788">Correção do erro quando a criação da conta falha.</span><span class="sxs-lookup"><span data-stu-id="ec939-788">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-789">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-789">Az.Compute</span></span>
* <span data-ttu-id="ec939-790">Funcionalidade do grupo de colocação em proximidade.</span><span class="sxs-lookup"><span data-stu-id="ec939-790">Proximity placement group feature.</span></span>
    - <span data-ttu-id="ec939-791">Foram adicionados os seguintes novos cmdlets:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="ec939-791">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="ec939-792">O novo parâmetro, ProximityPlacementGroupId, foi adicionado aos seguintes cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-792">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="ec939-793">O parâmetro StorageAccountType foi adicionado a New-AzGalleryImageVersion.</span><span class="sxs-lookup"><span data-stu-id="ec939-793">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="ec939-794">TargetRegion de New-AzGalleryImageVersion pode conter StorageAccountType.</span><span class="sxs-lookup"><span data-stu-id="ec939-794">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="ec939-795">O parâmetro opcional SkipShutdown foi adicionado a Stop-AzVM e Stop-AzVmss</span><span class="sxs-lookup"><span data-stu-id="ec939-795">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="ec939-796">Alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="ec939-796">Breaking changes</span></span>
    - <span data-ttu-id="ec939-797">Set-AzVMBootDiagnostics foi alterado para Set-AzVMBootDiagnostic.</span><span class="sxs-lookup"><span data-stu-id="ec939-797">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="ec939-798">Export-AzLogAnalyticThrottledRequests foi alterado para Export-AzLogAnalyticThrottledRequests.</span><span class="sxs-lookup"><span data-stu-id="ec939-798">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="ec939-799">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="ec939-799">Az.DeploymentManager</span></span>
* <span data-ttu-id="ec939-800">Primeira versão em Disponibilidade Geral dos cmdlets do Gestor de Implementação do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-800">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="ec939-801">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="ec939-801">Az.Dns</span></span>
* <span data-ttu-id="ec939-802">Delegação de NameServer de DNS automática</span><span class="sxs-lookup"><span data-stu-id="ec939-802">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="ec939-803">A criação de um cmdlet de zona DNS aceita o nome da zona principal como parâmetro opcional adicional.</span><span class="sxs-lookup"><span data-stu-id="ec939-803">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="ec939-804">Adiciona os registos NS na zona principal para a zona subordinada recém-criada.</span><span class="sxs-lookup"><span data-stu-id="ec939-804">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="ec939-805">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ec939-805">Az.FrontDoor</span></span>
* <span data-ttu-id="ec939-806">Primeira Versão em Disponibilidade Geral dos cmdlets do Azure Front Door Service</span><span class="sxs-lookup"><span data-stu-id="ec939-806">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="ec939-807">Alteração do nome dos cmdlets da WAF para incluir "Waf"</span><span class="sxs-lookup"><span data-stu-id="ec939-807">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="ec939-808">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec939-808">Az.HDInsight</span></span>
* <span data-ttu-id="ec939-809">Foram removidos dois cmdlets:</span><span class="sxs-lookup"><span data-stu-id="ec939-809">Removed two cmdlets:</span></span>
    - <span data-ttu-id="ec939-810">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ec939-810">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="ec939-811">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ec939-811">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="ec939-812">Foi adicionado um novo cmdlet Set-AzHDInsightGatewayCredential para substituir Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="ec939-812">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="ec939-813">O cmdlet Get-AzHDInsightJobOutput foi atualizado para distinguir a função de leitor da função de operador do hdinsight:</span><span class="sxs-lookup"><span data-stu-id="ec939-813">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="ec939-814">Os utilizadores com a função de leitor têm de especificar explicitamente o parâmetro "DefaultStorageAccountKey". Se não o fizerem, ocorre um erro.</span><span class="sxs-lookup"><span data-stu-id="ec939-814">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="ec939-815">Os utilizadores com a função de operador do HDInsight não serão afetados.</span><span class="sxs-lookup"><span data-stu-id="ec939-815">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ec939-816">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-816">Az.Monitor</span></span>
* <span data-ttu-id="ec939-817">Novos cmdlets para a API SQR (Regra de Consulta Agendada)</span><span class="sxs-lookup"><span data-stu-id="ec939-817">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="ec939-818">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="ec939-818">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="ec939-819">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="ec939-819">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="ec939-820">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="ec939-820">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="ec939-821">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="ec939-821">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="ec939-822">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="ec939-822">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="ec939-823">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="ec939-823">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="ec939-824">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ec939-824">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ec939-825">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ec939-825">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ec939-826">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ec939-826">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ec939-827">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ec939-827">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ec939-828">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="ec939-828">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="ec939-829">[Mais](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) informações sobre a API SQR</span><span class="sxs-lookup"><span data-stu-id="ec939-829">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="ec939-830">Az.Monitor.md foi atualizado para incluir cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="ec939-830">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-831">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-831">Az.Network</span></span>
* <span data-ttu-id="ec939-832">Foi adicionado suporte para o Recurso de Gateway de NAT</span><span class="sxs-lookup"><span data-stu-id="ec939-832">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="ec939-833">Novos cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-833">New cmdlets</span></span>
        - <span data-ttu-id="ec939-834">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ec939-834">New-AzNatGateway</span></span>
        - <span data-ttu-id="ec939-835">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ec939-835">Get-AzNatGateway</span></span>
        - <span data-ttu-id="ec939-836">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ec939-836">Set-AzNatGateway</span></span>
        - <span data-ttu-id="ec939-837">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="ec939-837">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="ec939-838">Cmdlets atualizados</span><span class="sxs-lookup"><span data-stu-id="ec939-838">Updated cmdlets</span></span>
        - <span data-ttu-id="ec939-839">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="ec939-839">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="ec939-840">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="ec939-840">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="ec939-841">Foram atualizados os seguintes comandos para a funcionalidade: Rotas personalizadas definidas/removidas em Brooklyn Gateway.</span><span class="sxs-lookup"><span data-stu-id="ec939-841">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="ec939-842">New-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="ec939-842">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="ec939-843">Set-AzVirtualNetworkGateway atualizado: Foi adicionado o parâmetro opcional -CustomRoute para definir os prefixos de endereço como rotas personalizadas a definir no Gateway.</span><span class="sxs-lookup"><span data-stu-id="ec939-843">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ec939-844">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-844">Az.PolicyInsights</span></span>
* <span data-ttu-id="ec939-845">Suporte para consultar os detalhes de avaliação da política.</span><span class="sxs-lookup"><span data-stu-id="ec939-845">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="ec939-846">Foi adicionado o parâmetro "-Expand" a Get-AzPolicyState.</span><span class="sxs-lookup"><span data-stu-id="ec939-846">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="ec939-847">Suporte para "-Expand PolicyEvaluationDetails".</span><span class="sxs-lookup"><span data-stu-id="ec939-847">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-848">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-848">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-849">Suporte para recuperação de sites Azure para o Azure entre subscrições.</span><span class="sxs-lookup"><span data-stu-id="ec939-849">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="ec939-850">Marcação das próximas alterações interruptivas do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="ec939-850">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="ec939-851">Correção para o plano de ação e o plano de recuperação do Azure Site Recovery.</span><span class="sxs-lookup"><span data-stu-id="ec939-851">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="ec939-852">Correção para o mapeamento de rede de atualização do Azure Site Recovery do Azure para o Azure.</span><span class="sxs-lookup"><span data-stu-id="ec939-852">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="ec939-853">Correção para a direção de proteção de atualização do Azure Site Recovery do Azure para o Azure para discos geridos.</span><span class="sxs-lookup"><span data-stu-id="ec939-853">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="ec939-854">Outras pequenas correções.</span><span class="sxs-lookup"><span data-stu-id="ec939-854">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="ec939-855">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="ec939-855">Az.Relay</span></span>
* <span data-ttu-id="ec939-856">Corrigir erros de digitação nas mensagens direcionadas ao cliente</span><span class="sxs-lookup"><span data-stu-id="ec939-856">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ec939-857">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ec939-857">Az.ServiceBus</span></span>
* <span data-ttu-id="ec939-858">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="ec939-858">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-859">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-859">Az.Storage</span></span>
* <span data-ttu-id="ec939-860">Atualização da Biblioteca de Cliente de Armazenamento 10.0.1 (o espaço de nomes de todos os objetos deste SDK mudam de "Microsoft.WindowsAzure.Storage. *" para "Microsoft.Azure.Storage.* ")</span><span class="sxs-lookup"><span data-stu-id="ec939-860">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="ec939-861">Atualização de Microsoft.Azure.Management.Storage 11.0.0 para suportar a nova versão de API 2019-04-01.</span><span class="sxs-lookup"><span data-stu-id="ec939-861">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="ec939-862">A Variante da Conta de armazenamento predefinida em Criar Conta de armazenamento muda de "Storage" para "StorageV2"</span><span class="sxs-lookup"><span data-stu-id="ec939-862">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="ec939-863">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-863">New-AzStorageAccount</span></span>
* <span data-ttu-id="ec939-864">Alteração do Sku.Name de saída do cmdlet da Conta de armazenamento para ficar alinhado com o SkuName de entrada ao adicionar "-" (por exemplo, "StandardLRS" muda para "Standard_LRS")</span><span class="sxs-lookup"><span data-stu-id="ec939-864">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="ec939-865">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-865">New-AzStorageAccount</span></span>
    - <span data-ttu-id="ec939-866">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-866">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="ec939-867">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-867">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-868">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-868">Az.Websites</span></span>
* <span data-ttu-id="ec939-869">A propriedade "Kind" passa a ser definida para objetos PSSite devolvidos por Get-AzWebApp</span><span class="sxs-lookup"><span data-stu-id="ec939-869">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="ec939-870">Marcação de Get-AzWebApp\*Metrics e Get-AzAppServicePlanMetrics preterida</span><span class="sxs-lookup"><span data-stu-id="ec939-870">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="ec939-871">1.8.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-871">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ec939-872">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="ec939-872">Highlights since the last major release</span></span>
* <span data-ttu-id="ec939-873">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="ec939-873">General availability of `Az` module</span></span>
* <span data-ttu-id="ec939-874">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ec939-874">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ec939-875">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ec939-875">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ec939-876">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-876">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ec939-877">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="ec939-877">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ec939-878">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-878">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ec939-879">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="ec939-879">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ec939-880">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-880">Az.Accounts</span></span>
* <span data-ttu-id="ec939-881">Atualize o Uninstall-AzureRm para eliminar corretamente os módulos no Mac</span><span class="sxs-lookup"><span data-stu-id="ec939-881">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="ec939-882">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ec939-882">Az.Batch</span></span>
* <span data-ttu-id="ec939-883">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-883">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ec939-884">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ec939-884">Az.Cdn</span></span>
* <span data-ttu-id="ec939-885">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-885">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ec939-886">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ec939-886">Az.CognitiveServices</span></span>
* <span data-ttu-id="ec939-887">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-887">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-888">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-888">Az.Compute</span></span>
* <span data-ttu-id="ec939-889">Corrigido o problema na instalação AEM se os ids de recurso dos discos tiverem o resourcegroups no id de recurso em letras minúsculas</span><span class="sxs-lookup"><span data-stu-id="ec939-889">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="ec939-890">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-890">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ec939-891">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="ec939-891">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-892">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-892">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-893">Adicione SsisProperties se o NodeCount não for nulo para o runtime de integração gerido.</span><span class="sxs-lookup"><span data-stu-id="ec939-893">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-894">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-894">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-895">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-895">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ec939-896">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ec939-896">Az.EventGrid</span></span>
* <span data-ttu-id="ec939-897">Atualizado o texto de ajuda do ponto final para indicar que os recursos devem ser criados antes de utilizar os cmdlets de subscrição de criação/atualização de evento.</span><span class="sxs-lookup"><span data-stu-id="ec939-897">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ec939-898">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ec939-898">Az.EventHub</span></span>
* <span data-ttu-id="ec939-899">Adicionados novos cmdlets para o NetworkRuleSet do Namespace</span><span class="sxs-lookup"><span data-stu-id="ec939-899">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="ec939-900">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="ec939-900">Az.HDInsight</span></span>
* <span data-ttu-id="ec939-901">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-901">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ec939-902">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ec939-902">Az.IotHub</span></span>
* <span data-ttu-id="ec939-903">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-903">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ec939-904">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec939-904">Az.KeyVault</span></span>
* <span data-ttu-id="ec939-905">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-905">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ec939-906">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="ec939-906">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="ec939-907">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="ec939-907">Az.MachineLearning</span></span>
* <span data-ttu-id="ec939-908">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-908">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="ec939-909">Az.Media</span><span class="sxs-lookup"><span data-stu-id="ec939-909">Az.Media</span></span>
* <span data-ttu-id="ec939-910">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-910">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ec939-911">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-911">Az.Monitor</span></span>
  * <span data-ttu-id="ec939-912">Novos cmdlets para a regra de alerta baseada em métricas de GenV2 (não clássica)</span><span class="sxs-lookup"><span data-stu-id="ec939-912">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="ec939-913">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="ec939-913">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="ec939-914">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="ec939-914">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="ec939-915">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ec939-915">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="ec939-916">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ec939-916">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="ec939-917">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="ec939-917">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="ec939-918">Atualizado o SDK de Monitor para a versão 0.22.0-preview</span><span class="sxs-lookup"><span data-stu-id="ec939-918">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-919">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-919">Az.Network</span></span>
* <span data-ttu-id="ec939-920">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-920">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ec939-921">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="ec939-921">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="ec939-922">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="ec939-922">Az.NotificationHubs</span></span>
* <span data-ttu-id="ec939-923">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-923">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ec939-924">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-924">Az.OperationalInsights</span></span>
* <span data-ttu-id="ec939-925">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-925">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="ec939-926">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="ec939-926">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="ec939-927">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-927">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-928">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-928">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-929">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-929">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ec939-930">Atualizado o formato de tabela para SQL na VM do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-930">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="ec939-931">Adicionado um método alternativo para obter a localização no AzureFileShare</span><span class="sxs-lookup"><span data-stu-id="ec939-931">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="ec939-932">ScheduleRunDays atualizado no objeto SchedulePolicy, de acordo com fuso horário</span><span class="sxs-lookup"><span data-stu-id="ec939-932">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ec939-933">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ec939-933">Az.RedisCache</span></span>
* <span data-ttu-id="ec939-934">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-934">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-935">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-935">Az.Resources</span></span>
* <span data-ttu-id="ec939-936">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="ec939-936">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-937">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-937">Az.Sql</span></span>
* <span data-ttu-id="ec939-938">Substitua a dependência do Monitor de SDK com um código comum</span><span class="sxs-lookup"><span data-stu-id="ec939-938">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="ec939-939">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-939">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ec939-940">Melhorado o processo de classificação de várias colunas.</span><span class="sxs-lookup"><span data-stu-id="ec939-940">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="ec939-941">Inclua propriedades de sku (nome, família e capacidade da sku) em resposta a Get-AzSqlServerServiceObjective e formato enquanto tabela, por predefinição.</span><span class="sxs-lookup"><span data-stu-id="ec939-941">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="ec939-942">Capacidade de Get-AzSqlServerServiceObjective por localização sem ser necessário um servidor pré-existente na região.</span><span class="sxs-lookup"><span data-stu-id="ec939-942">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="ec939-943">Suporte para o parâmetro de fuso horário na criação de Instância Gerida.</span><span class="sxs-lookup"><span data-stu-id="ec939-943">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="ec939-944">Corrigida a documentação sobre carateres universais</span><span class="sxs-lookup"><span data-stu-id="ec939-944">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-945">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-945">Az.Websites</span></span>
* <span data-ttu-id="ec939-946">corrige Set-AzWebApp e Set-AzWebAppSlot para não remover as etiquetas ao executar</span><span class="sxs-lookup"><span data-stu-id="ec939-946">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="ec939-947">Atualizados os cmdlets com nomes no plural para singular e foram preteridos os nomes no plural.</span><span class="sxs-lookup"><span data-stu-id="ec939-947">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="ec939-948">Atualizado o SDK dos Websites.</span><span class="sxs-lookup"><span data-stu-id="ec939-948">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="ec939-949">Removida a propriedade AdminSiteName de PSAppServicePlan.</span><span class="sxs-lookup"><span data-stu-id="ec939-949">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="ec939-950">1.7.0 - Abril de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-950">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ec939-951">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="ec939-951">Highlights since the last major release</span></span>
* <span data-ttu-id="ec939-952">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="ec939-952">General availability of `Az` module</span></span>
* <span data-ttu-id="ec939-953">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ec939-953">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ec939-954">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ec939-954">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ec939-955">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-955">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ec939-956">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="ec939-956">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ec939-957">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-957">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ec939-958">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="ec939-958">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="ec939-959">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-959">Az.Accounts</span></span>
* <span data-ttu-id="ec939-960">Atualização de Add-AzEnvironment e Set-AzEnvironment para aceitar o parâmetro AzureAnalysisServicesEndpointResourceId</span><span class="sxs-lookup"><span data-stu-id="ec939-960">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ec939-961">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ec939-961">Az.AnalysisServices</span></span>
* <span data-ttu-id="ec939-962">Utilização de ServiceClient nos cmdlets de plano de dados e remoção da lógica de autenticação original</span><span class="sxs-lookup"><span data-stu-id="ec939-962">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="ec939-963">Transformação de Add-AzureASAccount num wrapper de Connect-AzAccount para evitar uma alteração interruptiva</span><span class="sxs-lookup"><span data-stu-id="ec939-963">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-964">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-964">Az.Automation</span></span>
* <span data-ttu-id="ec939-965">Correção do erro do cmdlet New-AzAutomationSoftwareUpdateConfiguration relativamente a Inclusões.</span><span class="sxs-lookup"><span data-stu-id="ec939-965">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="ec939-966">Agora, os parâmetros IncludedKbNumber e IncludedPackageNameMask devem funcionar.</span><span class="sxs-lookup"><span data-stu-id="ec939-966">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="ec939-967">Correção do erro do grupo dinâmico da gestão de atualização da automatização do azure</span><span class="sxs-lookup"><span data-stu-id="ec939-967">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-968">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-968">Az.Compute</span></span>
* <span data-ttu-id="ec939-969">Adição do parâmetro HyperVGeneration a New-AzDiskConfig e New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-969">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="ec939-970">Permitir a criação de VM com imagem de galeria de outros inquilinos.</span><span class="sxs-lookup"><span data-stu-id="ec939-970">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="ec939-971">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ec939-971">Az.ContainerInstance</span></span>
* <span data-ttu-id="ec939-972">Correção do problema no parâmetro -Command de New-AzContainerGroup, que adicionava um argumento vazio à direita</span><span class="sxs-lookup"><span data-stu-id="ec939-972">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-973">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-973">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-974">Atualização da versão do SDK de .Net do ADF para 3.0.2</span><span class="sxs-lookup"><span data-stu-id="ec939-974">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="ec939-975">Atualização do cmdlet Set-AzDataFactoryV2 com parâmetros extra para definições relacionadas com RepoConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ec939-975">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-976">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-976">Az.Resources</span></span>
* <span data-ttu-id="ec939-977">Melhor processamento dos fornecedores de "Get-AzResource" no fornecimento dos parâmetros "-ResourceId" ou "-ResourceGroupName", "-Name" e "-ResourceType"</span><span class="sxs-lookup"><span data-stu-id="ec939-977">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="ec939-978">Melhor processamento de erros para "Test-AzDeployment" e "Test-AzResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="ec939-978">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="ec939-979">Processamento de erros que ocorrem fora da validação da implementação e inclusão dos mesmos na saída do comando</span><span class="sxs-lookup"><span data-stu-id="ec939-979">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="ec939-980">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="ec939-980">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="ec939-981">Adição do parâmetro opcional "-IgnoreDynamicParameters" ao conjunto de cmdlets de implementação para ignorar os pedidos nos cenários de script e de tarefas</span><span class="sxs-lookup"><span data-stu-id="ec939-981">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="ec939-982">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="ec939-982">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-983">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-983">Az.Sql</span></span>
* <span data-ttu-id="ec939-984">Suporte para a Classificação de Dados de Base de Dados.</span><span class="sxs-lookup"><span data-stu-id="ec939-984">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-985">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-985">Az.Storage</span></span>
* <span data-ttu-id="ec939-986">Comunicação de erros de detalhe ao criar o contexto de Armazenamento com o parâmetro -UseConnectedAccount, mas sem iniciar sessão na conta do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-986">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="ec939-987">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="ec939-987">New-AzStorageContext</span></span>
* <span data-ttu-id="ec939-988">Suporte para a Gestão das Propriedades do Serviço Blob de uma conta de Armazenamento especificada com a API Plano de gestão</span><span class="sxs-lookup"><span data-stu-id="ec939-988">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="ec939-989">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="ec939-989">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="ec939-990">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="ec939-990">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="ec939-991">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-991">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="ec939-992">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-992">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="ec939-993">Suporte - AsJob para Blobs e carregamento de ficheiros e transferência de cmdlets</span><span class="sxs-lookup"><span data-stu-id="ec939-993">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="ec939-994">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ec939-994">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="ec939-995">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="ec939-995">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="ec939-996">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ec939-996">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="ec939-997">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="ec939-997">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="ec939-998">1.6.0 - março de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-998">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="ec939-999">Destaques desde a última versão principal</span><span class="sxs-lookup"><span data-stu-id="ec939-999">Highlights since the last major release</span></span>
* <span data-ttu-id="ec939-1000">Disponibilidade geral do módulo `Az`</span><span class="sxs-lookup"><span data-stu-id="ec939-1000">General availability of `Az` module</span></span>
* <span data-ttu-id="ec939-1001">Para obter mais informações sobre o módulo `Az`, visite o seguinte: https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="ec939-1001">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="ec939-1002">Foram adicionados os elementos de conclusão Location, ResourceGroup e ResourceName: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="ec939-1002">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="ec939-1003">Foi adicionado o suporte a carateres universais para os cmdlets Get para Az.Compute e Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1003">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="ec939-1004">Foi adicionada a autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="ec939-1004">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ec939-1005">Adicionado o suporte para runbooks do Python 2 em Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-1005">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="ec939-1006">Az.LogicApp: Novos cmdlets para as Assemblagens de Conta de Integração e Configuração em lote</span><span class="sxs-lookup"><span data-stu-id="ec939-1006">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-1007">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-1007">Az.Automation</span></span>
* <span data-ttu-id="ec939-1008">Alteração na gestão de atualizações de automatização do Azure para suportar as seguintes novas funcionalidades:</span><span class="sxs-lookup"><span data-stu-id="ec939-1008">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="ec939-1009">Agrupamento dinâmico</span><span class="sxs-lookup"><span data-stu-id="ec939-1009">Dynamic grouping</span></span>
    * <span data-ttu-id="ec939-1010">Script de pré-publicação</span><span class="sxs-lookup"><span data-stu-id="ec939-1010">Pre-Post script</span></span>
    * <span data-ttu-id="ec939-1011">Definição de reinício</span><span class="sxs-lookup"><span data-stu-id="ec939-1011">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1012">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1012">Az.Compute</span></span>
* <span data-ttu-id="ec939-1013">Foi corrigido o problema com a resolução do caminho em Get-AzVmBootDiagnosticsData</span><span class="sxs-lookup"><span data-stu-id="ec939-1013">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="ec939-1014">Atualização da biblioteca de cliente de Computação para 25.0.0.</span><span class="sxs-lookup"><span data-stu-id="ec939-1014">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ec939-1015">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec939-1015">Az.KeyVault</span></span>
* <span data-ttu-id="ec939-1016">Foi adicionado o suporte a carateres universais para os cmdlets KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec939-1016">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-1017">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1017">Az.Network</span></span>
* <span data-ttu-id="ec939-1018">Adicionado o suporte às Informações sobre Ameaças para o Azure Firewall</span><span class="sxs-lookup"><span data-stu-id="ec939-1018">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="ec939-1019">Adicionadas as Regras Personalizadas e o recurso de nível superior da Política de Firewall do Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="ec939-1019">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-1020">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1020">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-1021">Adicionado SnapshotRetentionInDays à política de VM do Azure para suportar o RP Instantâneo</span><span class="sxs-lookup"><span data-stu-id="ec939-1021">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="ec939-1022">Adicionado o suporte a pipe para anular o registo a contentores</span><span class="sxs-lookup"><span data-stu-id="ec939-1022">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1023">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1023">Az.Resources</span></span>
* <span data-ttu-id="ec939-1024">Atualizado o suporte a carateres universais para Get-AzResource e Get-AzResourceGroup</span><span class="sxs-lookup"><span data-stu-id="ec939-1024">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="ec939-1025">Atualizadas as credenciais utilizadas ao fazer chamadas genéricas para ARM</span><span class="sxs-lookup"><span data-stu-id="ec939-1025">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-1026">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1026">Az.Sql</span></span>
* <span data-ttu-id="ec939-1027">alterado o parâmetro (ExcludeDetectionType) dos cmdlets da Deteção de Ameaças de DetectionType para string[] para torná-lo mais durável a mudanças futuras quando forem adicionados novos DetectionTypes e também para suportar o preenchimento automático.</span><span class="sxs-lookup"><span data-stu-id="ec939-1027">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-1028">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-1028">Az.Storage</span></span>
* <span data-ttu-id="ec939-1029">Suporte para Obter/Definir/Remover Política de Gestão numa conta de Armazenamento</span><span class="sxs-lookup"><span data-stu-id="ec939-1029">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="ec939-1030">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-1030">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ec939-1031">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-1031">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ec939-1032">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-1032">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="ec939-1033">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="ec939-1033">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="ec939-1034">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="ec939-1034">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="ec939-1035">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="ec939-1035">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-1036">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-1036">Az.Websites</span></span>
* <span data-ttu-id="ec939-1037">Corrigido o erro no modelo ARM que interrompe a clonagem de todas as ranhuras com "New-AzWebApp-IncludeSourceWebAppSlots"</span><span class="sxs-lookup"><span data-stu-id="ec939-1037">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="ec939-1038">1.5.0 – Março de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-1038">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-1039">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1039">Az.Accounts</span></span>
* <span data-ttu-id="ec939-1040">Foi adicionado o comando "Register-AzModule" para suportar os cmdlets AutoRest gerados</span><span class="sxs-lookup"><span data-stu-id="ec939-1040">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="ec939-1041">Foram atualizados os exemplos de Connect-AzAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-1041">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-1042">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-1042">Az.Automation</span></span>
* <span data-ttu-id="ec939-1043">Foi corrigido um problema ao obter determinados agendamentos mensais em vários cmdlets da Automatização do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-1043">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="ec939-1044">Foi corrigido Get-AzAutomationDscNode que devolvia apenas os 20 nós principais.</span><span class="sxs-lookup"><span data-stu-id="ec939-1044">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="ec939-1045">Devolve agora todos os nós</span><span class="sxs-lookup"><span data-stu-id="ec939-1045">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ec939-1046">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ec939-1046">Az.Cdn</span></span>
* <span data-ttu-id="ec939-1047">Foram adicionados novos cmdlets do Powershell para Ativar/Desativar o HTTPS de Domínios Personalizados e foram preteridos os antigos</span><span class="sxs-lookup"><span data-stu-id="ec939-1047">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1048">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1048">Az.Compute</span></span>
* <span data-ttu-id="ec939-1049">Foi adicionado o suporte de carateres universais para cmdlets Get</span><span class="sxs-lookup"><span data-stu-id="ec939-1049">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-1050">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-1050">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-1051">Foi atualizada a versão do SDK .NET do ADF para a 3.0.1</span><span class="sxs-lookup"><span data-stu-id="ec939-1051">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ec939-1052">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ec939-1052">Az.LogicApp</span></span>
* <span data-ttu-id="ec939-1053">Foi corrigido ListWorkflows que apenas obtinha a primeira página de resultados</span><span class="sxs-lookup"><span data-stu-id="ec939-1053">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-1054">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1054">Az.Network</span></span>
* <span data-ttu-id="ec939-1055">Foi adicionado o suporte de carateres universais para cmdlets Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1055">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-1056">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1056">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-1057">Foi adicionado um servidor SQL ao suporte de VM do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-1057">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="ec939-1058">Atualização do SDK</span><span class="sxs-lookup"><span data-stu-id="ec939-1058">SDK Update</span></span>
* <span data-ttu-id="ec939-1059">Foi removida a verificação VMappContainer em Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="ec939-1059">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="ec939-1060">Foram adicionados os parâmetros Name e ServerName a Get-ProtectableItem</span><span class="sxs-lookup"><span data-stu-id="ec939-1060">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1061">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1061">Az.Resources</span></span>
* <span data-ttu-id="ec939-1062">Foi adicionado o parâmetro `-TemplateObject` aos cmdlets de implementação</span><span class="sxs-lookup"><span data-stu-id="ec939-1062">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="ec939-1063">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="ec939-1063">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="ec939-1064">Foi corrigido um problema de piping do resultado de `Get-AzResource` em `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="ec939-1064">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="ec939-1065">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="ec939-1065">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="ec939-1066">Foi corrigido um problema na alteração do tipo de dados JSON ao executar `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="ec939-1066">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="ec939-1067">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="ec939-1067">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-1068">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1068">Az.Sql</span></span>
* <span data-ttu-id="ec939-1069">AuditingEndpointsCommunicator está a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="ec939-1069">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="ec939-1070">Está a ser corrigido o comportamento de um caso de periferia ao criar novas definições de diagnóstico.</span><span class="sxs-lookup"><span data-stu-id="ec939-1070">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-1071">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-1071">Az.Storage</span></span>
* <span data-ttu-id="ec939-1072">Suporte de Kind BlockBlobStorage ao criar uma conta de Armazenamento      - New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-1072">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="ec939-1073">1.4.0 – Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-1073">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="ec939-1074">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1074">Az.AnalysisServices</span></span>
* <span data-ttu-id="ec939-1075">O cmdlet AddAzureASAccount foi preterido</span><span class="sxs-lookup"><span data-stu-id="ec939-1075">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-1076">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-1076">Az.Automation</span></span>
* <span data-ttu-id="ec939-1077">Atualização da ajuda para Import-AzAutomationDscNodeConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1077">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="ec939-1078">Foi adicionada a validação de nomes de configuração ao cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1078">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="ec939-1079">Processamento de erros melhorado para o cmdlet Import-AzAutomationDscConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1079">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="ec939-1080">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1080">Az.CognitiveServices</span></span>
* <span data-ttu-id="ec939-1081">Foi adicionado o parâmetro CustomSubdomainName como um novo parâmetro opcional para New-AzCognitiveServicesAccount, utilizado para especificar o subdomínio para o recurso.</span><span class="sxs-lookup"><span data-stu-id="ec939-1081">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1082">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1082">Az.Compute</span></span>
* <span data-ttu-id="ec939-1083">Foi corrigido o problema com os conjuntos de parâmetros de ID</span><span class="sxs-lookup"><span data-stu-id="ec939-1083">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="ec939-1084">Atualização de Get-AzVMExtension de modo a listar todas as extensões instaladas, caso não seja fornecido o parâmetro Name</span><span class="sxs-lookup"><span data-stu-id="ec939-1084">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="ec939-1085">Adição dos parâmetros Tag e ResourceId ao cmdlet Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="ec939-1085">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="ec939-1086">O Get-AzVmssVM sem ID de instância e com InstanceView tem capacidade para listar VMs de VMSS com a vista de instância.</span><span class="sxs-lookup"><span data-stu-id="ec939-1086">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-1087">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-1087">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-1088">Adição de cmdlets para a enumeração e restauro de itens eliminados de ADL</span><span class="sxs-lookup"><span data-stu-id="ec939-1088">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="ec939-1089">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="ec939-1089">Az.EventHub</span></span>
* <span data-ttu-id="ec939-1090">Foi adicionada a nova propriedade booleana SkipEmptyArchives a Ignorar Arquivos Vazios na classe CaptureDescription de Eventhub</span><span class="sxs-lookup"><span data-stu-id="ec939-1090">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="ec939-1091">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec939-1091">Az.KeyVault</span></span>
* <span data-ttu-id="ec939-1092">Foi corrigida a etiquetagem em Set-AzKeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="ec939-1092">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ec939-1093">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ec939-1093">Az.LogicApp</span></span>
* <span data-ttu-id="ec939-1094">Adição de sku básico para Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="ec939-1094">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="ec939-1095">Adição de XSLT 2.0, XSLT 3.0 e Tipos de Mapa de Líquidos</span><span class="sxs-lookup"><span data-stu-id="ec939-1095">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="ec939-1096">Novos cmdlets para Assemblies de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="ec939-1096">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="ec939-1097">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ec939-1097">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ec939-1098">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ec939-1098">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ec939-1099">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ec939-1099">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="ec939-1100">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="ec939-1100">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="ec939-1101">Novos cmdlets para Configuração de Lote de Contas de Integração</span><span class="sxs-lookup"><span data-stu-id="ec939-1101">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="ec939-1102">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1102">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ec939-1103">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1103">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ec939-1104">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1104">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="ec939-1105">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1105">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="ec939-1106">Atualização do SDK de Aplicação Lógica para a versão 4.1.0</span><span class="sxs-lookup"><span data-stu-id="ec939-1106">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="ec939-1107">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-1107">Az.Monitor</span></span>
* <span data-ttu-id="ec939-1108">Atualização da ajuda para Get-AzMetric</span><span class="sxs-lookup"><span data-stu-id="ec939-1108">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-1109">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1109">Az.Network</span></span>
* <span data-ttu-id="ec939-1110">Atualização do exemplo de ajuda para Add-AzApplicationGatewayCustomError</span><span class="sxs-lookup"><span data-stu-id="ec939-1110">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="ec939-1111">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-1111">Az.OperationalInsights</span></span>
* <span data-ttu-id="ec939-1112">Suporte adicional para as origens de dados Novo ApplicationInsights e Obter ApplicationInsights.</span><span class="sxs-lookup"><span data-stu-id="ec939-1112">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="ec939-1113">Foi adicionado o novo tipo "ApplicationInsights" para suportar as origens de dados Obter ApplicationInsights específico e Obter ApplicationInsights completo de uma determinada área de trabalho.</span><span class="sxs-lookup"><span data-stu-id="ec939-1113">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="ec939-1114">Foi adicionado o cmdlet New-AzOperationalInsightsApplicationInsightsDataSource para criação de origem de dados com base em parâmetros de recurso de Application-Insights específicos: ID da subscrição, resourceGroupName e nome.</span><span class="sxs-lookup"><span data-stu-id="ec939-1114">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="ec939-1115">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1115">Az.Resources</span></span>
* <span data-ttu-id="ec939-1116">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="ec939-1116">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="ec939-1117">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="ec939-1117">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="ec939-1118">Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="ec939-1118">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="ec939-1119">Correção de erro que impedia a criação repetida de KeyCredentials</span><span class="sxs-lookup"><span data-stu-id="ec939-1119">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-1120">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1120">Az.Sql</span></span>
* <span data-ttu-id="ec939-1121">Suporte adicionado para a camada Hyperscale da BD SQL</span><span class="sxs-lookup"><span data-stu-id="ec939-1121">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="ec939-1122">Foi corrigido o erro no qual o restauro podia falhar devido à definição de propriedades desnecessárias no pedido de restauro</span><span class="sxs-lookup"><span data-stu-id="ec939-1122">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-1123">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-1123">Az.Websites</span></span>
* <span data-ttu-id="ec939-1124">Correção de exemplo em Get-AzWebAppSlotMetrics</span><span class="sxs-lookup"><span data-stu-id="ec939-1124">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="ec939-1125">1.3.0 - Fevereiro de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-1125">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-1126">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1126">Az.Accounts</span></span>
* <span data-ttu-id="ec939-1127">Atualização para a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="ec939-1127">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ec939-1128">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1128">Az.AnalysisServices</span></span>
<span data-ttu-id="ec939-1129">Disponibilidade geral para o módulo Az.AnalysisServices.</span><span class="sxs-lookup"><span data-stu-id="ec939-1129">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1130">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1130">Az.Compute</span></span>
* <span data-ttu-id="ec939-1131">Extensão AEM: Suporte adicionado para discos UltraSSD, P60, P70 e P80</span><span class="sxs-lookup"><span data-stu-id="ec939-1131">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="ec939-1132">Descrição de ajuda atualizada para Set-AzVMBootDiagnostics</span><span class="sxs-lookup"><span data-stu-id="ec939-1132">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="ec939-1133">Descrição de ajuda e exemplo atualizados para Update-AzImage</span><span class="sxs-lookup"><span data-stu-id="ec939-1133">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-1134">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1134">Az.RecoveryServices</span></span>
<span data-ttu-id="ec939-1135">Disponibilidade geral para o módulo Az.RecoveryServices.</span><span class="sxs-lookup"><span data-stu-id="ec939-1135">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1136">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1136">Az.Resources</span></span>
* <span data-ttu-id="ec939-1137">As etiquetas dos grupos de recursos foram corrigidas</span><span class="sxs-lookup"><span data-stu-id="ec939-1137">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="ec939-1138">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="ec939-1138">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="ec939-1139">Foi corrigido o problema em que `Get-AzureRmRoleAssignment` não respeitava -ErrorAction</span><span class="sxs-lookup"><span data-stu-id="ec939-1139">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="ec939-1140">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="ec939-1140">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-1141">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1141">Az.Sql</span></span>
* <span data-ttu-id="ec939-1142">Foi adicionado Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="ec939-1142">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="ec939-1143">Foi corrigido o problema em que não ter sessão iniciada na conta do Azure resultava numa exceção nullref ao executar cmdlets de SQL</span><span class="sxs-lookup"><span data-stu-id="ec939-1143">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="ec939-1144">Exceção nullref corrigida em Get-AzSqlCapability</span><span class="sxs-lookup"><span data-stu-id="ec939-1144">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="ec939-1145">1.2.1 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-1145">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-1146">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1146">Az.Accounts</span></span>
* <span data-ttu-id="ec939-1147">Lançamento da versão correta de Autenticação</span><span class="sxs-lookup"><span data-stu-id="ec939-1147">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="ec939-1148">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1148">Az.AnalysisServices</span></span>
* <span data-ttu-id="ec939-1149">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="ec939-1149">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-1150">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1150">Az.RecoveryServices</span></span>
* <span data-ttu-id="ec939-1151">Versão com a dependência de Autenticação atualizada</span><span class="sxs-lookup"><span data-stu-id="ec939-1151">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="ec939-1152">1.2.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-1152">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-1153">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1153">Az.Accounts</span></span>
* <span data-ttu-id="ec939-1154">Foi adicionada autenticação interativa e por nome de utilizador/palavra-passe apenas para o Windows PowerShell 5.1</span><span class="sxs-lookup"><span data-stu-id="ec939-1154">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="ec939-1155">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1155">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ec939-1156">Foi adicionada uma mensagem de aviso no PS Core para Uninstall-AzureRm</span><span class="sxs-lookup"><span data-stu-id="ec939-1156">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="ec939-1157">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="ec939-1157">Az.Aks</span></span>
* <span data-ttu-id="ec939-1158">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1158">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="ec939-1159">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-1159">Az.Automation</span></span>
* <span data-ttu-id="ec939-1160">Suporte adicionado para runbooks do Python 2</span><span class="sxs-lookup"><span data-stu-id="ec939-1160">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="ec939-1161">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1161">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="ec939-1162">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="ec939-1162">Az.Cdn</span></span>
* <span data-ttu-id="ec939-1163">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1163">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1164">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1164">Az.Compute</span></span>
* <span data-ttu-id="ec939-1165">Foi adicionado o cmdlet Invoke-AzVMReimage</span><span class="sxs-lookup"><span data-stu-id="ec939-1165">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="ec939-1166">Foi adicionado o parâmetro TempDisk a Set-AzVmss</span><span class="sxs-lookup"><span data-stu-id="ec939-1166">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="ec939-1167">Foi corrigida a mensagem de aviso de New-AzVM</span><span class="sxs-lookup"><span data-stu-id="ec939-1167">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="ec939-1168">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="ec939-1168">Az.ContainerRegistry</span></span>
* <span data-ttu-id="ec939-1169">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1169">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="ec939-1170">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="ec939-1170">Az.DataFactory</span></span>
* <span data-ttu-id="ec939-1171">Foi atualizada a versão do SDK .NET do ADF para a 3.0.0</span><span class="sxs-lookup"><span data-stu-id="ec939-1171">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-1172">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-1172">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-1173">Foi corrigido o problema com o ponto final do ADLS ao utilizar o MSI</span><span class="sxs-lookup"><span data-stu-id="ec939-1173">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="ec939-1174">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="ec939-1174">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="ec939-1175">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1175">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ec939-1176">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ec939-1176">Az.IotHub</span></span>
* <span data-ttu-id="ec939-1177">Foi adicionado o formato de Codificação ao cmdlet Add-IotHubRoutingEndpoint.</span><span class="sxs-lookup"><span data-stu-id="ec939-1177">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="ec939-1178">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec939-1178">Az.KeyVault</span></span>
* <span data-ttu-id="ec939-1179">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1179">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-1180">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1180">Az.Network</span></span>
* <span data-ttu-id="ec939-1181">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1181">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1182">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1182">Az.Resources</span></span>
* <span data-ttu-id="ec939-1183">Foram corrigidos exemplos incorretos na documentação de referência de "AzADAppCredential" e "New-AzADSpCredential"</span><span class="sxs-lookup"><span data-stu-id="ec939-1183">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="ec939-1184">Foi corrigido o problema em que o caminho para o parâmetro "-TemplateFile" não estava a ser resolvido antes da execução dos cmdlets de implementação do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="ec939-1184">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="ec939-1185">Az.Resources: Foi corrigida a documentação do valor predefinido New-AzureRmPolicyDefinition -Mode</span><span class="sxs-lookup"><span data-stu-id="ec939-1185">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="ec939-1186">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="ec939-1186">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="ec939-1187">Az.Resources: Foi corrigido o problema https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="ec939-1187">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="ec939-1188">Foi corrigido o problema de formatação do objeto "PSResourceGroupDeployment"</span><span class="sxs-lookup"><span data-stu-id="ec939-1188">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="ec939-1189">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="ec939-1189">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ec939-1190">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-1190">Az.ServiceFabric</span></span>
* <span data-ttu-id="ec939-1191">Foi corrigido o erro de reversão quando é adicionado um certificado ao modelo VMSS, mas é devolvida uma exceção: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="ec939-1191">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="ec939-1192">Foram corrigidas algumas mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="ec939-1192">Fix some error messages.</span></span>
* <span data-ttu-id="ec939-1193">Foi corrigida a criação do cluster com o modelo ARM predefinido para New-AzServiceFabriCluster que não estava a funcionar na migração para o Az.</span><span class="sxs-lookup"><span data-stu-id="ec939-1193">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="ec939-1194">Foi corrigida a adição do cluster/certificado da aplicação para adicionar apenas a Conjuntos de Dimensionamento de VMs que correspondam ao cluster ao verificar o ID do cluster na extensão.</span><span class="sxs-lookup"><span data-stu-id="ec939-1194">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ec939-1195">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ec939-1195">Az.SignalR</span></span>
* <span data-ttu-id="ec939-1196">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1196">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-1197">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1197">Az.Sql</span></span>
* <span data-ttu-id="ec939-1198">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1198">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ec939-1199">Foi atualizada a descrição do parâmetro LicenseType com valores possíveis</span><span class="sxs-lookup"><span data-stu-id="ec939-1199">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="ec939-1200">Foi corrigida a atualização da identidade de instância gerida que não estava a funcionar quando é a única propriedade atualizada</span><span class="sxs-lookup"><span data-stu-id="ec939-1200">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="ec939-1201">Suporte para o agrupamento personalizado na instância gerida</span><span class="sxs-lookup"><span data-stu-id="ec939-1201">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-1202">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-1202">Az.Storage</span></span>
* <span data-ttu-id="ec939-1203">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1203">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ec939-1204">Enviar mensagem de erro detalhada quando obter/definir o Registo/Métrica clássica na Conta de Armazenamento Premium, uma vez que a Conta de Armazenamento Premium não suporta o Registo/Métrica clássica.</span><span class="sxs-lookup"><span data-stu-id="ec939-1204">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="ec939-1205">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="ec939-1205">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="ec939-1206">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="ec939-1206">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="ec939-1207">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ec939-1207">Az.TrafficManager</span></span>
* <span data-ttu-id="ec939-1208">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1208">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-1209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-1209">Az.Websites</span></span>
* <span data-ttu-id="ec939-1210">Foram atualizados URLs de ajuda online incorretos</span><span class="sxs-lookup"><span data-stu-id="ec939-1210">Update incorrect online help URLs</span></span>
* <span data-ttu-id="ec939-1211">Foi corrigido "New-AzWebAppSSLBinding" para carregar o certificado para o grupo de recursos/localização correta se a aplicação estiver alojada no ASE.</span><span class="sxs-lookup"><span data-stu-id="ec939-1211">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="ec939-1212">Foi corrigido "New-AzWebAppSSLBinding" para não substituir as etiquetas no enlace de um certificado SSL para uma aplicação</span><span class="sxs-lookup"><span data-stu-id="ec939-1212">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="ec939-1213">1.1.0 - Janeiro de 2019</span><span class="sxs-lookup"><span data-stu-id="ec939-1213">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="ec939-1214">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1214">Az.Accounts</span></span>
* <span data-ttu-id="ec939-1215">Foi adicionado o Âmbito "Local" a Enable-AzureRmAlias</span><span class="sxs-lookup"><span data-stu-id="ec939-1215">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1216">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1216">Az.Compute</span></span>
* <span data-ttu-id="ec939-1217">O nome passa a ser opcional no conjunto de parâmetros de ID de Restart/Start/Stop/Remove/Set-AzVM e Save-AzVMImage</span><span class="sxs-lookup"><span data-stu-id="ec939-1217">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="ec939-1218">Foi atualizada a descrição do ID nos ficheiros de ajuda</span><span class="sxs-lookup"><span data-stu-id="ec939-1218">Updated the description of ID in help files</span></span>
* <span data-ttu-id="ec939-1219">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1219">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-1220">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-1220">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-1221">Foi atualizada a versão do SDK do plano de dados para 1.1.14 para correções de SDK.</span><span class="sxs-lookup"><span data-stu-id="ec939-1221">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="ec939-1222">Foi corrigido o processamento de accesstime e modificationtime negativos para getfilestatus e liststatus. Foi corrigido o cancelamento assíncrono de token</span><span class="sxs-lookup"><span data-stu-id="ec939-1222">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="ec939-1223">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="ec939-1223">Az.EventGrid</span></span>
* <span data-ttu-id="ec939-1224">Foi atualizado para utilizar a versão de API 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="ec939-1224">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="ec939-1225">Foram atualizados os seguintes cmdlets para suportar o novo cenário na versão de API 2019-01-01</span><span class="sxs-lookup"><span data-stu-id="ec939-1225">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="ec939-1226">New-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="ec939-1226">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="ec939-1227">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="ec939-1227">Event Time-To-Live,</span></span>
        - <span data-ttu-id="ec939-1228">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="ec939-1228">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="ec939-1229">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="ec939-1229">Dead letter endpoint.</span></span>
    - <span data-ttu-id="ec939-1230">Update-AzureRmEventGridSubscription: Foram adicionados novos parâmetros opcionais para especificar:</span><span class="sxs-lookup"><span data-stu-id="ec939-1230">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="ec939-1231">TTL de Evento,</span><span class="sxs-lookup"><span data-stu-id="ec939-1231">Event Time-To-Live,</span></span>
        - <span data-ttu-id="ec939-1232">Número máximo de tentativas de entrega para os eventos,</span><span class="sxs-lookup"><span data-stu-id="ec939-1232">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="ec939-1233">Ponto final de mensagens não entregues.</span><span class="sxs-lookup"><span data-stu-id="ec939-1233">Dead letter endpoint.</span></span>
* <span data-ttu-id="ec939-1234">Foram adicionados novos valores de enumeração (nomeadamente, storageQueue e hybridConnection) para a opção EndpointType nos cmdlets New-AzureRmEventGridSubscription e Update-AzureRmEventGridSubscription.</span><span class="sxs-lookup"><span data-stu-id="ec939-1234">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="ec939-1235">É apresentada uma mensagem de aviso se se esperar que a criação ou atualização da subscrição de evento requeira alguma ação manual do utilizador.</span><span class="sxs-lookup"><span data-stu-id="ec939-1235">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="ec939-1236">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="ec939-1236">Az.IotHub</span></span>
* <span data-ttu-id="ec939-1237">Foi atualizado para a versão mais recente do SDK IotHub</span><span class="sxs-lookup"><span data-stu-id="ec939-1237">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="ec939-1238">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="ec939-1238">Az.LogicApp</span></span>
* <span data-ttu-id="ec939-1239">Get-AzLogicApp lista tudo sem um Nome especificado</span><span class="sxs-lookup"><span data-stu-id="ec939-1239">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1240">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1240">Az.Resources</span></span>
* <span data-ttu-id="ec939-1241">Foi corrigido o problema do conjunto de parâmetros ao fornecer os parâmetros "-ODataQuery" e "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="ec939-1241">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="ec939-1242">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="ec939-1242">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="ec939-1243">Foi corrigido o processamento do parâmetro -Custom em New/Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="ec939-1243">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="ec939-1244">Foi corrigido o erro de digitação na documentação de New-AzDeployment</span><span class="sxs-lookup"><span data-stu-id="ec939-1244">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="ec939-1245">Foi tornado obrigatório o parâmetro "-MailNickname" para "New-AzADUser"</span><span class="sxs-lookup"><span data-stu-id="ec939-1245">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="ec939-1246">Obtenha mais informações aqui: https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="ec939-1246">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="ec939-1247">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="ec939-1247">Az.SignalR</span></span>
* <span data-ttu-id="ec939-1248">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1248">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-1249">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1249">Az.Sql</span></span>
* <span data-ttu-id="ec939-1250">Foi convertida a dependência de cliente de gestão de Armazenamento para a implementação de SDK comum.</span><span class="sxs-lookup"><span data-stu-id="ec939-1250">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="ec939-1251">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-1251">Az.Storage</span></span>
* <span data-ttu-id="ec939-1252">Foi definido o StorageAccountName do contexto Armazenamento como o verdadeiro Nome de Conta de Armazenamento quando é criado com o Token de SAS, OAuth ou Anónimo</span><span class="sxs-lookup"><span data-stu-id="ec939-1252">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="ec939-1253">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="ec939-1253">New-AzStorageContext</span></span>
* <span data-ttu-id="ec939-1254">Foi criado o Token de SAS do Objeto de Instantâneo de Blob com o parâmetro "-FullUri". Foi corrigido o URI devolvido para ser o URI de instantâneo</span><span class="sxs-lookup"><span data-stu-id="ec939-1254">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="ec939-1255">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="ec939-1255">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-1256">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-1256">Az.Websites</span></span>
* <span data-ttu-id="ec939-1257">Foi corrigido um erro de análise de data em "Get-AzDeletedWebApp"</span><span class="sxs-lookup"><span data-stu-id="ec939-1257">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="ec939-1258">Foi corrigido o problema de retrocompatibilidade do módulo Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1258">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="ec939-1259">1.0.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="ec939-1259">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="ec939-1260">Geral</span><span class="sxs-lookup"><span data-stu-id="ec939-1260">General</span></span>

- <span data-ttu-id="ec939-1261">Disponibilidade Geral do Módulo do Az</span><span class="sxs-lookup"><span data-stu-id="ec939-1261">General Availability of Az Module</span></span>
- <span data-ttu-id="ec939-1262">Ajuda online para cada módulo</span><span class="sxs-lookup"><span data-stu-id="ec939-1262">Online help for each module</span></span>
- <span data-ttu-id="ec939-1263">Para obter mais detalhes e um mapa, veja a [página Anúncio do Az](https://aka.ms/azps-announce)</span><span class="sxs-lookup"><span data-stu-id="ec939-1263">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="ec939-1264">Veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter informações sobre como migrar a partir do AzureRM</span><span class="sxs-lookup"><span data-stu-id="ec939-1264">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="ec939-1265">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1265">Az.Accounts</span></span>
- <span data-ttu-id="ec939-1266">Nome para o qual foi alterado o nome anterior Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ec939-1266">Changed from Az.Profile</span></span>
- <span data-ttu-id="ec939-1267">Correção de formatos de tabela para tipos de perfil e de contexto</span><span class="sxs-lookup"><span data-stu-id="ec939-1267">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="ec939-1268">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-1268">Az.ApiManagement</span></span>
- <span data-ttu-id="ec939-1269">Correções para #7002</span><span class="sxs-lookup"><span data-stu-id="ec939-1269">Fixes for #7002</span></span>
- <span data-ttu-id="ec939-1270">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1270">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="ec939-1271">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="ec939-1271">Az.Batch</span></span>
- <span data-ttu-id="ec939-1272">Foi adicionada a capacidade de determinar a versão do Agente de Nós do Azure Batch em execução em cada uma das VMs de um conjunto, através da nova propriedade `NodeAgentInformation` em `PSComputeNode`.</span><span class="sxs-lookup"><span data-stu-id="ec939-1272">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="ec939-1273">A predefinição de `Caching` para `PSDataDisk` é agora `ReadWrite` em vez de `None`.</span><span class="sxs-lookup"><span data-stu-id="ec939-1273">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="ec939-1274">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1274">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="ec939-1275">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="ec939-1275">Az.Billing</span></span>
- <span data-ttu-id="ec939-1276">Combina os cmdlets Billing, Consumption e UsageAggregates; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1276">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="ec939-1277">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1277">Az.CognitivServices</span></span>
- <span data-ttu-id="ec939-1278">Foram adicionados elementos de preenchimento para SkuName e Typem disponíveis na operação New-AzureRmCognitiveServicesAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-1278">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="ec939-1279">Foi removido o conjunto de parâmetros GetSkusWithAccountParamSetName de Get-AzCognitiveServicesAccountSkus</span><span class="sxs-lookup"><span data-stu-id="ec939-1279">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="ec939-1280">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ec939-1280">Az.ContainerInstance</span></span>
- <span data-ttu-id="ec939-1281">Foi adicionado suporte de ManagedIdentity</span><span class="sxs-lookup"><span data-stu-id="ec939-1281">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="ec939-1282">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="ec939-1282">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="ec939-1283">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1283">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="ec939-1284">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-1284">Az.DataLakeStore</span></span>
- <span data-ttu-id="ec939-1285">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1285">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="ec939-1286">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="ec939-1286">Az.Monitor</span></span>
- <span data-ttu-id="ec939-1287">O nome Az.Insights foi mudado para Az.Monitor e outras pequenas alterações interruptivas; veja o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1287">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="ec939-1288">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="ec939-1288">Az.KeyVault</span></span>
- <span data-ttu-id="ec939-1289">A propriedade preterida "PurgeDisabled" foi removida dos tipos de saída</span><span class="sxs-lookup"><span data-stu-id="ec939-1289">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="ec939-1290">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="ec939-1290">Az.MachineLearning</span></span>
- <span data-ttu-id="ec939-1291">Foram incluídos os cmdlets do módulo Az.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="ec939-1291">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="ec939-1292">Az.Media</span><span class="sxs-lookup"><span data-stu-id="ec939-1292">Az.Media</span></span>
- <span data-ttu-id="ec939-1293">Foi removido o alias preterido -Tags de New-AzMediaService</span><span class="sxs-lookup"><span data-stu-id="ec939-1293">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="ec939-1294">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1294">Az.Network</span></span>
<span data-ttu-id="ec939-1295">Foi adicionado suporte para a configuração de RewriteRuleSets no Gateway de Aplicação</span><span class="sxs-lookup"><span data-stu-id="ec939-1295">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="ec939-1296">Foram adicionados novos cmdlets:</span><span class="sxs-lookup"><span data-stu-id="ec939-1296">New cmdlets added:</span></span>
        - <span data-ttu-id="ec939-1297">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-1297">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ec939-1298">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-1298">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ec939-1299">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-1299">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ec939-1300">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-1300">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ec939-1301">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-1301">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="ec939-1302">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="ec939-1302">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="ec939-1303">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="ec939-1303">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="ec939-1304">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec939-1304">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="ec939-1305">Foram atualizados cmdlets com o parâmetro opcional -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="ec939-1305">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="ec939-1306">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="ec939-1306">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="ec939-1307">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="ec939-1307">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="ec939-1308">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="ec939-1308">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="ec939-1309">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-1309">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="ec939-1310">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-1310">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="ec939-1311">New-AzureRmApplicationGatewayUrlPathMapConfig. Foi adicionado Suporte de KeyVault ao Gateway de Aplicação através da utilização de Identidade.</span><span class="sxs-lookup"><span data-stu-id="ec939-1311">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="ec939-1312">Foram atualizados cmdlets com o parâmetro -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="ec939-1312">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="ec939-1313">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ec939-1313">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="ec939-1314">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ec939-1314">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="ec939-1315">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="ec939-1315">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="ec939-1316">O cmdlet New-AzApplicationGateway foi atualizado com o parâmetro opcional -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="ec939-1316">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="ec939-1317">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1317">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="ec939-1318">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-1318">Az.OperationalInsights</span></span>
- <span data-ttu-id="ec939-1319">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1319">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="ec939-1320">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ec939-1320">Az.Profile</span></span>
- <span data-ttu-id="ec939-1321">O nome do módulo foi alterado para Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="ec939-1321">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-1322">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1322">Az.RecoveryServices</span></span>
- <span data-ttu-id="ec939-1323">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1323">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="ec939-1324">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1324">Az.Resources</span></span>
- <span data-ttu-id="ec939-1325">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1325">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="ec939-1326">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-1326">Az.ServiceFabric</span></span>
- <span data-ttu-id="ec939-1327">Suporte para a especificação do certificado pelo nome comum e thumbprint</span><span class="sxs-lookup"><span data-stu-id="ec939-1327">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="ec939-1328">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1328">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="ec939-1329">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="ec939-1329">Az.SIgnalR</span></span>
- <span data-ttu-id="ec939-1330">Disponibilidade Geral de cmdlets do PowerShell para o SignalR</span><span class="sxs-lookup"><span data-stu-id="ec939-1330">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="ec939-1331">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1331">Az.Sql</span></span>
- <span data-ttu-id="ec939-1332">Foram adicionados os novos tipos de deteção Data_Exfiltration e Unsafe_Action aos cmdlets de Deteção de Ameaças</span><span class="sxs-lookup"><span data-stu-id="ec939-1332">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="ec939-1333">Atualização de exemplos na documentação para os cmdlets de Auditoria de SQL</span><span class="sxs-lookup"><span data-stu-id="ec939-1333">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="ec939-1334">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1334">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="ec939-1335">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-1335">Az.Storage</span></span>
- <span data-ttu-id="ec939-1336">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1336">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="ec939-1337">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-1337">Az.Websites</span></span>
- <span data-ttu-id="ec939-1338">Pequenas alterações interruptivas; consulte o [Guia de Migração](https://aka.ms/azps-migration-guide) para obter detalhes</span><span class="sxs-lookup"><span data-stu-id="ec939-1338">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="ec939-1339">0.7.0 - Dezembro de 2018</span><span class="sxs-lookup"><span data-stu-id="ec939-1339">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="ec939-1340">Geral</span><span class="sxs-lookup"><span data-stu-id="ec939-1340">General</span></span>

* <span data-ttu-id="ec939-1341">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="ec939-1341">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="ec939-1342">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1342">Az.Compute</span></span>

* <span data-ttu-id="ec939-1343">Foi adicionado suporte para SSD Ultra e Imagens da Galeria nos conjuntos de parâmetros simples para cmdlets `New-AzVm(ss)`.</span><span class="sxs-lookup"><span data-stu-id="ec939-1343">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="ec939-1344">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-1344">Az.DataLakeStore</span></span>

* <span data-ttu-id="ec939-1345">Foi corrigida a barra final do domínio da conta do ADLS</span><span class="sxs-lookup"><span data-stu-id="ec939-1345">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="ec939-1346">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="ec939-1346">Az.FrontDoor</span></span>

* <span data-ttu-id="ec939-1347">Foram corrigidas algumas ligações quebradas</span><span class="sxs-lookup"><span data-stu-id="ec939-1347">Fixed some broken links</span></span>
    - <span data-ttu-id="ec939-1348">Nos artigos de New-AzureRmFrontDoor e Set-AzureRmFrontDoor, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorHealthProbeSettingObject.</span><span class="sxs-lookup"><span data-stu-id="ec939-1348">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="ec939-1349">No artigo de New-AzureRmFrontDoorManagedRuleObject, foi corrigida a ligação para o artigo do cmdlet New-AzureRmFrontDoorRuleGroupOverrideObject.</span><span class="sxs-lookup"><span data-stu-id="ec939-1349">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="ec939-1350">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1350">Az.RecoveryServices</span></span>

* <span data-ttu-id="ec939-1351">Foram adicionadas validações do lado do cliente para operações de restauro da Partilha de Ficheiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="ec939-1351">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="ec939-1352">storageAccountName e storageAccountResourceGroupName são agora opções para o restauro de AFS.</span><span class="sxs-lookup"><span data-stu-id="ec939-1352">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="ec939-1353">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1353">Az.Resources</span></span>

* <span data-ttu-id="ec939-1354">Correção para https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="ec939-1354">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="ec939-1355">Atualização de Get-AzureRmRoleAssignment para utilizar o âmbito da subscrição caso este seja fornecido ao pedir administradores clássicos.</span><span class="sxs-lookup"><span data-stu-id="ec939-1355">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="ec939-1356">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1356">Az.Sql</span></span>

* <span data-ttu-id="ec939-1357">Pequenas alterações para a futura transição do AzureRM para Az</span><span class="sxs-lookup"><span data-stu-id="ec939-1357">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="ec939-1358">Foi corrigido o problema relacionado com a utilização de Get-AzureRmSqlDatabaseVulnerabilityAssessment com o núcleo DotNet</span><span class="sxs-lookup"><span data-stu-id="ec939-1358">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="ec939-1359">Modificação na documentação de mensagens de ajuda relacionadas com os cmdlets de Auditoria de SQL.</span><span class="sxs-lookup"><span data-stu-id="ec939-1359">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="ec939-1360">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-1360">Az.Storage</span></span>

* <span data-ttu-id="ec939-1361">-EnableHierarchicalNamespace foi adicionado para New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="ec939-1361">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="ec939-1362">Foi corrigido o problema no qual o cmdlet Copy File não consegue reutilizar o contexto de origem no destino quando não existe a entrada -DestContext</span><span class="sxs-lookup"><span data-stu-id="ec939-1362">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="ec939-1363">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="ec939-1363">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="ec939-1364">Suporte da configuração de Web Site Estático</span><span class="sxs-lookup"><span data-stu-id="ec939-1364">Support Static Website configuration</span></span>
    - <span data-ttu-id="ec939-1365">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ec939-1365">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="ec939-1366">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="ec939-1366">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="ec939-1367">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-1367">Az.Websites</span></span>

* <span data-ttu-id="ec939-1368">Set-AzureRmWebApp e Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="ec939-1368">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="ec939-1369">Foi adicionado o novo parâmetro (-AzureStoragePath) para especificar caminhos de Armazenamento do Azure a montar nas aplicações de contentor do Windows e Linux.</span><span class="sxs-lookup"><span data-stu-id="ec939-1369">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="ec939-1370">Utilize a saída do novo cmdlet New-AzureRmWebAppAzureStoragePath como um parâmetro para definir os caminhos de Armazenamento do Azure.</span><span class="sxs-lookup"><span data-stu-id="ec939-1370">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="ec939-1371">0.6.1 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="ec939-1371">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="ec939-1372">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="ec939-1372">Az.ApiManagement</span></span>
* <span data-ttu-id="ec939-1373">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="ec939-1373">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="ec939-1374">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="ec939-1374">Az.Automation</span></span>
* <span data-ttu-id="ec939-1375">Cmdlets da Automatização do Azure baseados no Swagger</span><span class="sxs-lookup"><span data-stu-id="ec939-1375">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="ec939-1376">Adicionados cmdlets da Gestão de Atualizações</span><span class="sxs-lookup"><span data-stu-id="ec939-1376">Added Update Management cmdlets</span></span>
* <span data-ttu-id="ec939-1377">Adicionados cmdlets de Controlo de Código Fonte</span><span class="sxs-lookup"><span data-stu-id="ec939-1377">Added Source Control cmdlets</span></span>
* <span data-ttu-id="ec939-1378">Adicionado o cmdlet Remove-AzureRmAutomationHybridWorkerGroup</span><span class="sxs-lookup"><span data-stu-id="ec939-1378">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="ec939-1379">Corrigido o comando de Nó de Registo de DSC</span><span class="sxs-lookup"><span data-stu-id="ec939-1379">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="ec939-1380">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1380">Az.Compute</span></span>
* <span data-ttu-id="ec939-1381">Corrigido o problema de identidade da identidade SystemAssigned</span><span class="sxs-lookup"><span data-stu-id="ec939-1381">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="ec939-1382">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="ec939-1382">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="ec939-1383">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="ec939-1383">Az.ContainerInstance</span></span>
* <span data-ttu-id="ec939-1384">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="ec939-1384">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="ec939-1385">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="ec939-1385">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="ec939-1386">Atualização da descrição dos exemplos dos cmdlets do marketplace</span><span class="sxs-lookup"><span data-stu-id="ec939-1386">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="ec939-1387">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1387">Az.Network</span></span>
* <span data-ttu-id="ec939-1388">Adicionado o cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span><span class="sxs-lookup"><span data-stu-id="ec939-1388">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="ec939-1389">Adicionado novamente o ICMP aos Protocolos de Rede do AzureFirewall</span><span class="sxs-lookup"><span data-stu-id="ec939-1389">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="ec939-1390">Atualização do cmdlet Test-AzureRmNetworkWatcherConnectivity, adicionada a validação no ID de destino, no endereço e na porta.</span><span class="sxs-lookup"><span data-stu-id="ec939-1390">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="ec939-1391">Corrigidos os problemas relacionados com a utilização da memória no mapa da VirtualNetwork</span><span class="sxs-lookup"><span data-stu-id="ec939-1391">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="ec939-1392">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="ec939-1392">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="ec939-1393">Correção para modificar a política de uma partilha de ficheiros protegida.</span><span class="sxs-lookup"><span data-stu-id="ec939-1393">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="ec939-1394">Conversão do fuso horário da política em maiúsculas.</span><span class="sxs-lookup"><span data-stu-id="ec939-1394">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="ec939-1395">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="ec939-1395">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="ec939-1396">Exemplo corrigido em New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="ec939-1396">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="ec939-1397">Atualização das dependências para o problema do mapeamento de tipos</span><span class="sxs-lookup"><span data-stu-id="ec939-1397">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="ec939-1398">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="ec939-1398">Az.Relay</span></span>
* <span data-ttu-id="ec939-1399">Adicionado o Parâmetro opcional -KeyValue ao cmdlet New-AzureRmRelayKey, o que permite ao utilizador fornecer o KeyValue.</span><span class="sxs-lookup"><span data-stu-id="ec939-1399">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="ec939-1400">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1400">Az.Resources</span></span>
* <span data-ttu-id="ec939-1401">Atualização da documentação de ajuda dos parâmetros relacionados com a identidade de recursos em `New-AzureRmPolicyAssignment` e `Set-AzureRmPolicyAssignment`</span><span class="sxs-lookup"><span data-stu-id="ec939-1401">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="ec939-1402">Adicionado um exemplo para New-AzureRmPolicyDefinition que utiliza -Metadata</span><span class="sxs-lookup"><span data-stu-id="ec939-1402">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="ec939-1403">Correção para permitir a preservação de maiúsculas e minúsculas nas chaves de Etiqueta no NetStandard: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="ec939-1403">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="ec939-1404">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-1404">Az.ServiceFabric</span></span>
* <span data-ttu-id="ec939-1405">Adicionadas mensagens de preterição para futuras alterações interruptivas</span><span class="sxs-lookup"><span data-stu-id="ec939-1405">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="ec939-1406">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1406">Az.Sql</span></span>
* <span data-ttu-id="ec939-1407">Adicionados novos cmdlets para operações CRUD na Instância Gerida de Base de Dados SQL do Azure e na Base de Dados Gerida SQL do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-1407">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="ec939-1408">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ec939-1408">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ec939-1409">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ec939-1409">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ec939-1410">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ec939-1410">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ec939-1411">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="ec939-1411">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="ec939-1412">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ec939-1412">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ec939-1413">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ec939-1413">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ec939-1414">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ec939-1414">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="ec939-1415">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="ec939-1415">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="ec939-1416">Ativada a gestão da Política de Auditoria Alargada num servidor ou numa base de dados.</span><span class="sxs-lookup"><span data-stu-id="ec939-1416">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="ec939-1417">Adicionado um novo parâmetro (PredicateExpression) para permitir a filtragem de registos de auditoria.</span><span class="sxs-lookup"><span data-stu-id="ec939-1417">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="ec939-1418">Foram modificados cmdlets para utilizar clientes SQL em vez de clientes Legados.</span><span class="sxs-lookup"><span data-stu-id="ec939-1418">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="ec939-1419">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="ec939-1419">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="ec939-1420">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="ec939-1420">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="ec939-1421">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="ec939-1421">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="ec939-1422">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="ec939-1422">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="ec939-1423">Corrigido o problema da utilização de Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings com o parâmetro de nome de conta de armazenamento definido</span><span class="sxs-lookup"><span data-stu-id="ec939-1423">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="ec939-1424">0.5.0 - Novembro de 2018</span><span class="sxs-lookup"><span data-stu-id="ec939-1424">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="ec939-1425">Geral</span><span class="sxs-lookup"><span data-stu-id="ec939-1425">General</span></span>
* <span data-ttu-id="ec939-1426">Foram adicionados Elementos de Preenchimento de Recursos a vários cmdlets de núcleo. Estes permitem percorrer os nomes de recursos existentes ao invocar cmdlets de forma interativa</span><span class="sxs-lookup"><span data-stu-id="ec939-1426">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="ec939-1427">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ec939-1427">Az.Profile</span></span>
* <span data-ttu-id="ec939-1428">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="ec939-1428">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="ec939-1429">O nome do parâmetro TenantId no cmdlet Connect-AzAccount foi mudado para Tenant e foi adicionado um alias para TenantId</span><span class="sxs-lookup"><span data-stu-id="ec939-1429">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="ec939-1430">A descrição de TenantId para Connect-AzAccount foi atualizada</span><span class="sxs-lookup"><span data-stu-id="ec939-1430">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="ec939-1431">Corrigida a mensagem de erro para o início de sessão falhado ao fornecer o domínio de inquilino</span><span class="sxs-lookup"><span data-stu-id="ec939-1431">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="ec939-1432">Corrigido o problema com o nome de contexto em conflito para as contas sem subscrições no inquilino</span><span class="sxs-lookup"><span data-stu-id="ec939-1432">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="ec939-1433">Corrigido o problema com os pontos finais DataLake ao utilizar MSI</span><span class="sxs-lookup"><span data-stu-id="ec939-1433">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="ec939-1434">Foi corrigido o problema no qual "Disconnect-AzAccount" era acionado se não estivesse ligado</span><span class="sxs-lookup"><span data-stu-id="ec939-1434">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="ec939-1435">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1435">Az.CognitiveServices</span></span>
* <span data-ttu-id="ec939-1436">Foi adicionada a operação Get-AzCognitiveServicesAccountSkus.</span><span class="sxs-lookup"><span data-stu-id="ec939-1436">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1437">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1437">Az.Compute</span></span>
* <span data-ttu-id="ec939-1438">Foram adicionados os cmdlets Add-AzVmssVMDataDisk e Remove-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="ec939-1438">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="ec939-1439">Get-AzVMImage mostra AutomaticOSUpgradeProperties</span><span class="sxs-lookup"><span data-stu-id="ec939-1439">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="ec939-1440">Foram corrigidos os valores de opção -BootstrapOptions e -JsonAttribute de SetAzVMChefExtension que não são definidos no formato json.</span><span class="sxs-lookup"><span data-stu-id="ec939-1440">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-1441">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-1441">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-1442">Atualizar o pacote DataLake para 1.1.10.</span><span class="sxs-lookup"><span data-stu-id="ec939-1442">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="ec939-1443">Adicionada a Concorrência predefinida para operações com vários threads.</span><span class="sxs-lookup"><span data-stu-id="ec939-1443">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="ec939-1444">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="ec939-1444">Az.Insights</span></span>
* <span data-ttu-id="ec939-1445">Corrigido o problema n.º 7267 (área de dimensionamento automático)</span><span class="sxs-lookup"><span data-stu-id="ec939-1445">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="ec939-1446">Problemas ao criar uma nova regra de dimensionamento automático não definem corretamente os parâmetros enumerados (são sempre definidos para o valor predefinido).</span><span class="sxs-lookup"><span data-stu-id="ec939-1446">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="ec939-1447">Foi corrigido o problema n.º 7513 [Insights] Set-AzDiagnosticSetting precisa que as categorias sejam especificadas de forma explícita durante a criação da definição</span><span class="sxs-lookup"><span data-stu-id="ec939-1447">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="ec939-1448">Agora o cmdlet não requer indicação explícita das categorias a ativar durante a criação, ou seja, funciona conforme documentado</span><span class="sxs-lookup"><span data-stu-id="ec939-1448">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-1449">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1449">Az.Network</span></span>
* <span data-ttu-id="ec939-1450">Alterado o PeeringType para ser um parâmetro obrigatório para os seguintes cmdlets:-</span><span class="sxs-lookup"><span data-stu-id="ec939-1450">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="ec939-1451">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="ec939-1451">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="ec939-1452">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="ec939-1452">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="ec939-1453">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="ec939-1453">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="ec939-1454">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="ec939-1454">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="ec939-1455">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="ec939-1455">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="ec939-1456">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="ec939-1456">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="ec939-1457">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="ec939-1457">Az.PolicyInsights</span></span>
* <span data-ttu-id="ec939-1458">Adicionados os cmdlets de remediação de política</span><span class="sxs-lookup"><span data-stu-id="ec939-1458">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1459">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1459">Az.Resources</span></span>
* <span data-ttu-id="ec939-1460">Correção para https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="ec939-1460">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="ec939-1461">Permitir a listagem de recursos que utilizam o parâmetro "-ResourceId" para "Get-AzResource"</span><span class="sxs-lookup"><span data-stu-id="ec939-1461">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="ec939-1462">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="ec939-1462">Az.ServiceBus</span></span>
* <span data-ttu-id="ec939-1463">Foi adicionada a propriedade só de leitura MigrationState a PSServiceBusMigrationConfigurationAttributes que ajudam a saber o estado de Migração.</span><span class="sxs-lookup"><span data-stu-id="ec939-1463">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="ec939-1464">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="ec939-1464">Az.ServiceFabric</span></span>
* <span data-ttu-id="ec939-1465">Corrigida a adição de certificado ao Linux VMSS.</span><span class="sxs-lookup"><span data-stu-id="ec939-1465">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="ec939-1466">Correção de "Add-AzServiceFabricClusterCertificate"</span><span class="sxs-lookup"><span data-stu-id="ec939-1466">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="ec939-1467">Utilizar o thumbprint correto a partir do novo certificado (Azure/service-fabric-issues#932).</span><span class="sxs-lookup"><span data-stu-id="ec939-1467">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="ec939-1468">Exibir corretamente a exceção (Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="ec939-1468">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="ec939-1469">Correção de "Update-AzServiceFabricDurability" de modo a atualizar a configuração do cluster antes de iniciar a operação CreateOrUpdate de Vmss.</span><span class="sxs-lookup"><span data-stu-id="ec939-1469">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="ec939-1470">0.4.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="ec939-1470">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="ec939-1471">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="ec939-1471">Az.Profile</span></span>
* <span data-ttu-id="ec939-1472">Foi corrigido o problema de Get-AzSubscription no CloudShell</span><span class="sxs-lookup"><span data-stu-id="ec939-1472">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="ec939-1473">Atualizar o código comum para utilizar a versão mais recente do ClientRuntime</span><span class="sxs-lookup"><span data-stu-id="ec939-1473">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1474">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1474">Az.Compute</span></span>
* <span data-ttu-id="ec939-1475">Foram adicionados novos tamanhos à lista de permissões de tamanhos de VM para os quais serão ativadas redes aceleradas quando for utilizado o conjunto de parâmetros simples para "New-AzVm"</span><span class="sxs-lookup"><span data-stu-id="ec939-1475">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="ec939-1476">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="ec939-1476">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="ec939-1477">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ec939-1477">Az.DataLakeStore</span></span>
* <span data-ttu-id="ec939-1478">Adicionar suporte para as Regras de Rede Virtual</span><span class="sxs-lookup"><span data-stu-id="ec939-1478">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="ec939-1479">Get-AzDataLakeStoreVirtualNetworkRule: Obtém ou lista a regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="ec939-1479">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="ec939-1480">Add-AzDataLakeStoreVirtualNetworkRule: Adiciona uma regra de rede virtual à conta especificada do Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ec939-1480">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="ec939-1481">Set-AzDataLakeStoreVirtualNetworkRule: Modifica a regra de rede virtual especificada na conta do Data Lake Store especificada.</span><span class="sxs-lookup"><span data-stu-id="ec939-1481">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="ec939-1482">Remove-AzDataLakeStoreVirtualNetworkRule: Elimina uma regra de rede virtual do Data Lake Store do Azure.</span><span class="sxs-lookup"><span data-stu-id="ec939-1482">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-1483">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1483">Az.Network</span></span>
* <span data-ttu-id="ec939-1484">Atualização do cmdlet Test-AzNetworkWatcherConnectivity; passagem do valor do protocolo para o back-end.</span><span class="sxs-lookup"><span data-stu-id="ec939-1484">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="ec939-1485">Foi adicionado o preenchedor de argumentos ResourceName a todos os cmdlets.</span><span class="sxs-lookup"><span data-stu-id="ec939-1485">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1486">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1486">Az.Resources</span></span>
* <span data-ttu-id="ec939-1487">Foi corrigido o problema no qual Get-AzRoleDefinition aciona uma exceção ininteligível (quando o perfil predefinido não tem uma subscrição e não é especificado um âmbito) ao adicionar uma exceção com significado no cenário.</span><span class="sxs-lookup"><span data-stu-id="ec939-1487">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="ec939-1488">Também definido o conjunto de parâmetros predefinidos para "RoleDefinitionNameParameterSet".</span><span class="sxs-lookup"><span data-stu-id="ec939-1488">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="ec939-1489">0.3.0 - Outubro de 2018</span><span class="sxs-lookup"><span data-stu-id="ec939-1489">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="ec939-1490">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="ec939-1490">Azure.Storage</span></span>
* <span data-ttu-id="ec939-1491">Correção do problema de a funcionalidade Copiar Blob/Ficheiro não copiar os metadados quando o destino tem metadados</span><span class="sxs-lookup"><span data-stu-id="ec939-1491">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="ec939-1492">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="ec939-1492">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="ec939-1493">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="ec939-1493">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="ec939-1494">Suporte para a obtenção da utilização de recursos do Armazenamento de uma localização específica e adição de uma mensagem de aviso que informa que a obtenção da utilização global de recursos do Armazenamento é obsoleta.</span><span class="sxs-lookup"><span data-stu-id="ec939-1494">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="ec939-1495">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="ec939-1495">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="ec939-1496">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="ec939-1496">Az.CognitiveServices</span></span>
* <span data-ttu-id="ec939-1497">Suporte de Get-AzCognitiveServicesAccountSkus sem uma conta existente.</span><span class="sxs-lookup"><span data-stu-id="ec939-1497">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="ec939-1498">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="ec939-1498">Az.Compute</span></span>
* <span data-ttu-id="ec939-1499">Correção de Get-AzVM -ResourceGroupName <rg> de modo a devolver mais de 50 resultados, se necessário</span><span class="sxs-lookup"><span data-stu-id="ec939-1499">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="ec939-1500">Foi adicionado um exemplo de "SimpleParameterSet" à ajuda do cmdlet New-AzVmss.</span><span class="sxs-lookup"><span data-stu-id="ec939-1500">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="ec939-1501">Correção de um erro de digitação na mensagem de progresso do Azure Disk Encryption</span><span class="sxs-lookup"><span data-stu-id="ec939-1501">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="ec939-1502">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="ec939-1502">Az.DataFactoryV2</span></span>
* <span data-ttu-id="ec939-1503">Atualização da versão do SDK .NET do ADF para a 2.3.0.</span><span class="sxs-lookup"><span data-stu-id="ec939-1503">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="ec939-1504">Az.Network</span><span class="sxs-lookup"><span data-stu-id="ec939-1504">Az.Network</span></span>
* <span data-ttu-id="ec939-1505">Adição da funcionalidade NetworkProfile.</span><span class="sxs-lookup"><span data-stu-id="ec939-1505">Added NetworkProfile functionality.</span></span> <span data-ttu-id="ec939-1506">novos cmdlets adicionados</span><span class="sxs-lookup"><span data-stu-id="ec939-1506">new cmdlets added</span></span>
    - <span data-ttu-id="ec939-1507">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ec939-1507">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="ec939-1508">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ec939-1508">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="ec939-1509">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ec939-1509">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="ec939-1510">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="ec939-1510">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="ec939-1511">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-1511">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="ec939-1512">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-1512">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="ec939-1513">Adição de uma ligação de associação do serviço no Modelo de Sub-rede</span><span class="sxs-lookup"><span data-stu-id="ec939-1513">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="ec939-1514">Foram adicionados os cmdlets New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap e Remove-AzVirtualNetworkTap</span><span class="sxs-lookup"><span data-stu-id="ec939-1514">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="ec939-1515">Foram adicionados os cmdlets Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig e Remove-AzNEtworkInterfaceTapConfig</span><span class="sxs-lookup"><span data-stu-id="ec939-1515">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="ec939-1516">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="ec939-1516">Az.RedisCache</span></span>
* <span data-ttu-id="ec939-1517">Permitir que qualquer cadeia como parâmetro Size permaneça.</span><span class="sxs-lookup"><span data-stu-id="ec939-1517">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="ec939-1518">Adição de P5 no pop-up de PSArgumentCompleter</span><span class="sxs-lookup"><span data-stu-id="ec939-1518">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="ec939-1519">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="ec939-1519">Az.Resources</span></span>
* <span data-ttu-id="ec939-1520">Foi adicionado o parâmetro -Mode em falta a Set-AzPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="ec939-1520">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="ec939-1521">Foi corrigido o erro de cmdlet Get-AzProviderOperation relativo a operações com uma Origem que contém o Utilizador</span><span class="sxs-lookup"><span data-stu-id="ec939-1521">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="ec939-1522">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="ec939-1522">Az.Sql</span></span>
* <span data-ttu-id="ec939-1523">Correção do problema em que alguns cmdlets de cópia de segurança não reconheciam a subscrição atual do Azure</span><span class="sxs-lookup"><span data-stu-id="ec939-1523">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="ec939-1524">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="ec939-1524">Az.Websites</span></span>
* <span data-ttu-id="ec939-1525">Novo Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Obtém o URL do Webhook de Implementação Contínua do Contentor</span><span class="sxs-lookup"><span data-stu-id="ec939-1525">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="ec939-1526">Novos Cmdlets New-AzWebAppContainerPSSession e Enter-WebAppContainerPSSession - Iniciam uma sessão remota do PowerShell numa aplicação de contentor do Windows</span><span class="sxs-lookup"><span data-stu-id="ec939-1526">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="ec939-1527">0.2.0 - Setembro de 2018</span><span class="sxs-lookup"><span data-stu-id="ec939-1527">0.2.0 - September 2018</span></span>
 <span data-ttu-id="ec939-1528">Versão Inicial</span><span class="sxs-lookup"><span data-stu-id="ec939-1528">Initial Release</span></span>
